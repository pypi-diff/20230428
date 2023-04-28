# Comparing `tmp/nec_sol-0.5.1.post1-py3-none-any.whl.zip` & `tmp/nec_sol-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 7824 bytes, number of entries: 7
--rw-r--r--  2.0 unx    17008 b- defN 22-Nov-04 08:11 nec-sol/__main__.py
--rw-r--r--  2.0 unx     3942 b- defN 22-Oct-17 09:38 nec-sol/config.json
--rwxrwxrwx  2.0 unx      229 b- defN 22-Oct-17 09:12 nec_sol-0.5.1.post1.data/scripts/nec-sol
-?rw-------  2.0 unx      907 b- defN 22-Nov-04 08:12 nec_sol-0.5.1.post1.dist-info/METADATA
-?rw-------  2.0 unx        7 b- defN 22-Nov-04 08:12 nec_sol-0.5.1.post1.dist-info/top_list.txt
-?rw-------  2.0 unx       87 b- defN 22-Nov-04 08:12 nec_sol-0.5.1.post1.dist-info/WHEEL
-?rw-------  2.0 unx      582 b- defN 22-Nov-04 08:12 nec_sol-0.5.1.post1.dist-info/RECORD
-7 files, 22762 bytes uncompressed, 6812 bytes compressed:  70.1%
+Zip file size: 6771 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    16382 b- defN 23-Apr-28 12:56 nec-sol/__main__.py
+-rwxrwxrwx  2.0 unx      229 b- defN 23-Mar-23 09:11 nec_sol-0.5.2.data/scripts/nec-sol
+-rw-------  2.0 unx      964 b- defN 23-Apr-28 13:07 nec_sol-0.5.2.dist-info/METADATA
+-rw-------  2.0 unx       87 b- defN 23-Apr-28 13:07 nec_sol-0.5.2.dist-info/WHEEL
+-rw-------  2.0 unx        7 b- defN 23-Apr-28 13:07 nec_sol-0.5.2.dist-info/top_list.txt
+-rw-------  2.0 unx      474 b- defN 23-Apr-28 13:07 nec_sol-0.5.2.dist-info/RECORD
+6 files, 18143 bytes uncompressed, 5933 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
 Filename: nec-sol/__main__.py
 Comment: 
 
-Filename: nec-sol/config.json
+Filename: nec_sol-0.5.2.data/scripts/nec-sol
 Comment: 
 
-Filename: nec_sol-0.5.1.post1.data/scripts/nec-sol
+Filename: nec_sol-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: nec_sol-0.5.1.post1.dist-info/METADATA
+Filename: nec_sol-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: nec_sol-0.5.1.post1.dist-info/top_list.txt
+Filename: nec_sol-0.5.2.dist-info/top_list.txt
 Comment: 
 
-Filename: nec_sol-0.5.1.post1.dist-info/WHEEL
-Comment: 
-
-Filename: nec_sol-0.5.1.post1.dist-info/RECORD
+Filename: nec_sol-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nec-sol/__main__.py

```diff
@@ -1,50 +1,48 @@
-from collections import OrderedDict
-from simple_term_menu import TerminalMenu
 import getpass
 import platform
 import re
 import requests
 import subprocess
 import sys
 import urllib.parse
-import json
 import os
 import traceback
 import argparse
-from typing import Union, List, Tuple, Optional, Dict, Set, Any
+from typing import Union, List, Tuple
+from termcolor import colored
+from simple_term_menu import TerminalMenu
 
 #-------------------------------------------------------------------------------
-class Plugin:
-	def __init__(self, name: str, version: str, url: Optional[str] = None, dependencies: Optional[List[str]] = []):
-		if not(version is None or version.startswith(('<=', '>=', '==', '~='))):
-			raise Exception(f'invalid version detected: {version}')
-
-		self.name			= name
-		self.version		= version
-		self.url			= url
-		self.dependencies	= dependencies
-		
-	def __repr__(self):
-		return f'[Plugin name={self.name}, version={self.version}, url={self.url}, dependencies={self.dependencies}]'
+s_version = "0.5.2"
+s_license_version = "1.0"
+s_prefix = "nec"
+s_default_versions = {
+	"torch": "~=2.0.0",
+	"tensorflow": "~=2.12.0"
+}
+s_urls = [
+	'https://{USERNAME}:{PASSWORD}@sol.neclab.eu/core/',
+	'https://{USERNAME}:{PASSWORD}@sol.neclab.eu/license/',
+	'https://{USERNAME}:{PASSWORD}@sol.neclab.eu/x86/',
+	'https://{USERNAME}:{PASSWORD}@sol.neclab.eu/ve/',
+	'https://{USERNAME}:{PASSWORD}@sol.neclab.eu/nvidia/',
+	'https://{USERNAME}:{PASSWORD}@sol.neclab.eu/dev/',
+]
+s_available_frameworks	= ['torch', 'tensorflow', 'numpy', 'onnx']
+
+#-------------------------------------------------------------------------------
+emph	= lambda x: colored(x,				attrs=['bold'])
+red		= lambda x: colored(x, 'red', 		attrs=['bold'])
+green	= lambda x: colored(x, 'green',		attrs=['bold'])
+yellow	= lambda x: colored(x, 'yellow',	attrs=['bold'])
 
-L_EMPH  	= "\033[1m"
-L_ERROR		= "\033[0;31m"
-L_SUCCESS	= "\033[0;32m"
-L_RESET 	= "\033[0m"
-
-s_access			= None
-s_available			= None
 s_installed			= None
-s_prefix			= None
-s_license_version	= None
-s_version			= None
 s_dependencies		= None
 s_python_packages	= None
-s_default_versions	= None
 
 #-------------------------------------------------------------------------------
 # taken from: https://stackoverflow.com/questions/1871549/determine-if-python-is-running-inside-virtualenv
 def is_virtualenv():
 	return (hasattr(sys, 'real_prefix') or (hasattr(sys, 'base_prefix') and sys.base_prefix != sys.prefix))
 
 #-------------------------------------------------------------------------------
@@ -58,112 +56,104 @@
 	ret = subprocess.run(cmd, stdout=subprocess.PIPE)
 	if ret.returncode != 0:
 		raise Exception("PIP error detected")
 	return ret.stdout.decode('utf-8')
 
 #-------------------------------------------------------------------------------
 def initialize():
-	global s_prefix, s_version, s_license_version, s_available, s_access, s_python_packages, s_installed, s_dependencies
-
-	# Open Config File ---------------------------------------------------------
-	with open(os.path.join(os.path.dirname(__file__), 'config.json'), 'r') as f:
-		data = json.load(f)
-		assert isinstance(data, dict)
-		s_prefix			= data.get('prefix')
-		s_version			= data.get('version')
-		s_license_version	= data.get('license_version')
-		s_default_versions	= data.get('default_versions')
-		s_available			= list()
-		s_access			= set()
-		for plugin in data.get('plugins'):
-			p = Plugin(*plugin)
-			s_available.append(p)
-			if p.url: # None == PyPI
-				s_access.add(p.url)
+	global s_prefix, s_version, s_license_version, s_python_packages, s_installed, s_dependencies
 
 	# Init Available Modules ---------------------------------------------------
 	output				= run_output(['python3', '-m', 'pip', 'list', 'installed'])
 	s_python_packages	= output.split('\n')[2:]
 	s_installed			= dict()
 	prog				= re.compile(r'^({}-sol[a-z0-9-]+)\s+([0-9\.a-z]+)'.format(s_prefix))
 	for x in s_python_packages:
 		match = prog.match(x)
 		if match:
 			s_installed[match[1]] = match[2]
 
-	# Init Available Hardware --------------------------------------------------
+	# Init Dependencies --------------------------------------------------------
 	s_dependencies = dict()
 
+	# Init Features ------------------------------------------------------------
+	if args.features == ['all']:
+		s_dependencies['sdk']	= s_version
+		s_dependencies['tests']	= s_version
+	else:
+		for f in args.features:
+			if f in ['sdk', 'tests']:	s_dependencies[f] = s_version
+			else:						raise Exception(f'Unknown feature: {f}')
+
+	# Init Available Hardware --------------------------------------------------
 	if args.devices == ['all']:
-		def add_device(name, func, force=False):
+		def add_device(name, func):
 			global s_dependencies
 			s_dependencies[name] = None
 	else:
-		def add_device(name, func, force=False):
+		def add_device(name, func):
 			global s_dependencies
-
 			try:
-				if func() if force or len(args.devices) == 0 else args.devices.index(name) >= 0:
+				if func() if len(args.devices) == 0 else args.devices.index(name) >= 0:
 					s_dependencies[name] = None
 			except ValueError:
 				pass
 
-	add_device('x86_64',	lambda: platform.machine() == 'x86_64', True)
+	add_device('x86',		lambda: platform.machine() == 'x86_64')
 	add_device('ve',		lambda: os.path.exists('/sys/class/ve'))
 	add_device('nvidia',	lambda: os.path.exists('/proc/driver/nvidia/version'))
 
 	dev_cnt = len(s_dependencies)
 	if dev_cnt == 0:
 		raise Exception('No devices detected or selected via --devices!')
 		
 	# Init Available Frameworks ------------------------------------------------
-	available_frameworks = ['torch', 'tensorflow', 'numpy', 'onnx']
 	if len(args.frameworks) == 0: # auto
-		args.frameworks = available_frameworks
+		args.frameworks = s_available_frameworks
 	else:
 		if args.frameworks == ['all']:
-			args.frameworks = available_frameworks
+			args.frameworks = s_available_frameworks
 
 		regex = re.compile(r'([a-zA-Z0-9\-]+)\s*(==|<=|>=|~=)?\s*([0-9\.]+(\.post[0-9]+)?)?')
 
 		for d in args.frameworks:
 			match = regex.search(d)
 
 			if match is None:
 				raise Exception(f'Unsupported framework: {d}')
 
 			name, operator, version = match[1], match[2], match[3]
 
-			if name not in available_frameworks:
+			if name not in s_available_frameworks:
 				raise Exception(f'Unsupported framework: {d}')
 
 			s_dependencies[name] = None if operator is None and version is None else f'{operator}{version}'
 
 	# Determine Framework versions
 	for x in s_python_packages:
 		x = x.split(' ')
 		d, v = x[0], x[-1]
 		if d in args.frameworks:
 			s_dependencies[d] = f'~={v}'
 
-	if (len(s_dependencies) - dev_cnt) == 0:
+	if args.mode != 'debug' and (len(s_dependencies) - dev_cnt) == 0:
 		raise Exception('No frameworks detected or selected via --frameworks!')
 
 	# Init default versions to prevent PIP to try hundreds of combinations
 	for k, v in s_default_versions.items():
 		if s_dependencies.get(k, False) is None: # False == not found, don't set, None == found but no version specified or found
 			s_dependencies[k] = v
 
 #-------------------------------------------------------------------------------
 # Callbacks
 #-------------------------------------------------------------------------------
 def install(args):
 	# Run PIP installation -----------------------------------------------------
-	is_install	= args.mode != 'download'
-	is_local	= args.folder != None
+	is_install	= args.mode   != 'download'
+	is_local	= args.folder is not None
 
 	credentials, user_access = None, None
 	if not is_local:
 		credentials, user_access = check_license(args)
 	
 	# Get list of plugins to be installed --------------------------------------
 	plugins = available_plugins(args, user_access)
@@ -173,20 +163,15 @@
 		uninstall(args)
 
 	cmd = ['python3', '-m', 'pip', 'install' if is_install else 'download']
 
 	if is_install and not is_virtualenv() and args.user:
 		cmd.append('--user')
 
-	for p in plugins:
-		assert isinstance(p, Plugin)
-		x = p.name
-		if p.version is not None:
-			x = f'{x}{p.version}'
-		cmd.append(x)
+	cmd += plugins
 
 	if is_local:
 		cmd.append('--no-index')
 		cmd.append('-f')
 		cmd.append(args.folder)
 	else:
 		assert isinstance(credentials, tuple) and len(credentials) == 2
@@ -195,16 +180,27 @@
 			cmd.append('--trusted-host')
 			cmd.append('sol.neclab.eu')
 
 		# https://pip.pypa.io/en/stable/topics/authentication/#percent-encoding-special-characters
 		username = credentials[0]
 		password = urllib.parse.quote(credentials[1].encode('utf8'))
 
-		urls = set(p.url for p in plugins if p.url is not None)
-		for u in urls:
+		def urls():
+			for url in user_access:
+				if 'license' in url:
+					yield f'{url}index.php/pip-license-index'
+				elif any(dev in url for dev in ['core', 'x86', 've', 'nvidia']):
+					yield f'{url}v{s_version}'
+					yield f'{url}dist'
+				elif 'dev' in url:
+					yield f'{url}v{s_version}'
+				else:
+					yield url
+
+		for u in urls():
 			cmd.append('-f')
 			cmd.append(u.replace('{USERNAME}', username).replace('{PASSWORD}', password))
 
 	run(cmd)
 
 #-------------------------------------------------------------------------------
 def uninstall(args):
@@ -233,40 +229,40 @@
 				username = args.username
 
 			password = args.password or getpass.getpass()
 			credentials = (username, password)
 			print()
 
 			if not check_login():
-				print(L_ERROR, 'Login failed!', L_RESET)
+				print(red('Login failed!'))
 				credentials = None
 	else: # non-interactive
 		credentials = (args.username, args.password)
 
 		if not check_login():
 			raise Exception('Login failed!')
 
 	user_access	= set()
 	cache		= dict()
 
-	def add_access(url):
+	def add_access(url: str) -> bool:
 		code = cache.get(url, None)
 		if isinstance(code, int):
 			return code == 200
 
 		auth = None
 		if '{USERNAME}:{PASSWORD}@' in url:
 			url		= url.replace('{USERNAME}:{PASSWORD}@', '')
 			auth	= credentials
 
 		r			= requests.get(url, auth=auth, verify=not args.trust)
 		cache[url]	= r.status_code
 		return r.status_code == 200
 
-	for url in s_access:
+	for url in s_urls:
 		if add_access(url):
 			user_access.add(url)
 
 	return credentials, user_access, cache
 
 #-------------------------------------------------------------------------------
 def fetch_license(credentials, args):
@@ -345,17 +341,17 @@
 
 		if args.accept_license:
 			license_text			= '\n'.join(license_text)
 			license_authorization	= license_authorization.replace('\n', '')
 			license_acceptance		= license_acceptance.replace('\n', '')
 			print(license_text)
 			print()
-			print(f'{license_authorization}:', L_EMPH, 'yes, I am [user accepted through --accept-license flag]', L_RESET)
+			print(f'{license_authorization}:', emph('yes, I am [user accepted through --accept-license flag]'))
 			print()
-			print(f'{license_acceptance}:', L_EMPH, 'accept license [user accepted through --accept-license flag]', L_RESET)
+			print(f'{license_acceptance}:', emph('accept license [user accepted through --accept-license flag]'))
 			print()
 		else:
 			less(license_text)
 
 			options			= ['no, I am not', 'yes, I am']
 			terminal_menu	= TerminalMenu(options, title=license_authorization)
 			choice			= terminal_menu.show()
@@ -365,90 +361,79 @@
 			terminal_menu	= TerminalMenu(options, title=license_acceptance)
 			choice			= terminal_menu.show()
 			if choice != 1:	raise Exception('License declined!')
 	
 	return credentials, user_access
 
 #-------------------------------------------------------------------------------
-def available_plugins(args, user_access: Optional[Set[str]]) -> List[Plugin]:
-	is_x86			= False
-	is_ve			= False
-	is_nvidia		= False
-	is_torch		= False
-	is_tensorflow	= False
-	is_onnx			= False
-	is_numpy		= False
-
-	def check(p):
-		nonlocal is_ve, is_x86, is_nvidia, is_torch, is_tensorflow, is_onnx, is_numpy
-
-		if user_access:
-			if p.url not in user_access:
-				return False
-		
-		for dep in p.dependencies:
-			if dep not in s_dependencies:
-				return False
-
-		n = p.name
-		if n.endswith('device-nvidia'):			is_nvidia		= True
-		if n.endswith('device-ve'):				is_ve			= True
-		if n.endswith('device-x86'):			is_x86			= True
-		if n.endswith('framework-tensorflow'):	is_tensorflow	= s_dependencies['tensorflow']
-		if n.endswith('framework-pytorch'):		is_torch		= s_dependencies['torch']
-		if n.endswith('framework-onnx'):		is_onnx			= s_dependencies['onnx']
-		if n.endswith('framework-numpy'):		is_numpy		= s_dependencies['numpy']
-
-		return True
-
-	plugins = [p for p in s_available if check(p)]
-
-	if is_tensorflow		is not False:	plugins.append(Plugin('tensorflow',			is_tensorflow	))
-	if is_torch				is not False:	plugins.append(Plugin('torch',				is_torch		))
-	if is_onnx				is not False:	plugins.append(Plugin('onnx',				is_onnx			))
-	if is_numpy				is not False:	plugins.append(Plugin('numpy',				is_numpy		))
-
-	if is_ve:
-		if is_tensorflow	is not False:	plugins.append(Plugin('veda-tensorflow',	is_tensorflow	))
-		if is_torch			is not False:	plugins.append(Plugin('veda-pytorch',		is_torch		))
+def available_plugins(args, user_access) -> List[str]:
+	plugins = []
+	extras	= []
+
+	if args.folder:
+		def has_access(x: str) -> bool:
+			return True
+	else:
+		def has_access(x: str) -> bool:
+			url = 'https://{USERNAME}:{PASSWORD}@sol.neclab.eu/' + x + '/'
+			return url in user_access
+
+	frameworks = ['tensorflow', 'torch', 'onnx', 'numpy']
+	for framework in frameworks:
+		if framework in s_dependencies:
+			extras.append(framework)
+			plugins.append(f'{framework}{s_dependencies[framework] or ""}')
+
+	for device in ['nvidia', 've', 'x86']:
+		if device in s_dependencies and has_access(device):
+			extras.append(device)
+
+	if 'tests' in s_dependencies and has_access('dev'):
+		for framework in frameworks:
+			if framework in extras:
+				extras.append(f'tests-{framework}')
+
+	if 'sdk' in s_dependencies and has_access('dev'):
+		extras.append('sdk')
+
+	if 've' in extras:
+		if 'tensorflow'	in extras: plugins.append(f'veda-tensorflow{s_dependencies["tensorflow"] or ""}')
+		if 'torch'		in extras: plugins.append(f'veda-pytorch{s_dependencies["torch"] or ""}')
 
+	plugins.append(f'{s_prefix}-sol-core[{",".join(extras)}]=={s_version}')
+	
 	if args.mode == 'download':
-		plugins.append(Plugin('nec-sol', f'=={s_version}'))
+		plugins.append(f'nec-sol=={s_version}')
 
-	return sorted(plugins, key=lambda x: x.name)
+	return sorted(plugins)
 
 #-------------------------------------------------------------------------------
 def debug(args):
 	credentials, user_access, cache = check_access(args)
 	
 	msg = fetch_license(credentials, args)
 
-	print(f'{L_EMPH}User Information:{L_RESET}')
+	print(emph('User Information:'))
 	print(f'Username: {credentials[0]}')
-	license = f'{L_ERROR}failed{L_RESET}' if isinstance(msg, Exception) else msg['license_type']
+	license = red("failed") if isinstance(msg, Exception) else msg['license_type']
 	print(f'License: {license}')
 	print()
 	
-	print(f'{L_EMPH}User Permissions:{L_RESET}')
+	print(emph('User Permissions:'))
 	for k, v in sorted(cache.items()):
-		print(f'{k.replace("{USERNAME}:{PASSWORD}@", "")}:{L_SUCCESS if v == 200 else L_ERROR} {"granted" if v == 200 else "denied"}{L_RESET}')
-	print()
-
-	print(f'{L_EMPH}Devices/Frameworks to be installed:{L_RESET}')
-	for k, v in sorted(s_dependencies.items()):
-		print(f'- {k}{"" if v is None else v}')
+		print(f'{k.replace("{USERNAME}:{PASSWORD}@", "")}:{green("granted") if v == 200 else red("denied")}')
 	print()
 
-	print(f'{L_EMPH}Plugins to be installed:{L_RESET}')
+	print(emph('Packages to be installed:'))
 	for p in available_plugins(args, user_access):
-		print(f'- {p.name}{"" if p.version is None else p.version}')
+		print(f'- {p}')
 	print()
 
 	if args.verbose:
-		print(f'{L_EMPH}Installed Packages:{L_RESET}')
+		print(emph('Installed Packages:'))
 		for line in s_python_packages:
 			print(line)
 
 #-------------------------------------------------------------------------------
 if __name__ == '__main__':
 	parser = argparse.ArgumentParser(description=f'NEC-SOL Package Manager v{s_version}')
 	parser.add_argument('mode', choices=[
@@ -460,36 +445,41 @@
 	parser.add_argument('--accept-license', action='store_true', help='accept SOL license agreement')
 	parser.add_argument('-u', '--username', default=None, type=str, help='SOL user name')
 	parser.add_argument('-p', '--password', default=None, type=str, help='SOL user password')
 	parser.add_argument('-f', '--folder', default=None, type=str, help='folder pointing to downloaded SOL packages')
 	parser.add_argument('--trust', action='store_true', help='trust all SSL certificates (not recommended)')
 	parser.add_argument('--devices', choices=[
 		'all',
-		'x86_64',
+		'x86',
 		've',
 		'nvidia'
 	], nargs='*', type=str, default=[], help='manually list devices to download/install')
+	parser.add_argument('--features', choices=[
+		'all',
+		'sdk',
+		'tests'
+	], nargs='*', type=str, default=[], help='manually list features to download/install')
 	parser.add_argument('--frameworks', nargs='*', type=str, default=[], help='manually list frameworks to download/install')
 	parser.add_argument('--user', action='store_true', help='install all packages using --user flag')
 	parser.add_argument('--verbose', action='store_true', help='shows debug information')
 	args = parser.parse_args()
 	
 	try:
 		if sys.platform != 'linux':
 			raise Exception(f'SOL only works on linux, but you are running: {sys.platform}')
 
 		initialize()
 		
-		print(f'{L_EMPH}## NEC-SOL Package Manager v{s_version}{L_RESET}')
+		print(emph(f'## NEC-SOL Package Manager v{s_version}'))
 		
 		if		args.mode == 'install':		install		(args)
 		elif	args.mode == 'download':	install		(args)
 		elif	args.mode == 'uninstall':	uninstall	(args)
 		elif	args.mode == 'debug':		debug		(args)
 		else:	raise Exception(f'unsupported installer mode: {mode}')
 	except Exception as e:
 		print()
-		print(L_ERROR, str(e), L_RESET)
+		print(red(str(e)))
 		print()
 		if args.verbose:
 			for line in traceback.format_tb(e.__traceback__):
 				print(line)
```

## Comparing `nec_sol-0.5.1.post1.dist-info/METADATA` & `nec_sol-0.5.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: nec-sol
-Version: 0.5.1.post1
-Requires-Python: >=3.7
-Summary: SOL Installer
+Version: 0.5.2
+Requires-Python: >=3.8
+Summary: NEC SOL Installer
 Author: Nicolas Weber
 Author-email: nicolas.weber@neclab.eu
 Home-page: https://sol.neclab.eu/
+License: Other/Proprietary License
 Platform: linux_x86_x64
-Project-URL: Documentation, https://sol.neclab.eu/docs/v0.5.1
+Project-URL: Documentation, https://sol.neclab.eu/docs/v0.5.2
 Project-URL: Bug Tracker, https://gitlab.neclab.eu/
-Requires-Dist: simple-term-menu
 Requires-Dist: requests
+Requires-Dist: termcolor
+Requires-Dist: simple-term-menu
 Description-Content-Type: text/markdown
 
 ![SOL Logo](https://sol.neclab.eu/logo.svg)
 
 <hr/>
 
 ```nec-sol``` is the installation wrapper for the [SOL Neural Network
@@ -23,8 +25,8 @@
 
 See the [documentation](https://sol.neclab.eu/docs/) on how to perform the
 installation.
 
 ## Useful Links:
 * [Documentation](https://sol.neclab.eu/docs/)
 * [Issue Tracker](https://sol.neclab.eu/issue/)
-* [Homepage](https://sol.neclab.eu/)
+* [Homepage](https://sol.neclab.eu/)
```

