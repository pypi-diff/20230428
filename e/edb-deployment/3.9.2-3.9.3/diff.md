# Comparing `tmp/edb-deployment-3.9.2.tar.gz` & `tmp/edb-deployment-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edb-deployment-3.9.2.tar", last modified: Tue Jan 25 09:17:35 2022, max compression
+gzip compressed data, was "edb-deployment-3.9.3.tar", last modified: Fri Jan 28 14:54:28 2022, max compression
```

## Comparing `edb-deployment-3.9.2.tar` & `edb-deployment-3.9.3.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.141407 edb-deployment-3.9.2/
--rw-r--r--   0 julien     (501) staff       (20)     1434 2021-07-05 08:10:53.000000 edb-deployment-3.9.2/LICENSE.md
--rw-r--r--   0 julien     (501) staff       (20)    13709 2022-01-25 09:17:35.141003 edb-deployment-3.9.2/PKG-INFO
--rw-r--r--   0 julien     (501) staff       (20)    12924 2021-11-22 13:27:33.000000 edb-deployment-3.9.2/README.md
--rwxr-xr-x   0 julien     (501) staff       (20)      138 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edb-deployment
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.973242 edb-deployment-3.9.2/edb_deployment.egg-info/
--rw-r--r--   0 julien     (501) staff       (20)    13709 2022-01-25 09:17:33.000000 edb-deployment-3.9.2/edb_deployment.egg-info/PKG-INFO
--rw-r--r--   0 julien     (501) staff       (20)    12133 2022-01-25 09:17:33.000000 edb-deployment-3.9.2/edb_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 julien     (501) staff       (20)        1 2022-01-25 09:17:33.000000 edb-deployment-3.9.2/edb_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 julien     (501) staff       (20)       33 2022-01-25 09:17:33.000000 edb-deployment-3.9.2/edb_deployment.egg-info/requires.txt
--rw-r--r--   0 julien     (501) staff       (20)       10 2022-01-25 09:17:33.000000 edb-deployment-3.9.2/edb_deployment.egg-info/top_level.txt
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.982606 edb-deployment-3.9.2/edbdeploy/
--rw-r--r--   0 julien     (501) staff       (20)      819 2022-01-25 09:17:12.000000 edb-deployment-3.9.2/edbdeploy/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     1523 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/action.py
--rw-r--r--   0 julien     (501) staff       (20)     8327 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/ansible.py
--rw-r--r--   0 julien     (501) staff       (20)     5753 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/cli.py
--rw-r--r--   0 julien     (501) staff       (20)    24968 2021-07-29 08:12:39.000000 edb-deployment-3.9.2/edbdeploy/cloud.py
--rw-r--r--   0 julien     (501) staff       (20)     7045 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/command.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.990586 edb-deployment-3.9.2/edbdeploy/commands/
--rw-r--r--   0 julien     (501) staff       (20)        0 2021-07-29 08:12:39.000000 edb-deployment-3.9.2/edbdeploy/commands/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     5047 2021-07-29 08:12:39.000000 edb-deployment-3.9.2/edbdeploy/commands/aurora.py
--rw-r--r--   0 julien     (501) staff       (20)     5361 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/commands/aws.py
--rw-r--r--   0 julien     (501) staff       (20)     5464 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/commands/aws_pot.py
--rw-r--r--   0 julien     (501) staff       (20)     5116 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/commands/azure.py
--rw-r--r--   0 julien     (501) staff       (20)     4769 2021-07-29 08:12:39.000000 edb-deployment-3.9.2/edbdeploy/commands/azure_db.py
--rw-r--r--   0 julien     (501) staff       (20)     6584 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/commands/azure_pot.py
--rw-r--r--   0 julien     (501) staff       (20)     4699 2021-11-22 13:27:33.000000 edb-deployment-3.9.2/edbdeploy/commands/baremetal.py
--rw-r--r--   0 julien     (501) staff       (20)     2492 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/commands/default.py
--rw-r--r--   0 julien     (501) staff       (20)     5717 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/commands/gcloud.py
--rw-r--r--   0 julien     (501) staff       (20)     7185 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/commands/gcloud_pot.py
--rw-r--r--   0 julien     (501) staff       (20)     5365 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/commands/gcloud_sql.py
--rw-r--r--   0 julien     (501) staff       (20)     5006 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/commands/rds.py
--rw-r--r--   0 julien     (501) staff       (20)     5961 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/commands/virtualbox.py
--rw-r--r--   0 julien     (501) staff       (20)     5963 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/commands/vmware.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.959458 edb-deployment-3.9.2/edbdeploy/data/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.994835 edb-deployment-3.9.2/edbdeploy/data/ansible/
--rw-r--r--   0 julien     (501) staff       (20)     1828 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-Always-On-Platinum.yml
--rw-r--r--   0 julien     (501) staff       (20)     1826 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-Always-On-Silver.yml
--rw-r--r--   0 julien     (501) staff       (20)     1612 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA-1.yml
--rw-r--r--   0 julien     (501) staff       (20)     1478 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA-2.yml
--rw-r--r--   0 julien     (501) staff       (20)     1720 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA-3.yml
--rw-r--r--   0 julien     (501) staff       (20)     1606 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA.yml
--rw-r--r--   0 julien     (501) staff       (20)      943 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/HammerDB-DBaaS.yml
--rw-r--r--   0 julien     (501) staff       (20)      937 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/HammerDB-TPROC-C.yml
--rw-r--r--   0 julien     (501) staff       (20)     2016 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/POT-Remove-Project-Route53.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.950656 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.950520 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.995624 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/defaults/
--rw-r--r--   0 julien     (501) staff       (20)      932 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/defaults/main.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.996354 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/handlers/
--rw-r--r--   0 julien     (501) staff       (20)       33 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/handlers/main.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.019003 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/
--rw-r--r--   0 julien     (501) staff       (20)      319 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/bdr_setup.yml
--rw-r--r--   0 julien     (501) staff       (20)      791 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/main.yml
--rw-r--r--   0 julien     (501) staff       (20)     1916 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/os_configure_user.yml
--rw-r--r--   0 julien     (501) staff       (20)     2275 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_certs.yml
--rw-r--r--   0 julien     (501) staff       (20)     2761 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_probe_alert.yml
--rw-r--r--   0 julien     (501) staff       (20)     2294 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_create_user.yml
--rw-r--r--   0 julien     (501) staff       (20)      423 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_hba_rule.yml
--rw-r--r--   0 julien     (501) staff       (20)     1141 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_hba.yml
--rw-r--r--   0 julien     (501) staff       (20)      999 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_scripts.yml
--rw-r--r--   0 julien     (501) staff       (20)     2431 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_user_pgpass.yml
--rw-r--r--   0 julien     (501) staff       (20)     1805 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/update_route53.yml
--rw-r--r--   0 julien     (501) staff       (20)     1171 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/verify_variables.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.024036 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/
--rwxr-xr-x   0 julien     (501) staff       (20)     3880 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/barman-backup-monitor.py.template
--rw-r--r--   0 julien     (501) staff       (20)     2348 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/data_view.sql
--rw-r--r--   0 julien     (501) staff       (20)     4480 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/harp-proxy-pgbouncer-monitor.sh.templates
--rw-r--r--   0 julien     (501) staff       (20)    15076 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_bdr_probe.sql.template
--rw-r--r--   0 julien     (501) staff       (20)     8925 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_charts.sql.template
--rw-r--r--   0 julien     (501) staff       (20)     5877 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.platinum.template
--rw-r--r--   0 julien     (501) staff       (20)     5174 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.silver.template
--rw-r--r--   0 julien     (501) staff       (20)     4091 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_probe_alert.sql
--rw-r--r--   0 julien     (501) staff       (20)      127 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pg_env_dbserver.sh.template
--rw-r--r--   0 julien     (501) staff       (20)      118 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pg_env_pgbouncer.sh.template
--rw-r--r--   0 julien     (501) staff       (20)      162 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pot_aliases.sh.template
--rw-r--r--   0 julien     (501) staff       (20)      507 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/sudo_user.template
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.025034 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/
--rw-r--r--   0 julien     (501) staff       (20)      537 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/EPAS.yml
--rw-r--r--   0 julien     (501) staff       (20)      272 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/PG.yml
--rw-r--r--   0 julien     (501) staff       (20)       34 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/main.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.951248 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.025405 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/defaults/
--rw-r--r--   0 julien     (501) staff       (20)      857 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/defaults/main.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.025750 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/handlers/
--rw-r--r--   0 julien     (501) staff       (20)       33 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/handlers/main.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.031569 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/
--rw-r--r--   0 julien     (501) staff       (20)     1158 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/efm_scripts_rules.yml
--rw-r--r--   0 julien     (501) staff       (20)      807 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/main.yml
--rw-r--r--   0 julien     (501) staff       (20)      851 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/os_configure_user.yml
--rw-r--r--   0 julien     (501) staff       (20)     2109 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pem_server_certs.yml
--rw-r--r--   0 julien     (501) staff       (20)      398 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pem_server_probe_alert.yml
--rw-r--r--   0 julien     (501) staff       (20)     1692 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_create_user.yml
--rw-r--r--   0 julien     (501) staff       (20)      450 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_hba_rule.yml
--rw-r--r--   0 julien     (501) staff       (20)     1148 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_pot_hba.yml
--rw-r--r--   0 julien     (501) staff       (20)      343 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_pot_scripts.yml
--rw-r--r--   0 julien     (501) staff       (20)     1661 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_user_pgpass.yml
--rw-r--r--   0 julien     (501) staff       (20)      415 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pot_setup.yml
--rw-r--r--   0 julien     (501) staff       (20)     1854 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/update_route53.yml
--rw-r--r--   0 julien     (501) staff       (20)     1171 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/verify_variables.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.038621 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/
--rwxr-xr-x   0 julien     (501) staff       (20)    17523 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.3.10.template
--rw-r--r--   0 julien     (501) staff       (20)    17524 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.0.template
--rwxr-xr-x   0 julien     (501) staff       (20)    18524 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.1.template
--rw-r--r--   0 julien     (501) staff       (20)     2137 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_reconfigure_node.sh.template
--rw-r--r--   0 julien     (501) staff       (20)     4006 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_rewind.sh.template
--rw-r--r--   0 julien     (501) staff       (20)     1231 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_sudo.template
--rw-r--r--   0 julien     (501) staff       (20)     1081 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/pem_probe_alert.sql
--rw-r--r--   0 julien     (501) staff       (20)      126 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/pg_env_dbserver.sh.template
--rw-r--r--   0 julien     (501) staff       (20)      265 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/pot_aliases.sh.template
--rw-r--r--   0 julien     (501) staff       (20)      553 2021-08-02 14:19:30.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/sudo_user.template
--rw-r--r--   0 julien     (501) staff       (20)      296 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/tuned.conf.template
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.039973 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/vars/
--rw-r--r--   0 julien     (501) staff       (20)      556 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/vars/EPAS.yml
--rw-r--r--   0 julien     (501) staff       (20)      272 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/vars/PG.yml
--rw-r--r--   0 julien     (501) staff       (20)       29 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/vars/main.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.044429 edb-deployment-3.9.2/edbdeploy/data/templates/
--rw-r--r--   0 julien     (501) staff       (20)     4762 2022-01-25 09:08:43.000000 edb-deployment-3.9.2/edbdeploy/data/templates/config.yml.j2
--rw-r--r--   0 julien     (501) staff       (20)     6339 2022-01-25 09:08:43.000000 edb-deployment-3.9.2/edbdeploy/data/templates/inventory.yml.j2
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.957882 edb-deployment-3.9.2/edbdeploy/data/terraform/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.046595 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.955029 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.079403 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/ec2/
--rw-r--r--   0 julien     (501) staff       (20)    17311 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/ec2/ec2.tf
--rw-r--r--   0 julien     (501) staff       (20)     4191 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/ec2/outputs.tf
--rwxr-xr-x   0 julien     (501) staff       (20)      416 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/ec2/setup_volume.sh
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.080150 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/network/
--rw-r--r--   0 julien     (501) staff       (20)      791 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/network/network.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.080649 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/policies/
--rw-r--r--   0 julien     (501) staff       (20)      836 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/policies/policy.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.081056 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/routes/
--rw-r--r--   0 julien     (501) staff       (20)     1519 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/routes/routes.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.082321 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/security/
--rw-r--r--   0 julien     (501) staff       (20)       85 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/security/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)     3373 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/security/security.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.083250 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/vpc/
--rw-r--r--   0 julien     (501) staff       (20)       46 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/vpc/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)      248 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/vpc/vpc.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.955258 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/global/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.084438 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/global/iam/
--rw-r--r--   0 julien     (501) staff       (20)      358 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/global/iam/iam.tf
--rw-r--r--   0 julien     (501) staff       (20)      125 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/global/iam/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)     3019 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/main.tf
--rw-r--r--   0 julien     (501) staff       (20)       45 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/provider.tf
--rw-r--r--   0 julien     (501) staff       (20)     1462 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/tags.tf.template
--rw-r--r--   0 julien     (501) staff       (20)     1357 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws/variables.tf.template
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.048464 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.953902 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.070314 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/aws/
--rw-r--r--   0 julien     (501) staff       (20)     7132 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/aws/aws.tf
--rw-r--r--   0 julien     (501) staff       (20)     2210 2021-12-17 09:43:12.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/aws/outputs.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.070849 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/network/
--rw-r--r--   0 julien     (501) staff       (20)      791 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/network/network.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.071410 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/policies/
--rw-r--r--   0 julien     (501) staff       (20)      836 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/policies/policy.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.073858 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/routes/
--rw-r--r--   0 julien     (501) staff       (20)     1208 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/routes/routes.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.074862 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/security/
--rw-r--r--   0 julien     (501) staff       (20)      161 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/security/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)     1855 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/security/security.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.075886 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/vpc/
--rw-r--r--   0 julien     (501) staff       (20)       46 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/vpc/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)      248 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/vpc/vpc.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.954127 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/global/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.077333 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/global/iam/
--rw-r--r--   0 julien     (501) staff       (20)      358 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/global/iam/iam.tf
--rw-r--r--   0 julien     (501) staff       (20)      125 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/global/iam/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)     2506 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/main.tf
--rw-r--r--   0 julien     (501) staff       (20)       45 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/provider.tf
--rw-r--r--   0 julien     (501) staff       (20)     1462 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/tags.tf.template
--rw-r--r--   0 julien     (501) staff       (20)     1258 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/variables.tf.template
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.049975 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.952703 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.050585 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/
--rw-r--r--   0 julien     (501) staff       (20)     5944 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/aws.tf
--rw-r--r--   0 julien     (501) staff       (20)     1979 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/outputs.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.066286 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/network/
--rw-r--r--   0 julien     (501) staff       (20)      791 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/network/network.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.066755 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/policies/
--rw-r--r--   0 julien     (501) staff       (20)      836 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/policies/policy.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.067186 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/routes/
--rw-r--r--   0 julien     (501) staff       (20)     1208 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/routes/routes.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.067925 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/security/
--rw-r--r--   0 julien     (501) staff       (20)      161 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/security/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)     1855 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/security/security.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.068547 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/vpc/
--rw-r--r--   0 julien     (501) staff       (20)       46 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/vpc/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)      248 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/vpc/vpc.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.952920 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/global/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.069248 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/global/iam/
--rw-r--r--   0 julien     (501) staff       (20)      358 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/global/iam/iam.tf
--rw-r--r--   0 julien     (501) staff       (20)      125 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/global/iam/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)     2407 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/main.tf
--rw-r--r--   0 julien     (501) staff       (20)       45 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/provider.tf
--rw-r--r--   0 julien     (501) staff       (20)     1462 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/tags.tf.template
--rw-r--r--   0 julien     (501) staff       (20)     1155 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/variables.tf.template
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.086520 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.957596 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.093625 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/network/
--rw-r--r--   0 julien     (501) staff       (20)      367 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/network/network.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.094058 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/resourcegroup/
--rw-r--r--   0 julien     (501) staff       (20)      264 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/resourcegroup/rg.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.094438 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/security/
--rw-r--r--   0 julien     (501) staff       (20)     5984 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/security/security.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.094974 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/storageaccount/
--rw-r--r--   0 julien     (501) staff       (20)      500 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/storageaccount/storageaccount.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.095493 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/storagecontainer/
--rw-r--r--   0 julien     (501) staff       (20)      333 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/storagecontainer/storagecontainer.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.098015 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm/
--rw-r--r--   0 julien     (501) staff       (20)     4133 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm/outputs.tf
--rwxr-xr-x   0 julien     (501) staff       (20)      416 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm/setup_volume.sh
--rw-r--r--   0 julien     (501) staff       (20)    24134 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm/vm.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.099765 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm-hammerdb/
--rw-r--r--   0 julien     (501) staff       (20)     2014 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm-hammerdb/outputs.tf
--rwxr-xr-x   0 julien     (501) staff       (20)      349 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm-hammerdb/setup_volume.sh
--rw-r--r--   0 julien     (501) staff       (20)    15922 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm-hammerdb/vm-hammerdb.tf
--rw-r--r--   0 julien     (501) staff       (20)     4602 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/main.tf
--rw-r--r--   0 julien     (501) staff       (20)      161 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/provider.tf
--rw-r--r--   0 julien     (501) staff       (20)     1181 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/tags.tf.template
--rw-r--r--   0 julien     (501) staff       (20)      965 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure/variables.tf.template
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.089661 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.956451 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.090257 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/network/
--rw-r--r--   0 julien     (501) staff       (20)      367 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/network/network.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.090757 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/resourcegroup/
--rw-r--r--   0 julien     (501) staff       (20)      264 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/resourcegroup/rg.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.091239 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/security/
--rw-r--r--   0 julien     (501) staff       (20)     2611 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/security/security.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.091758 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/storageaccount/
--rw-r--r--   0 julien     (501) staff       (20)      500 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/storageaccount/storageaccount.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.092240 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/storagecontainer/
--rw-r--r--   0 julien     (501) staff       (20)      286 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/storagecontainer/storagecontainer.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.093166 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/vm/
--rw-r--r--   0 julien     (501) staff       (20)     3681 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/vm/outputs.tf
--rw-r--r--   0 julien     (501) staff       (20)    12813 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/vm/vm.tf
--rw-r--r--   0 julien     (501) staff       (20)     2371 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/main.tf
--rw-r--r--   0 julien     (501) staff       (20)       58 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/provider.tf
--rw-r--r--   0 julien     (501) staff       (20)     1181 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/tags.tf.template
--rw-r--r--   0 julien     (501) staff       (20)      862 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/variables.tf.template
--rw-r--r--   0 julien     (501) staff       (20)      129 2022-01-25 09:08:43.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/versions.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.117286 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.958851 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.120902 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/compute/
--rw-r--r--   0 julien     (501) staff       (20)    20023 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/compute/compute.tf
--rw-r--r--   0 julien     (501) staff       (20)     4250 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/compute/outputs.tf
--rwxr-xr-x   0 julien     (501) staff       (20)      416 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/compute/setup_volume.sh
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.121453 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/network/
--rw-r--r--   0 julien     (501) staff       (20)      489 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/network/network.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.121826 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/security/
--rw-r--r--   0 julien     (501) staff       (20)     6580 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/security/firewall.tf
--rw-r--r--   0 julien     (501) staff       (20)     1813 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/main.tf
--rw-r--r--   0 julien     (501) staff       (20)       99 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/provider.tf
--rw-r--r--   0 julien     (501) staff       (20)     1183 2021-11-22 13:27:33.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/tags.tf.template
--rw-r--r--   0 julien     (501) staff       (20)     1230 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/variables.tf.template
--rw-r--r--   0 julien     (501) staff       (20)      127 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/versions.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.118664 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.958376 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.119320 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/compute/
--rw-r--r--   0 julien     (501) staff       (20)    11483 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/compute/compute.tf
--rw-r--r--   0 julien     (501) staff       (20)     2928 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/compute/outputs.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.119631 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/network/
--rw-r--r--   0 julien     (501) staff       (20)      489 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/network/network.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.119933 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/security/
--rw-r--r--   0 julien     (501) staff       (20)     2899 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/security/firewall.tf
--rw-r--r--   0 julien     (501) staff       (20)     1397 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/main.tf
--rw-r--r--   0 julien     (501) staff       (20)       99 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/provider.tf
--rw-r--r--   0 julien     (501) staff       (20)     1104 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/variables.tf.template
--rw-r--r--   0 julien     (501) staff       (20)      127 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/versions.tf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:34.959063 edb-deployment-3.9.2/edbdeploy/data/tpaexec/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.122452 edb-deployment-3.9.2/edbdeploy/data/tpaexec/hooks/
--rw-r--r--   0 julien     (501) staff       (20)     2728 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/tpaexec/hooks/post-deploy.yml
--rw-r--r--   0 julien     (501) staff       (20)      398 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/data/tpaexec/hooks/pre-initdb.yml
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.123053 edb-deployment-3.9.2/edbdeploy/data/tpaexec/hooks/templates/
--rw-r--r--   0 julien     (501) staff       (20)       62 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/tpaexec/hooks/templates/harp-manager.override.conf
--rw-r--r--   0 julien     (501) staff       (20)       62 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/data/tpaexec/hooks/templates/harp-proxy.override.conf
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.123943 edb-deployment-3.9.2/edbdeploy/data/virtualbox/
--rwxr-xr-x   0 julien     (501) staff       (20)     2018 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/virtualbox/c8-EDB-RA-1
--rwxr-xr-x   0 julien     (501) staff       (20)     2434 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/virtualbox/c8-EDB-RA-2
--rwxr-xr-x   0 julien     (501) staff       (20)     2818 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/data/virtualbox/c8-EDB-RA-3
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.125129 edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/
--rwxr-xr-x   0 julien     (501) staff       (20)     1040 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/c8-EDB-RA-1
--rwxr-xr-x   0 julien     (501) staff       (20)     1738 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/c8-EDB-RA-2
--rwxr-xr-x   0 julien     (501) staff       (20)     2779 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/c8-EDB-RA-3
--rwxr-xr-x   0 julien     (501) staff       (20)     1349 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/playbook.yml
--rw-r--r--   0 julien     (501) staff       (20)      397 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/errors.py
--rw-r--r--   0 julien     (501) staff       (20)     1990 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/installation.py
--rw-r--r--   0 julien     (501) staff       (20)    10018 2022-01-25 09:08:43.000000 edb-deployment-3.9.2/edbdeploy/options.py
--rw-r--r--   0 julien     (501) staff       (20)     1612 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/password.py
--rw-r--r--   0 julien     (501) staff       (20)    63378 2022-01-25 09:08:43.000000 edb-deployment-3.9.2/edbdeploy/project.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.132893 edb-deployment-3.9.2/edbdeploy/projects/
--rw-r--r--   0 julien     (501) staff       (20)        0 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/projects/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     4342 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/projects/aws.py
--rw-r--r--   0 julien     (501) staff       (20)     8362 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/projects/aws_pot.py
--rw-r--r--   0 julien     (501) staff       (20)     5101 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/projects/aws_rds.py
--rw-r--r--   0 julien     (501) staff       (20)     1121 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/projects/aws_rds_aurora.py
--rw-r--r--   0 julien     (501) staff       (20)     3907 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/projects/azure.py
--rw-r--r--   0 julien     (501) staff       (20)     4240 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/projects/azure_db.py
--rw-r--r--   0 julien     (501) staff       (20)     7934 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/projects/azure_pot.py
--rw-r--r--   0 julien     (501) staff       (20)     2985 2021-11-17 15:19:50.000000 edb-deployment-3.9.2/edbdeploy/projects/baremetal.py
--rw-r--r--   0 julien     (501) staff       (20)     4416 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/projects/gcloud.py
--rw-r--r--   0 julien     (501) staff       (20)     8099 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/edbdeploy/projects/gcloud_pot.py
--rw-r--r--   0 julien     (501) staff       (20)     2535 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/projects/gcloud_sql.py
--rw-r--r--   0 julien     (501) staff       (20)    19772 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/projects/virtualbox.py
--rw-r--r--   0 julien     (501) staff       (20)    18871 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/projects/vmware.py
--rw-r--r--   0 julien     (501) staff       (20)     1385 2022-01-25 09:12:40.000000 edb-deployment-3.9.2/edbdeploy/render.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-25 09:17:35.140169 edb-deployment-3.9.2/edbdeploy/spec/
--rw-r--r--   0 julien     (501) staff       (20)    14424 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     7419 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/aws.py
--rw-r--r--   0 julien     (501) staff       (20)     1472 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/aws_rds.py
--rw-r--r--   0 julien     (501) staff       (20)      423 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/aws_rds_aurora.py
--rw-r--r--   0 julien     (501) staff       (20)     5358 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/azure.py
--rw-r--r--   0 julien     (501) staff       (20)     1204 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/azure_db.py
--rw-r--r--   0 julien     (501) staff       (20)     4559 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/spec/baremetal.py
--rw-r--r--   0 julien     (501) staff       (20)     5586 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/gcloud.py
--rw-r--r--   0 julien     (501) staff       (20)     1346 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/gcloud_sql.py
--rw-r--r--   0 julien     (501) staff       (20)     4506 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/spec/reference_architecture.py
--rw-r--r--   0 julien     (501) staff       (20)     2196 2021-11-02 13:36:41.000000 edb-deployment-3.9.2/edbdeploy/spec/virtualbox.py
--rw-r--r--   0 julien     (501) staff       (20)     4591 2021-12-21 12:52:56.000000 edb-deployment-3.9.2/edbdeploy/spec/vmware.py
--rw-r--r--   0 julien     (501) staff       (20)     5081 2021-10-25 08:14:11.000000 edb-deployment-3.9.2/edbdeploy/specifications.py
--rw-r--r--   0 julien     (501) staff       (20)      888 2021-09-14 06:41:50.000000 edb-deployment-3.9.2/edbdeploy/system.py
--rw-r--r--   0 julien     (501) staff       (20)     8390 2021-09-13 15:20:44.000000 edb-deployment-3.9.2/edbdeploy/terraform.py
--rw-r--r--   0 julien     (501) staff       (20)     6423 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/tpaexec.py
--rw-r--r--   0 julien     (501) staff       (20)    10883 2021-08-30 12:22:34.000000 edb-deployment-3.9.2/edbdeploy/virtualbox.py
--rw-r--r--   0 julien     (501) staff       (20)    12570 2021-07-29 08:12:40.000000 edb-deployment-3.9.2/edbdeploy/vmware.py
--rw-r--r--   0 julien     (501) staff       (20)       38 2022-01-25 09:17:35.141497 edb-deployment-3.9.2/setup.cfg
--rw-r--r--   0 julien     (501) staff       (20)     2535 2022-01-25 08:38:31.000000 edb-deployment-3.9.2/setup.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:28.263844 edb-deployment-3.9.3/
+-rw-r--r--   0 julien     (501) staff       (20)     1434 2021-07-05 08:10:53.000000 edb-deployment-3.9.3/LICENSE.md
+-rw-r--r--   0 julien     (501) staff       (20)    13709 2022-01-28 14:54:28.262983 edb-deployment-3.9.3/PKG-INFO
+-rw-r--r--   0 julien     (501) staff       (20)    12924 2021-11-22 13:27:33.000000 edb-deployment-3.9.3/README.md
+-rwxr-xr-x   0 julien     (501) staff       (20)      138 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edb-deployment
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.959771 edb-deployment-3.9.3/edb_deployment.egg-info/
+-rw-r--r--   0 julien     (501) staff       (20)    13709 2022-01-28 14:54:24.000000 edb-deployment-3.9.3/edb_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 julien     (501) staff       (20)    12133 2022-01-28 14:54:24.000000 edb-deployment-3.9.3/edb_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 julien     (501) staff       (20)        1 2022-01-28 14:54:24.000000 edb-deployment-3.9.3/edb_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 julien     (501) staff       (20)       33 2022-01-28 14:54:24.000000 edb-deployment-3.9.3/edb_deployment.egg-info/requires.txt
+-rw-r--r--   0 julien     (501) staff       (20)       10 2022-01-28 14:54:24.000000 edb-deployment-3.9.3/edb_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.126359 edb-deployment-3.9.3/edbdeploy/
+-rw-r--r--   0 julien     (501) staff       (20)      819 2022-01-28 14:54:16.000000 edb-deployment-3.9.3/edbdeploy/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     1523 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/action.py
+-rw-r--r--   0 julien     (501) staff       (20)     8327 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/ansible.py
+-rw-r--r--   0 julien     (501) staff       (20)     5753 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/cli.py
+-rw-r--r--   0 julien     (501) staff       (20)    24968 2021-07-29 08:12:39.000000 edb-deployment-3.9.3/edbdeploy/cloud.py
+-rw-r--r--   0 julien     (501) staff       (20)     7045 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/command.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.267528 edb-deployment-3.9.3/edbdeploy/commands/
+-rw-r--r--   0 julien     (501) staff       (20)        0 2021-07-29 08:12:39.000000 edb-deployment-3.9.3/edbdeploy/commands/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     5047 2021-07-29 08:12:39.000000 edb-deployment-3.9.3/edbdeploy/commands/aurora.py
+-rw-r--r--   0 julien     (501) staff       (20)     5361 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/commands/aws.py
+-rw-r--r--   0 julien     (501) staff       (20)     5464 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/commands/aws_pot.py
+-rw-r--r--   0 julien     (501) staff       (20)     5116 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/commands/azure.py
+-rw-r--r--   0 julien     (501) staff       (20)     4769 2021-07-29 08:12:39.000000 edb-deployment-3.9.3/edbdeploy/commands/azure_db.py
+-rw-r--r--   0 julien     (501) staff       (20)     6584 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/commands/azure_pot.py
+-rw-r--r--   0 julien     (501) staff       (20)     4699 2021-11-22 13:27:33.000000 edb-deployment-3.9.3/edbdeploy/commands/baremetal.py
+-rw-r--r--   0 julien     (501) staff       (20)     2492 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/commands/default.py
+-rw-r--r--   0 julien     (501) staff       (20)     5717 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/commands/gcloud.py
+-rw-r--r--   0 julien     (501) staff       (20)     7185 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/commands/gcloud_pot.py
+-rw-r--r--   0 julien     (501) staff       (20)     5365 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/commands/gcloud_sql.py
+-rw-r--r--   0 julien     (501) staff       (20)     5006 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/commands/rds.py
+-rw-r--r--   0 julien     (501) staff       (20)     5961 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/commands/virtualbox.py
+-rw-r--r--   0 julien     (501) staff       (20)     5963 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/commands/vmware.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.941316 edb-deployment-3.9.3/edbdeploy/data/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.353519 edb-deployment-3.9.3/edbdeploy/data/ansible/
+-rw-r--r--   0 julien     (501) staff       (20)     1828 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-Always-On-Platinum.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1826 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-Always-On-Silver.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1612 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA-1.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1478 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA-2.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1720 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA-3.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1606 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA.yml
+-rw-r--r--   0 julien     (501) staff       (20)      943 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/HammerDB-DBaaS.yml
+-rw-r--r--   0 julien     (501) staff       (20)      937 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/HammerDB-TPROC-C.yml
+-rw-r--r--   0 julien     (501) staff       (20)     2016 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/POT-Remove-Project-Route53.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.932010 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.931868 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.359364 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/defaults/
+-rw-r--r--   0 julien     (501) staff       (20)      932 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/defaults/main.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.365697 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/handlers/
+-rw-r--r--   0 julien     (501) staff       (20)       33 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/handlers/main.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.474691 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/
+-rw-r--r--   0 julien     (501) staff       (20)      319 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/bdr_setup.yml
+-rw-r--r--   0 julien     (501) staff       (20)      791 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/main.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1916 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/os_configure_user.yml
+-rw-r--r--   0 julien     (501) staff       (20)     2275 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_certs.yml
+-rw-r--r--   0 julien     (501) staff       (20)     2761 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_probe_alert.yml
+-rw-r--r--   0 julien     (501) staff       (20)     2294 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_create_user.yml
+-rw-r--r--   0 julien     (501) staff       (20)      423 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_hba_rule.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1141 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_hba.yml
+-rw-r--r--   0 julien     (501) staff       (20)      999 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_scripts.yml
+-rw-r--r--   0 julien     (501) staff       (20)     2431 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_user_pgpass.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1805 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/update_route53.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1171 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/verify_variables.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.610432 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/
+-rwxr-xr-x   0 julien     (501) staff       (20)     3880 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/barman-backup-monitor.py.template
+-rw-r--r--   0 julien     (501) staff       (20)     2348 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/data_view.sql
+-rw-r--r--   0 julien     (501) staff       (20)     4480 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/harp-proxy-pgbouncer-monitor.sh.templates
+-rw-r--r--   0 julien     (501) staff       (20)    15076 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_bdr_probe.sql.template
+-rw-r--r--   0 julien     (501) staff       (20)     8925 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_charts.sql.template
+-rw-r--r--   0 julien     (501) staff       (20)     5877 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.platinum.template
+-rw-r--r--   0 julien     (501) staff       (20)     5174 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.silver.template
+-rw-r--r--   0 julien     (501) staff       (20)     4091 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_probe_alert.sql
+-rw-r--r--   0 julien     (501) staff       (20)      127 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pg_env_dbserver.sh.template
+-rw-r--r--   0 julien     (501) staff       (20)      118 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pg_env_pgbouncer.sh.template
+-rw-r--r--   0 julien     (501) staff       (20)      162 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pot_aliases.sh.template
+-rw-r--r--   0 julien     (501) staff       (20)      507 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/sudo_user.template
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.647222 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/
+-rw-r--r--   0 julien     (501) staff       (20)      537 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/EPAS.yml
+-rw-r--r--   0 julien     (501) staff       (20)      272 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/PG.yml
+-rw-r--r--   0 julien     (501) staff       (20)       34 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/main.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.932705 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.653556 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/defaults/
+-rw-r--r--   0 julien     (501) staff       (20)      857 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/defaults/main.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.659391 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/handlers/
+-rw-r--r--   0 julien     (501) staff       (20)       33 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/handlers/main.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.797179 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/
+-rw-r--r--   0 julien     (501) staff       (20)     1158 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/efm_scripts_rules.yml
+-rw-r--r--   0 julien     (501) staff       (20)      807 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/main.yml
+-rw-r--r--   0 julien     (501) staff       (20)      851 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/os_configure_user.yml
+-rw-r--r--   0 julien     (501) staff       (20)     2109 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pem_server_certs.yml
+-rw-r--r--   0 julien     (501) staff       (20)      398 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pem_server_probe_alert.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1692 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_create_user.yml
+-rw-r--r--   0 julien     (501) staff       (20)      450 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_hba_rule.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1148 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_pot_hba.yml
+-rw-r--r--   0 julien     (501) staff       (20)      343 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_pot_scripts.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1661 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_user_pgpass.yml
+-rw-r--r--   0 julien     (501) staff       (20)      415 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pot_setup.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1854 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/update_route53.yml
+-rw-r--r--   0 julien     (501) staff       (20)     1171 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/verify_variables.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.896528 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/
+-rwxr-xr-x   0 julien     (501) staff       (20)    17523 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.3.10.template
+-rw-r--r--   0 julien     (501) staff       (20)    17524 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.0.template
+-rwxr-xr-x   0 julien     (501) staff       (20)    18524 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.1.template
+-rw-r--r--   0 julien     (501) staff       (20)     2137 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_reconfigure_node.sh.template
+-rw-r--r--   0 julien     (501) staff       (20)     4006 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_rewind.sh.template
+-rw-r--r--   0 julien     (501) staff       (20)     1231 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_sudo.template
+-rw-r--r--   0 julien     (501) staff       (20)     1081 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/pem_probe_alert.sql
+-rw-r--r--   0 julien     (501) staff       (20)      126 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/pg_env_dbserver.sh.template
+-rw-r--r--   0 julien     (501) staff       (20)      265 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/pot_aliases.sh.template
+-rw-r--r--   0 julien     (501) staff       (20)      553 2021-08-02 14:19:30.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/sudo_user.template
+-rw-r--r--   0 julien     (501) staff       (20)      296 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/tuned.conf.template
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.914601 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/vars/
+-rw-r--r--   0 julien     (501) staff       (20)      556 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/vars/EPAS.yml
+-rw-r--r--   0 julien     (501) staff       (20)      272 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/vars/PG.yml
+-rw-r--r--   0 julien     (501) staff       (20)       29 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/vars/main.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.927583 edb-deployment-3.9.3/edbdeploy/data/templates/
+-rw-r--r--   0 julien     (501) staff       (20)     4830 2022-01-28 10:17:08.000000 edb-deployment-3.9.3/edbdeploy/data/templates/config.yml.j2
+-rw-r--r--   0 julien     (501) staff       (20)     6339 2022-01-26 12:28:03.000000 edb-deployment-3.9.3/edbdeploy/data/templates/inventory.yml.j2
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.939745 edb-deployment-3.9.3/edbdeploy/data/terraform/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:26.969603 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.936842 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.323505 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/ec2/
+-rw-r--r--   0 julien     (501) staff       (20)    17311 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/ec2/ec2.tf
+-rw-r--r--   0 julien     (501) staff       (20)     4191 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/ec2/outputs.tf
+-rwxr-xr-x   0 julien     (501) staff       (20)      416 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/ec2/setup_volume.sh
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.347312 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/network/
+-rw-r--r--   0 julien     (501) staff       (20)      791 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/network/network.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.354055 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/policies/
+-rw-r--r--   0 julien     (501) staff       (20)      836 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/policies/policy.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.361509 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/routes/
+-rw-r--r--   0 julien     (501) staff       (20)     1519 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/routes/routes.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.375892 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/security/
+-rw-r--r--   0 julien     (501) staff       (20)       85 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/security/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)     3373 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/security/security.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.403671 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/vpc/
+-rw-r--r--   0 julien     (501) staff       (20)       46 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/vpc/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)      248 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/vpc/vpc.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.937157 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/global/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.415382 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/global/iam/
+-rw-r--r--   0 julien     (501) staff       (20)      358 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/global/iam/iam.tf
+-rw-r--r--   0 julien     (501) staff       (20)      125 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/global/iam/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)     3019 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/main.tf
+-rw-r--r--   0 julien     (501) staff       (20)       45 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/provider.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1462 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/tags.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)     1357 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws/variables.tf.template
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.010067 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.935738 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.176530 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/aws/
+-rw-r--r--   0 julien     (501) staff       (20)     7132 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/aws/aws.tf
+-rw-r--r--   0 julien     (501) staff       (20)     2210 2021-12-17 09:43:12.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/aws/outputs.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.197807 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/network/
+-rw-r--r--   0 julien     (501) staff       (20)      791 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/network/network.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.203992 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/policies/
+-rw-r--r--   0 julien     (501) staff       (20)      836 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/policies/policy.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.210917 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/routes/
+-rw-r--r--   0 julien     (501) staff       (20)     1208 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/routes/routes.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.225713 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/security/
+-rw-r--r--   0 julien     (501) staff       (20)      161 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/security/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1855 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/security/security.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.256870 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/vpc/
+-rw-r--r--   0 julien     (501) staff       (20)       46 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/vpc/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)      248 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/vpc/vpc.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.935974 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/global/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.277286 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/global/iam/
+-rw-r--r--   0 julien     (501) staff       (20)      358 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/global/iam/iam.tf
+-rw-r--r--   0 julien     (501) staff       (20)      125 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/global/iam/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)     2506 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/main.tf
+-rw-r--r--   0 julien     (501) staff       (20)       45 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/provider.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1462 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/tags.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)     1258 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/variables.tf.template
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.053701 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.934486 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.066747 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/
+-rw-r--r--   0 julien     (501) staff       (20)     5944 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/aws.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1979 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/outputs.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.074915 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/network/
+-rw-r--r--   0 julien     (501) staff       (20)      791 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/network/network.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.097558 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/policies/
+-rw-r--r--   0 julien     (501) staff       (20)      836 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/policies/policy.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.104088 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/routes/
+-rw-r--r--   0 julien     (501) staff       (20)     1208 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/routes/routes.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.117134 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/security/
+-rw-r--r--   0 julien     (501) staff       (20)      161 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/security/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1855 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/security/security.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.147726 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/vpc/
+-rw-r--r--   0 julien     (501) staff       (20)       46 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/vpc/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)      248 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/vpc/vpc.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.934746 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/global/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.159472 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/global/iam/
+-rw-r--r--   0 julien     (501) staff       (20)      358 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/global/iam/iam.tf
+-rw-r--r--   0 julien     (501) staff       (20)      125 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/global/iam/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)     2407 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/main.tf
+-rw-r--r--   0 julien     (501) staff       (20)       45 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/provider.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1462 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/tags.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)     1155 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/variables.tf.template
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.461490 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.939493 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.596952 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/network/
+-rw-r--r--   0 julien     (501) staff       (20)      367 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/network/network.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.604376 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/resourcegroup/
+-rw-r--r--   0 julien     (501) staff       (20)      264 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/resourcegroup/rg.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.611586 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/security/
+-rw-r--r--   0 julien     (501) staff       (20)     5984 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/security/security.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.619435 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/storageaccount/
+-rw-r--r--   0 julien     (501) staff       (20)      500 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/storageaccount/storageaccount.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.626371 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/storagecontainer/
+-rw-r--r--   0 julien     (501) staff       (20)      333 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/storagecontainer/storagecontainer.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.667864 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm/
+-rw-r--r--   0 julien     (501) staff       (20)     4133 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm/outputs.tf
+-rwxr-xr-x   0 julien     (501) staff       (20)      416 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm/setup_volume.sh
+-rw-r--r--   0 julien     (501) staff       (20)    24134 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm/vm.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.707729 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm-hammerdb/
+-rw-r--r--   0 julien     (501) staff       (20)     2014 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm-hammerdb/outputs.tf
+-rwxr-xr-x   0 julien     (501) staff       (20)      349 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm-hammerdb/setup_volume.sh
+-rw-r--r--   0 julien     (501) staff       (20)    15922 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm-hammerdb/vm-hammerdb.tf
+-rw-r--r--   0 julien     (501) staff       (20)     4602 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/main.tf
+-rw-r--r--   0 julien     (501) staff       (20)      161 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/provider.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1181 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/tags.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)      965 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure/variables.tf.template
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.509839 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.938357 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.515663 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/network/
+-rw-r--r--   0 julien     (501) staff       (20)      367 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/network/network.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.522225 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/resourcegroup/
+-rw-r--r--   0 julien     (501) staff       (20)      264 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/resourcegroup/rg.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.529408 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/security/
+-rw-r--r--   0 julien     (501) staff       (20)     2611 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/security/security.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.548448 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/storageaccount/
+-rw-r--r--   0 julien     (501) staff       (20)      500 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/storageaccount/storageaccount.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.554815 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/storagecontainer/
+-rw-r--r--   0 julien     (501) staff       (20)      286 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/storagecontainer/storagecontainer.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.572786 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/vm/
+-rw-r--r--   0 julien     (501) staff       (20)     3681 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/vm/outputs.tf
+-rw-r--r--   0 julien     (501) staff       (20)    12813 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/vm/vm.tf
+-rw-r--r--   0 julien     (501) staff       (20)     2371 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/main.tf
+-rw-r--r--   0 julien     (501) staff       (20)       58 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/provider.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1181 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/tags.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)      862 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/variables.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)      129 2022-01-26 12:28:03.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/versions.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.760507 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.940753 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.874663 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/compute/
+-rw-r--r--   0 julien     (501) staff       (20)    20023 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/compute/compute.tf
+-rw-r--r--   0 julien     (501) staff       (20)     4250 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/compute/outputs.tf
+-rwxr-xr-x   0 julien     (501) staff       (20)      416 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/compute/setup_volume.sh
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.897462 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/network/
+-rw-r--r--   0 julien     (501) staff       (20)      489 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/network/network.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.905238 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/security/
+-rw-r--r--   0 julien     (501) staff       (20)     6580 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/security/firewall.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1813 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/main.tf
+-rw-r--r--   0 julien     (501) staff       (20)       99 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/provider.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1183 2021-11-22 13:27:33.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/tags.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)     1230 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/variables.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)      127 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/versions.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.803481 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.940177 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.818946 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/compute/
+-rw-r--r--   0 julien     (501) staff       (20)    11483 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/compute/compute.tf
+-rw-r--r--   0 julien     (501) staff       (20)     2928 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/compute/outputs.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.826056 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/network/
+-rw-r--r--   0 julien     (501) staff       (20)      489 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/network/network.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.848022 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/security/
+-rw-r--r--   0 julien     (501) staff       (20)     2899 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/security/firewall.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1397 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/main.tf
+-rw-r--r--   0 julien     (501) staff       (20)       99 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/provider.tf
+-rw-r--r--   0 julien     (501) staff       (20)     1104 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/variables.tf.template
+-rw-r--r--   0 julien     (501) staff       (20)      127 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/versions.tf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:25.940961 edb-deployment-3.9.3/edbdeploy/data/tpaexec/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.912423 edb-deployment-3.9.3/edbdeploy/data/tpaexec/hooks/
+-rw-r--r--   0 julien     (501) staff       (20)     4516 2022-01-28 14:40:29.000000 edb-deployment-3.9.3/edbdeploy/data/tpaexec/hooks/post-deploy.yml
+-rw-r--r--   0 julien     (501) staff       (20)      398 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/data/tpaexec/hooks/pre-initdb.yml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.923963 edb-deployment-3.9.3/edbdeploy/data/tpaexec/hooks/templates/
+-rw-r--r--   0 julien     (501) staff       (20)       62 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/tpaexec/hooks/templates/harp-manager.override.conf
+-rw-r--r--   0 julien     (501) staff       (20)       62 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/data/tpaexec/hooks/templates/harp-proxy.override.conf
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.959410 edb-deployment-3.9.3/edbdeploy/data/virtualbox/
+-rwxr-xr-x   0 julien     (501) staff       (20)     2018 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/virtualbox/c8-EDB-RA-1
+-rwxr-xr-x   0 julien     (501) staff       (20)     2434 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/virtualbox/c8-EDB-RA-2
+-rwxr-xr-x   0 julien     (501) staff       (20)     2818 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/data/virtualbox/c8-EDB-RA-3
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:27.997751 edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/
+-rwxr-xr-x   0 julien     (501) staff       (20)     1040 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/c8-EDB-RA-1
+-rwxr-xr-x   0 julien     (501) staff       (20)     1738 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/c8-EDB-RA-2
+-rwxr-xr-x   0 julien     (501) staff       (20)     2779 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/c8-EDB-RA-3
+-rwxr-xr-x   0 julien     (501) staff       (20)     1349 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/playbook.yml
+-rw-r--r--   0 julien     (501) staff       (20)      397 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/errors.py
+-rw-r--r--   0 julien     (501) staff       (20)     1990 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/installation.py
+-rw-r--r--   0 julien     (501) staff       (20)    10018 2022-01-26 12:28:03.000000 edb-deployment-3.9.3/edbdeploy/options.py
+-rw-r--r--   0 julien     (501) staff       (20)     1612 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/password.py
+-rw-r--r--   0 julien     (501) staff       (20)    63378 2022-01-26 12:28:03.000000 edb-deployment-3.9.3/edbdeploy/project.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:28.148033 edb-deployment-3.9.3/edbdeploy/projects/
+-rw-r--r--   0 julien     (501) staff       (20)        0 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/projects/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     4342 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/projects/aws.py
+-rw-r--r--   0 julien     (501) staff       (20)     8362 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/projects/aws_pot.py
+-rw-r--r--   0 julien     (501) staff       (20)     5101 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/projects/aws_rds.py
+-rw-r--r--   0 julien     (501) staff       (20)     1121 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/projects/aws_rds_aurora.py
+-rw-r--r--   0 julien     (501) staff       (20)     3907 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/projects/azure.py
+-rw-r--r--   0 julien     (501) staff       (20)     4240 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/projects/azure_db.py
+-rw-r--r--   0 julien     (501) staff       (20)     7934 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/projects/azure_pot.py
+-rw-r--r--   0 julien     (501) staff       (20)     2985 2021-11-17 15:19:50.000000 edb-deployment-3.9.3/edbdeploy/projects/baremetal.py
+-rw-r--r--   0 julien     (501) staff       (20)     4416 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/projects/gcloud.py
+-rw-r--r--   0 julien     (501) staff       (20)     8099 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/edbdeploy/projects/gcloud_pot.py
+-rw-r--r--   0 julien     (501) staff       (20)     2535 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/projects/gcloud_sql.py
+-rw-r--r--   0 julien     (501) staff       (20)    19772 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/projects/virtualbox.py
+-rw-r--r--   0 julien     (501) staff       (20)    18871 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/projects/vmware.py
+-rw-r--r--   0 julien     (501) staff       (20)     1385 2022-01-25 14:49:09.000000 edb-deployment-3.9.3/edbdeploy/render.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2022-01-28 14:54:28.262215 edb-deployment-3.9.3/edbdeploy/spec/
+-rw-r--r--   0 julien     (501) staff       (20)    14424 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     7419 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/aws.py
+-rw-r--r--   0 julien     (501) staff       (20)     1472 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/aws_rds.py
+-rw-r--r--   0 julien     (501) staff       (20)      423 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/aws_rds_aurora.py
+-rw-r--r--   0 julien     (501) staff       (20)     5358 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/azure.py
+-rw-r--r--   0 julien     (501) staff       (20)     1204 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/azure_db.py
+-rw-r--r--   0 julien     (501) staff       (20)     4559 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/spec/baremetal.py
+-rw-r--r--   0 julien     (501) staff       (20)     5586 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/gcloud.py
+-rw-r--r--   0 julien     (501) staff       (20)     1346 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/gcloud_sql.py
+-rw-r--r--   0 julien     (501) staff       (20)     4506 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/spec/reference_architecture.py
+-rw-r--r--   0 julien     (501) staff       (20)     2196 2021-11-02 13:36:41.000000 edb-deployment-3.9.3/edbdeploy/spec/virtualbox.py
+-rw-r--r--   0 julien     (501) staff       (20)     4591 2021-12-21 12:52:56.000000 edb-deployment-3.9.3/edbdeploy/spec/vmware.py
+-rw-r--r--   0 julien     (501) staff       (20)     5081 2021-10-25 08:14:11.000000 edb-deployment-3.9.3/edbdeploy/specifications.py
+-rw-r--r--   0 julien     (501) staff       (20)      888 2021-09-14 06:41:50.000000 edb-deployment-3.9.3/edbdeploy/system.py
+-rw-r--r--   0 julien     (501) staff       (20)     8390 2021-09-13 15:20:44.000000 edb-deployment-3.9.3/edbdeploy/terraform.py
+-rw-r--r--   0 julien     (501) staff       (20)     6423 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/tpaexec.py
+-rw-r--r--   0 julien     (501) staff       (20)    10883 2021-08-30 12:22:34.000000 edb-deployment-3.9.3/edbdeploy/virtualbox.py
+-rw-r--r--   0 julien     (501) staff       (20)    12570 2021-07-29 08:12:40.000000 edb-deployment-3.9.3/edbdeploy/vmware.py
+-rw-r--r--   0 julien     (501) staff       (20)       38 2022-01-28 14:54:28.264003 edb-deployment-3.9.3/setup.cfg
+-rw-r--r--   0 julien     (501) staff       (20)     2535 2022-01-25 08:38:31.000000 edb-deployment-3.9.3/setup.py
```

### Comparing `edb-deployment-3.9.2/LICENSE.md` & `edb-deployment-3.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/PKG-INFO` & `edb-deployment-3.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edb-deployment
-Version: 3.9.2
+Version: 3.9.3
 Summary:  Postgres Deployment Scripts are an easy way to deploy PostgreSQL, EDB Postgres Advanced Server, and EDB Tools in the Cloud. 
 Home-page: https://github.com/EnterpriseDB/postgres-deployment/
 Author: EDB
 Author-email: edb-devops@enterprisedb.com
 License: BSD
 Keywords: postgresql edb epas cli deploy cloud aws rds aurora azure gcloud vmware
 Platform: UNKNOWN
```

### Comparing `edb-deployment-3.9.2/README.md` & `edb-deployment-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edb_deployment.egg-info/PKG-INFO` & `edb-deployment-3.9.3/edb_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edb-deployment
-Version: 3.9.2
+Version: 3.9.3
 Summary:  Postgres Deployment Scripts are an easy way to deploy PostgreSQL, EDB Postgres Advanced Server, and EDB Tools in the Cloud. 
 Home-page: https://github.com/EnterpriseDB/postgres-deployment/
 Author: EDB
 Author-email: edb-devops@enterprisedb.com
 License: BSD
 Keywords: postgresql edb epas cli deploy cloud aws rds aurora azure gcloud vmware
 Platform: UNKNOWN
```

### Comparing `edb-deployment-3.9.2/edb_deployment.egg-info/SOURCES.txt` & `edb-deployment-3.9.3/edb_deployment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/__init__.py` & `edb-deployment-3.9.3/edbdeploy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.9.2"
+__version__ = "3.9.3"
 # Version number of the Ansible collection we want to use
 __edb_ansible_version__ = "3.8.0"
 
 def to_num(version):
     """
     Convert version number from 3 digits tuple to 1 integer.
     (1, 2, 3) -> 100020003
```

### Comparing `edb-deployment-3.9.2/edbdeploy/action.py` & `edb-deployment-3.9.3/edbdeploy/action.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/ansible.py` & `edb-deployment-3.9.3/edbdeploy/ansible.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/cli.py` & `edb-deployment-3.9.3/edbdeploy/cli.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/cloud.py` & `edb-deployment-3.9.3/edbdeploy/cloud.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/command.py` & `edb-deployment-3.9.3/edbdeploy/command.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/aurora.py` & `edb-deployment-3.9.3/edbdeploy/commands/aurora.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/aws.py` & `edb-deployment-3.9.3/edbdeploy/commands/aws.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/aws_pot.py` & `edb-deployment-3.9.3/edbdeploy/commands/aws_pot.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/azure.py` & `edb-deployment-3.9.3/edbdeploy/commands/azure.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/azure_db.py` & `edb-deployment-3.9.3/edbdeploy/commands/azure_db.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/azure_pot.py` & `edb-deployment-3.9.3/edbdeploy/commands/azure_pot.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/baremetal.py` & `edb-deployment-3.9.3/edbdeploy/commands/baremetal.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/default.py` & `edb-deployment-3.9.3/edbdeploy/commands/default.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/gcloud.py` & `edb-deployment-3.9.3/edbdeploy/commands/gcloud.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/gcloud_pot.py` & `edb-deployment-3.9.3/edbdeploy/commands/gcloud_pot.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/gcloud_sql.py` & `edb-deployment-3.9.3/edbdeploy/commands/gcloud_sql.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/rds.py` & `edb-deployment-3.9.3/edbdeploy/commands/rds.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/virtualbox.py` & `edb-deployment-3.9.3/edbdeploy/commands/virtualbox.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/commands/vmware.py` & `edb-deployment-3.9.3/edbdeploy/commands/vmware.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-Always-On-Platinum.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-Always-On-Platinum.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-Always-On-Silver.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-Always-On-Silver.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA-1.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA-1.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA-2.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA-2.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA-3.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA-3.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/EDB-RA.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/EDB-RA.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/HammerDB-DBaaS.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/HammerDB-DBaaS.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/HammerDB-TPROC-C.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/HammerDB-TPROC-C.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/POT-Remove-Project-Route53.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/POT-Remove-Project-Route53.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/defaults/main.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/main.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/os_configure_user.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/os_configure_user.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_certs.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_certs.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_probe_alert.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pem_server_probe_alert.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_create_user.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_create_user.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_hba.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_hba.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_scripts.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_pot_scripts.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_user_pgpass.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/pg_user_pgpass.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/update_route53.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/update_route53.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/verify_variables.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/tasks/verify_variables.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/barman-backup-monitor.py.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/barman-backup-monitor.py.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/data_view.sql` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/data_view.sql`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/harp-proxy-pgbouncer-monitor.sh.templates` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/harp-proxy-pgbouncer-monitor.sh.templates`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_bdr_probe.sql.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_bdr_probe.sql.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_charts.sql.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_charts.sql.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.platinum.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.platinum.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.silver.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_dashboards.sql.silver.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_probe_alert.sql` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/templates/pem_probe_alert.sql`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/EPAS.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/bdr_pot_setup/vars/EPAS.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/defaults/main.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/efm_scripts_rules.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/efm_scripts_rules.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/main.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/os_configure_user.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/os_configure_user.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pem_server_certs.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pem_server_certs.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_create_user.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_create_user.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_pot_hba.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_pot_hba.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_user_pgpass.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/pg_user_pgpass.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/update_route53.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/update_route53.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/tasks/verify_variables.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/tasks/verify_variables.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.3.10.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.3.10.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.0.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.0.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.1.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_db_functions.4.1.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_reconfigure_node.sh.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_reconfigure_node.sh.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_rewind.sh.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_rewind.sh.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/efm_sudo.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/efm_sudo.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/pem_probe_alert.sql` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/pem_probe_alert.sql`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/templates/sudo_user.template` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/templates/sudo_user.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/ansible/roles/pot_setup/vars/EPAS.yml` & `edb-deployment-3.9.3/edbdeploy/data/ansible/roles/pot_setup/vars/EPAS.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/templates/config.yml.j2` & `edb-deployment-3.9.3/edbdeploy/data/templates/config.yml.j2`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 cluster_tags: {}
 
 cluster_vars:
   bdr_database: edb
   bdr_node_group: bdrgroup
   bdr_version: '4'
   failover_manager: harp
+  harp_request_timeout: '250ms'
+  harp_watch_poll_interval: '500ms'
   harp_consensus_protocol: etcd
   postgres_data_dir: /pgdata/pg_data
   postgres_wal_dir: /pgwal/pg_wal
   postgres_coredump_filter: '0xff'
   postgres_version: '14'
   postgresql_flavour: epas
   postgres_user: enterprisedb
@@ -129,15 +131,15 @@
     - database: edb
       type: bdr
       replication_sets:
       - bdrgroup
 {% endfor %}
 {% for pooler_server in servers['pooler_server'] %}
 - Name: pgbouncer{{ pooler_server['id'] }}
-{%   if pooler_server['id'] < 4 %}
+{%   if pooler_server['id'] < 3 %}
   location: BDRDC1
 {%   else %}
   location: BDRDC2
 {%   endif %}
   node: {{ servers.get('bdr_server', []) | length + servers.get('bdr_witness_server', []) | length + pooler_server['id'] }}
   public_ip:  {{ pooler_server['public_ip'] }}
   private_ip: {{ pooler_server['private_ip'] }}
```

### Comparing `edb-deployment-3.9.2/edbdeploy/data/templates/inventory.yml.j2` & `edb-deployment-3.9.3/edbdeploy/data/templates/inventory.yml.j2`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/ec2/ec2.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/ec2/ec2.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/ec2/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/ec2/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/network/network.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/network/network.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/policies/policy.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/policies/policy.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/routes/routes.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/routes/routes.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/environments/security/security.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/environments/security/security.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/main.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/main.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/tags.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/tags.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws/variables.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws/variables.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/aws/aws.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/aws/aws.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/aws/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/network/network.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/network/network.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/policies/policy.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/policies/policy.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/routes/routes.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/routes/routes.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/environments/security/security.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/environments/security/security.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/main.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/main.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/tags.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/tags.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds/variables.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds/variables.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/aws.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/aws.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/network/network.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/network/network.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/policies/policy.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/policies/policy.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/routes/routes.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/routes/routes.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/environments/security/security.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/environments/security/security.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/main.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/main.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/tags.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/tags.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/aws-rds-aurora/variables.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/aws-rds-aurora/variables.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/security/security.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/security/security.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm/vm.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm/vm.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm-hammerdb/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm-hammerdb/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/environments/vm-hammerdb/vm-hammerdb.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/environments/vm-hammerdb/vm-hammerdb.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/main.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/main.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/tags.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/tags.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure/variables.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure/variables.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/security/security.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/security/security.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/vm/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/vm/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/environments/vm/vm.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/environments/vm/vm.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/main.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/main.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/tags.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/tags.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/azure-db/variables.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/azure-db/variables.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/compute/compute.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/compute/compute.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/compute/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/compute/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/environments/security/firewall.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/environments/security/firewall.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/main.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/main.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/tags.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/tags.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud/variables.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud/variables.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/compute/compute.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/compute/compute.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/compute/outputs.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/compute/outputs.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/environments/security/firewall.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/environments/security/firewall.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/main.tf` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/main.tf`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/terraform/gcloud-sql/variables.tf.template` & `edb-deployment-3.9.3/edbdeploy/data/terraform/gcloud-sql/variables.tf.template`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/virtualbox/c8-EDB-RA-1` & `edb-deployment-3.9.3/edbdeploy/data/virtualbox/c8-EDB-RA-1`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/virtualbox/c8-EDB-RA-2` & `edb-deployment-3.9.3/edbdeploy/data/virtualbox/c8-EDB-RA-2`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/virtualbox/c8-EDB-RA-3` & `edb-deployment-3.9.3/edbdeploy/data/virtualbox/c8-EDB-RA-3`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/c8-EDB-RA-1` & `edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/c8-EDB-RA-1`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/c8-EDB-RA-2` & `edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/c8-EDB-RA-2`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/c8-EDB-RA-3` & `edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/c8-EDB-RA-3`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/data/vmware-wkstn/playbook.yml` & `edb-deployment-3.9.3/edbdeploy/data/vmware-wkstn/playbook.yml`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/installation.py` & `edb-deployment-3.9.3/edbdeploy/installation.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/options.py` & `edb-deployment-3.9.3/edbdeploy/options.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/password.py` & `edb-deployment-3.9.3/edbdeploy/password.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/project.py` & `edb-deployment-3.9.3/edbdeploy/project.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/aws.py` & `edb-deployment-3.9.3/edbdeploy/projects/aws.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/aws_pot.py` & `edb-deployment-3.9.3/edbdeploy/projects/aws_pot.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/aws_rds.py` & `edb-deployment-3.9.3/edbdeploy/projects/aws_rds.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/aws_rds_aurora.py` & `edb-deployment-3.9.3/edbdeploy/projects/aws_rds_aurora.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/azure.py` & `edb-deployment-3.9.3/edbdeploy/projects/azure.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/azure_db.py` & `edb-deployment-3.9.3/edbdeploy/projects/azure_db.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/azure_pot.py` & `edb-deployment-3.9.3/edbdeploy/projects/azure_pot.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/baremetal.py` & `edb-deployment-3.9.3/edbdeploy/projects/baremetal.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/gcloud.py` & `edb-deployment-3.9.3/edbdeploy/projects/gcloud.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/gcloud_pot.py` & `edb-deployment-3.9.3/edbdeploy/projects/gcloud_pot.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/gcloud_sql.py` & `edb-deployment-3.9.3/edbdeploy/projects/gcloud_sql.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/virtualbox.py` & `edb-deployment-3.9.3/edbdeploy/projects/virtualbox.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/projects/vmware.py` & `edb-deployment-3.9.3/edbdeploy/projects/vmware.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/render.py` & `edb-deployment-3.9.3/edbdeploy/render.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/__init__.py` & `edb-deployment-3.9.3/edbdeploy/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/aws.py` & `edb-deployment-3.9.3/edbdeploy/spec/aws.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/aws_rds.py` & `edb-deployment-3.9.3/edbdeploy/spec/aws_rds.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/azure.py` & `edb-deployment-3.9.3/edbdeploy/spec/azure.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/azure_db.py` & `edb-deployment-3.9.3/edbdeploy/spec/azure_db.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/baremetal.py` & `edb-deployment-3.9.3/edbdeploy/spec/baremetal.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/gcloud.py` & `edb-deployment-3.9.3/edbdeploy/spec/gcloud.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/gcloud_sql.py` & `edb-deployment-3.9.3/edbdeploy/spec/gcloud_sql.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/reference_architecture.py` & `edb-deployment-3.9.3/edbdeploy/spec/reference_architecture.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/virtualbox.py` & `edb-deployment-3.9.3/edbdeploy/spec/virtualbox.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/spec/vmware.py` & `edb-deployment-3.9.3/edbdeploy/spec/vmware.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/specifications.py` & `edb-deployment-3.9.3/edbdeploy/specifications.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/system.py` & `edb-deployment-3.9.3/edbdeploy/system.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/terraform.py` & `edb-deployment-3.9.3/edbdeploy/terraform.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/tpaexec.py` & `edb-deployment-3.9.3/edbdeploy/tpaexec.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/virtualbox.py` & `edb-deployment-3.9.3/edbdeploy/virtualbox.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/edbdeploy/vmware.py` & `edb-deployment-3.9.3/edbdeploy/vmware.py`

 * *Files identical despite different names*

### Comparing `edb-deployment-3.9.2/setup.py` & `edb-deployment-3.9.3/setup.py`

 * *Files identical despite different names*

