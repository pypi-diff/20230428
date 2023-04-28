# Comparing `tmp/strongmind_deployment-0.0.8-py3-none-any.whl.zip` & `tmp/strongmind_deployment-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4129 bytes, number of entries: 7
+Zip file size: 4760 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx     2476 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
--rw-r--r--  2.0 unx     3191 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
-?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.8.dist-info/RECORD
-7 files, 8105 bytes uncompressed, 3007 bytes compressed:  62.9%
+-rw-r--r--  2.0 unx     4252 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     3991 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.9.dist-info/RECORD
+7 files, 10681 bytes uncompressed, 3638 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: strongmind_deployment/container.py
 Comment: 
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
-Filename: strongmind_deployment-0.0.8.dist-info/METADATA
+Filename: strongmind_deployment-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-0.0.8.dist-info/WHEEL
+Filename: strongmind_deployment-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-0.0.8.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-0.0.8.dist-info/RECORD
+Filename: strongmind_deployment-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -7,50 +7,90 @@
 from pulumi import Config, export, Output
 
 
 class ContainerComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
+        self._security_group_name = None
         self.container_image = kwargs.get('container_image')
         self.app_path = kwargs.get('app_path') or './'
         self.container_port = kwargs.get('container_port') or 3000
         self.cpu = kwargs.get('cpu') or 256
         self.memory = kwargs.get("memory") or 512
         self.env_vars = kwargs.get('env_vars', {})
 
+        project = pulumi.get_project()
+        self.tags = {
+            "product": project,
+            "repository": project,
+            "service": project,
+            "environment": self.env_vars.get("ENVIRONMENT_NAME", "stage"),
+        }
+
         self.ecs_cluster = aws.ecs.Cluster("cluster",
                                            name=name,
+                                           tags=self.tags,
                                            opts=pulumi.ResourceOptions(parent=self),
                                            )
-        self.load_balancer = awsx.lb.ApplicationLoadBalancer("loadbalancer",
-                                                             name=name,
-                                                             default_target_group_port=self.container_port,
-                                                             opts=pulumi.ResourceOptions(parent=self),
-                                                             )
+        self.load_balancer = awsx.lb.ApplicationLoadBalancer(
+            "loadbalancer",
+            name=name,
+            default_target_group_port=self.container_port,
+            tags=self.tags,
+            opts=pulumi.ResourceOptions(parent=self),
+        )
 
+        load_balancer_arn = kwargs.get('load_balancer_arn', self.load_balancer.load_balancer.arn)
+        target_group_arn = kwargs.get('target_group_arn', self.load_balancer.default_target_group.arn)
+        self.load_balancer_listener = aws.lb.Listener("listener80",
+                                                      port=80,
+                                                      protocol="HTTP",
+                                                      load_balancer_arn=load_balancer_arn,
+                                                      # port=443,
+                                                      # protocol="HTTPS",
+                                                      default_actions=[
+                                                          aws.lb.ListenerDefaultActionArgs(
+                                                              type="forward",
+                                                              target_group_arn=target_group_arn
+                                                          )],
+                                                      )
+        # aws.lb.ListenerArgs(
+        #     port=80,
+        #     protocol="HTTP",
+        #     default_action=awsx.lb.ApplicationListenerDefaultActionArgs(
+        #         type="redirect",
+        #         redirect=awsx.lb.ApplicationListenerDefaultActionRedirectArgs(
+        #             port="443",
+        #             protocol="HTTPS",
+        #             status_code="HTTP_301",
+        #         ),
+        #     )
+        # ),
         task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
-                container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
-                    image=self.container_image,
-                    cpu=self.cpu,
-                    memory=self.memory,
-                    essential=True,
-                    port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
-                        container_port=self.container_port,
-                        host_port=self.container_port,
-                        target_group=self.load_balancer.default_target_group,
-                    )],
-                    environment=[{"name": k, "value": v} for k, v in self.env_vars.items()]
-                )
+            skip_destroy=True,
+            container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
+                image=self.container_image,
+                cpu=self.cpu,
+                memory=self.memory,
+                essential=True,
+                port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
+                    container_port=self.container_port,
+                    host_port=self.container_port,
+                    target_group=self.load_balancer.default_target_group,
+                )],
+                environment=[{"name": k, "value": v} for k, v in self.env_vars.items()]
             )
-
+        )
         self.fargate_service = awsx.ecs.FargateService(
             "service",
             name=f"{name}-service",
             cluster=self.ecs_cluster.arn,
+            continue_before_steady_state=True,
             assign_public_ip=True,
             task_definition_args=task_definition_args,
+            tags=self.tags,
             opts=pulumi.ResourceOptions(parent=self),
         )
 
         export("url", Output.concat("http://", self.load_balancer.load_balancer.dns_name))
         self.register_outputs({})
```

## strongmind_deployment/rails.py

```diff
@@ -7,36 +7,61 @@
 
 from strongmind_deployment.container import ContainerComponent
 
 
 class RailsComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:rails', name, None, opts)
+        self.firewall_rule = None
         self.db_password = None
         self.container = None
         self.rds_serverless_cluster_instance = None
         self.rds_serverless_cluster = None
         self.kwargs = kwargs
 
         self.rds(name)
 
         self.ecs(name)
 
-        self.register_outputs({
-            'rds_serverless_cluster': self.rds_serverless_cluster.cluster_identifier
-        })
+        self.security()
+
+        self.register_outputs({})
+
+    def security(self):
+        container_security_group_id = self.kwargs.get(
+            'container_security_group_id',
+            self.container.fargate_service.service.network_configuration.security_groups[0])  # pragma: no cover
+
+        self.firewall_rule = aws.ec2.SecurityGroupRule(
+            'rds_security_group_rule',
+            type='ingress',
+            from_port=5432,
+            to_port=5432,
+            protocol='tcp',
+            security_group_id=self.rds_serverless_cluster.vpc_security_group_ids[0],
+            source_security_group_id=container_security_group_id,
+            opts=pulumi.ResourceOptions(parent=self,
+                                        depends_on=[self.rds_serverless_cluster_instance,
+                                                    self.container])
+        )
 
     def ecs(self, name):
         if 'env_vars' not in self.kwargs:
             self.kwargs['env_vars'] = {}
 
-        self.kwargs['env_vars']['DATABASE_HOST'] = self.rds_serverless_cluster.endpoint
-        self.kwargs['env_vars']['DB_USERNAME'] = self.rds_serverless_cluster.master_username
-        self.kwargs['env_vars']['DB_PASSWORD'] = self.rds_serverless_cluster.master_password
-        self.kwargs['env_vars']['DATABASE_URL'] = self.get_database_url()
+        additional_env_vars = {
+            'DATABASE_HOST': self.rds_serverless_cluster.endpoint,
+            'DB_USERNAME': self.rds_serverless_cluster.master_username,
+            'DB_PASSWORD': self.rds_serverless_cluster.master_password,
+            'DATABASE_URL': self.get_database_url(),
+            'RAILS_ENV': 'production'
+        }
+
+        self.kwargs['env_vars'].update(additional_env_vars)
+
         self.container = ContainerComponent(name,
                                             pulumi.ResourceOptions(parent=self),
                                             **self.kwargs
                                             )
 
     def rds(self, name):
         self.db_password = random.RandomPassword("password",
@@ -44,14 +69,15 @@
                                                  special=False)
         self.rds_serverless_cluster = aws.rds.Cluster(
             'rds_serverless_cluster',
             cluster_identifier=name,
             engine='aurora-postgresql',
             engine_mode='provisioned',
             engine_version='15.2',
+            database_name="app",
             master_username=name.replace('-', '_'),
             master_password=self.db_password.result,
             opts=pulumi.ResourceOptions(parent=self),
             serverlessv2_scaling_configuration=aws.rds.ClusterServerlessv2ScalingConfigurationArgs(
                 min_capacity=0.5,
                 max_capacity=16,
             )
@@ -70,9 +96,8 @@
     def get_database_url(self):
         return Output.concat('postgres://',
                              self.rds_serverless_cluster.master_username,
                              ':',
                              self.rds_serverless_cluster.master_password,
                              '@',
                              self.rds_serverless_cluster.endpoint,
-                             ':5432/',
-                             self.rds_serverless_cluster.master_username)
+                             ':5432/app')
```

## Comparing `strongmind_deployment-0.0.8.dist-info/METADATA` & `strongmind_deployment-0.0.9.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-0.0.8.dist-info/licenses/LICENSE` & `strongmind_deployment-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-0.0.8.dist-info/RECORD` & `strongmind_deployment-0.0.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-strongmind_deployment/container.py,sha256=zJirxtLBlHI-i2e7Zg_8CbI0j6OmBKo2ax2xmVZ3uPw,2476
-strongmind_deployment/rails.py,sha256=Y2JjgIwQNJcdqiyumFbRDprpSVkFDnAO22Fc5EGRo0k,3191
-strongmind_deployment-0.0.8.dist-info/METADATA,sha256=Bc5SYZW2Sob2cnQ7PwHsAYnx7_dZpvE35xk9yJJ_xhU,675
-strongmind_deployment-0.0.8.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-strongmind_deployment-0.0.8.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-0.0.8.dist-info/RECORD,,
+strongmind_deployment/container.py,sha256=Bs2N49dywfdi4Lbt4GoK6t_dZpLRUt-PMXC4QDcNHEQ,4252
+strongmind_deployment/rails.py,sha256=Y5ZH7BsyluAHn2IAXwHUAMTPLEpBSsEnqEnVA-RElC0,3991
+strongmind_deployment-0.0.9.dist-info/METADATA,sha256=90j0gDOb5zUOozsoncVA2SsEdOOPro3Z58_7UZNm24o,675
+strongmind_deployment-0.0.9.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+strongmind_deployment-0.0.9.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-0.0.9.dist-info/RECORD,,
```

