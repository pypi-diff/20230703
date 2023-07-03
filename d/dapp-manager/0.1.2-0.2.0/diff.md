# Comparing `tmp/dapp_manager-0.1.2.tar.gz` & `tmp/dapp_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapp_manager-0.1.2.tar", max compression
+gzip compressed data, was "dapp_manager-0.2.0.tar", max compression
```

## Comparing `dapp_manager-0.1.2.tar` & `dapp_manager-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
--rw-r--r--   0        0        0    26526 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/LICENSE
--rw-r--r--   0        0        0     7276 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/README.md
--rw-r--r--   0        0        0      149 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/__init__.py
--rw-r--r--   0        0        0       97 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/__main__.py
--rw-r--r--   0        0        0     1261 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/__init__.py
--rw-r--r--   0        0        0      674 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.bash
--rw-r--r--   0        0        0      171 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.fish
--rw-r--r--   0        0        0      900 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.zsh
--rw-r--r--   0        0        0     4825 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/cli.py
--rw-r--r--   0        0        0     9265 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/dapp_manager.py
--rw-r--r--   0        0        0     4056 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/dapp_starter.py
--rw-r--r--   0        0        0     2067 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/py.typed
--rw-r--r--   0        0        0     4887 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/storage.py
--rw-r--r--   0        0        0       50 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/README.md
--rw-r--r--   0        0        0       70 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/__init__.py
--rw-r--r--   0        0        0     1634 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/__main__.py
--rw-r--r--   0        0        0     4928 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/dapp_size_resolver.py
--rw-r--r--   0        0        0     1960 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/dapp_stats.py
--rw-r--r--   0        0        0      118 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/__init__.py
--rw-r--r--   0        0        0      360 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/enums.py
--rw-r--r--   0        0        0     1272 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/models.py
--rw-r--r--   0        0        0      257 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/schemas.py
--rw-r--r--   0        0        0     4499 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8500 1970-01-01 00:00:00.000000 dapp_manager-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7276 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/README.md
+-rw-r--r--   0        0        0      149 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/__main__.py
+-rw-r--r--   0        0        0     1261 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/autocomplete/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/autocomplete/scripts/.dapp-manager.bash
+-rw-r--r--   0        0        0      171 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/autocomplete/scripts/.dapp-manager.fish
+-rw-r--r--   0        0        0      900 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/autocomplete/scripts/.dapp-manager.zsh
+-rw-r--r--   0        0        0     5819 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/cli.py
+-rw-r--r--   0        0        0    10016 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/dapp_manager.py
+-rw-r--r--   0        0        0     4707 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/dapp_starter.py
+-rw-r--r--   0        0        0     2545 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/exceptions.py
+-rw-r--r--   0        0        0       74 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/inspect/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/inspect/__main__.py
+-rw-r--r--   0        0        0      209 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/inspect/templates/app_structure/network.txt
+-rw-r--r--   0        0        0     1102 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/inspect/templates/app_structure/node.txt
+-rw-r--r--   0        0        0      158 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/inspect/templates/app_structure/payload.txt
+-rw-r--r--   0        0        0      720 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/inspect/templates/app_structure.txt
+-rw-r--r--   0        0        0        0 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/py.typed
+-rw-r--r--   0        0        0     5927 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_manager/storage.py
+-rw-r--r--   0        0        0       50 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/README.md
+-rw-r--r--   0        0        0       70 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/__main__.py
+-rw-r--r--   0        0        0     4925 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/dapp_size_resolver.py
+-rw-r--r--   0        0        0     1960 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/dapp_stats.py
+-rw-r--r--   0        0        0      118 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/statistics/__init__.py
+-rw-r--r--   0        0        0      360 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/statistics/enums.py
+-rw-r--r--   0        0        0     1272 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/statistics/models.py
+-rw-r--r--   0        0        0      257 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/dapp_stats/statistics/schemas.py
+-rw-r--r--   0        0        0     4535 2023-07-03 08:33:39.393310 dapp_manager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8572 1970-01-01 00:00:00.000000 dapp_manager-0.2.0/PKG-INFO
```

### Comparing `dapp_manager-0.1.2/LICENSE` & `dapp_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/README.md` & `dapp_manager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/dapp_manager/autocomplete/__init__.py` & `dapp_manager-0.2.0/dapp_manager/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.bash` & `dapp_manager-0.2.0/dapp_manager/autocomplete/scripts/.dapp-manager.bash`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.zsh` & `dapp_manager-0.2.0/dapp_manager/autocomplete/scripts/.dapp-manager.zsh`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/dapp_manager/cli.py` & `dapp_manager-0.2.0/dapp_manager/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,18 +54,50 @@
     required=True,
     type=Path,
 )
 @click.option(
     "--log-level",
     type=click.Choice(LOG_CHOICES, case_sensitive=False),
 )
+@click.option("--api-port", type=int, help="Enable the GAOM API on a given port.")
+@click.option(
+    "--api-host",
+    type=str,
+    help="Specify a host address for the GAOM API to bind to. (default: 127.0.0.1)"
+    "Requires `--api-port` to also be specified.",
+)
+@click.option(
+    "--skip-manifest-validation",
+    is_flag=True,
+    default=False,
+)
 @_capture_api_exceptions
-def start(descriptors: Tuple[Path], *, config: Path, log_level: Optional[str]):
+def start(
+    descriptors: Tuple[Path],
+    *,
+    config: Path,
+    log_level: Optional[str],
+    api_port: Optional[int],
+    api_host: str,
+    skip_manifest_validation: bool,
+):
     """Start a new app using the provided descriptor and config files."""
-    dapp = DappManager.start(*descriptors, config=config, log_level=log_level)
+    if api_port:
+        api_kwargs = {"api_host": api_host or "127.0.0.1", "api_port": api_port}
+    elif api_host:
+        raise DappManagerException("To enable the API, please specify the `--api-port` too.")
+    else:
+        api_kwargs = {}
+    dapp = DappManager.start(
+        *descriptors,
+        config=config,
+        log_level=log_level,
+        skip_manifest_validation=skip_manifest_validation,
+        **api_kwargs,  # type: ignore [arg-type] # noqa
+    )
     print(dapp.app_id)
 
 
 @cli.command()
 @_capture_api_exceptions
 def list():
     """List known app IDs (both active and dead).
@@ -142,14 +174,22 @@
 def exec(*, app_id, service, command, timeout):
     dapp = DappManager(app_id)
     dapp.exec_command(service, command, timeout)
 
 
 @cli.command()
 @_with_app_id
+@_capture_api_exceptions
+def inspect(*, app_id):
+    dapp = DappManager(app_id)
+    print(dapp.inspect())
+
+
+@cli.command()
+@_with_app_id
 @click.argument("file-type", type=click.Choice(["state", "data", "log", "stdout", "stderr"]))
 @click.option(
     "--ensure-alive/--no-ensure-alive",
     default=True,
 )
 @click.option(
     "-f",
@@ -163,15 +203,15 @@
 
     dapp = DappManager(app_id)
 
     if follow:
         for chunk in dapp.read_file_follow(file_type, ensure_alive=ensure_alive):
             print(chunk, end="")
     else:
-        print(dapp.read_file(file_type, ensure_alive=ensure_alive))
+        print(dapp.read_file(file_type, ensure_alive=ensure_alive), end="")
 
 
 @cli.command()
 @click.argument("shell", type=click.Choice(["bash", "fish", "zsh"]))
 @click.option(
     "--path",
     "-p",
```

### Comparing `dapp_manager-0.1.2/dapp_manager/dapp_manager.py` & `dapp_manager-0.2.0/dapp_manager/dapp_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from time import sleep
 from typing import Iterator, List, Optional, Union
 
 import appdirs
 import psutil
 
 from .dapp_starter import DappStarter
-from .exceptions import AppNotRunning
+from .exceptions import AppNotRunning, GaomApiUnavailable
+from .inspect import Inspect
 from .storage import RunnerReadFileType, SimpleStorage
 
 PathType = Union[str, os.PathLike]
 
 COMMAND_OUTPUT_INTERVAL = timedelta(seconds=1)
 READ_FILE_FOLLOW_INTERVAL = timedelta(milliseconds=100)
 READ_FILE_CHUNK_SIZE = 1024
@@ -50,26 +51,37 @@
     @classmethod
     def start(
         cls,
         descriptor: PathType,
         *other_descriptors: PathType,
         config: PathType,
         log_level: Optional[str] = None,
+        api_host: Optional[str] = None,
+        api_port: Optional[int] = None,
+        skip_manifest_validation: bool = False,
         timeout: float = 1,
     ) -> "DappManager":
         """Start a new app."""
 
         descriptor_paths = [Path(d) for d in [descriptor, *other_descriptors]]
         config_path = Path(config)
 
         app_id = uuid.uuid4().hex
         storage = cls._create_storage(app_id)
         storage.init()
 
-        starter = DappStarter(descriptor_paths, config_path, storage, log_level=log_level)
+        starter = DappStarter(
+            descriptor_paths,
+            config_path,
+            storage,
+            log_level=log_level,
+            api_host=api_host,
+            api_port=api_port,
+            skip_manifest_validation=skip_manifest_validation,
+        )
         starter.start(timeout=timeout)
 
         return cls(app_id)
 
     @classmethod
     def prune(cls) -> List[str]:
         """Remove all the information about past (i.e. not running now) apps.
@@ -192,14 +204,21 @@
                     commands = msg.get(service_name, {}).get(str(service_idx))
                     for cdict in commands:
                         self.__print_executed_command(cdict)
                     break
 
                 raise TimeoutError()
 
+    def inspect(self) -> str:
+        """Query the GAOM API and present a comprehensive report."""
+        self._ensure_alive()
+        api = self._ensure_api()
+        inspect = Inspect(api)
+        return inspect.display_app_structure()
+
     def stop(self, timeout: int) -> bool:
         """Stop the dapp gracefully (SIGINT), waiting at most `timeout` seconds.
 
         Returned value indicates if the app was successfully stopped.
         """
 
         self._ensure_alive()
@@ -254,14 +273,19 @@
         if not self._is_running():
             self.storage.set_not_running()
 
     def _ensure_alive(self) -> None:
         if not self.alive:
             raise AppNotRunning(self.app_id)
 
+    def _ensure_api(self) -> str:
+        if not self.storage.api:
+            raise GaomApiUnavailable(self.app_id)
+        return self.storage.api
+
     def _is_running(self) -> bool:
         try:
             # TODO: https://github.com/golemfactory/dapp-manager/issues/9
 
             this_process = psutil.Process()
             app_process = psutil.Process(self.pid)
```

### Comparing `dapp_manager-0.1.2/dapp_manager/dapp_starter.py` & `dapp_manager-0.2.0/dapp_manager/dapp_starter.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,19 +14,25 @@
 class DappStarter:
     def __init__(
         self,
         descriptors: List[Path],
         config: Path,
         storage: SimpleStorage,
         log_level: Optional[str] = None,
+        api_host: Optional[str] = None,
+        api_port: Optional[int] = None,
+        skip_manifest_validation: bool = False,
     ):
         self.descriptors = descriptors
         self.config = config
         self.storage = storage
         self.log_level = log_level
+        self.api_host = api_host
+        self.api_port = api_port
+        self.skip_manifest_validation = skip_manifest_validation
 
     def start(self, timeout: float) -> None:
         """Start a dapp. Wait TIMEOUT seconds. Raise StartupFailed if process is not running."""
 
         command = self._get_command()
 
         # Handling graceful shutdown for windows.
@@ -54,14 +60,17 @@
                 runner_stderr = None
 
             self.storage.delete()
 
             raise StartupFailed(stdout, stderr, runner_stdout, runner_stderr)
 
         self.storage.save_pid(proc.pid)
+        if self.api_host and self.api_port:
+            self.storage.save_api_host(self.api_host)
+            self.storage.save_api_port(self.api_port)
 
     def _check_succesful_startup(
         self, proc: subprocess.Popen, timeout: float
     ) -> Tuple[bool, str, str]:
         stop = datetime.now() + timedelta(seconds=timeout)
 
         outputs: List[str] = []
@@ -97,15 +106,22 @@
             args += ["--log-level", self.log_level]
 
         # TODO: is there's a better way to iterate over elements of a Literal type?
         for file_type in RunnerFileType.__args__:  # type: ignore [attr-defined]
             file_name = str(self.storage.file_name(file_type).resolve())
             args += [f"--{file_type}", file_name]
 
+        if self.api_host and self.api_port:
+            args += ["--enable-api", "--api-host", self.api_host, "--api-port", str(self.api_port)]
+
         args += [str(d.resolve()) for d in self.descriptors]
+
+        if self.skip_manifest_validation:
+            args += ["--skip-manifest-validation"]
+
         return args
 
     def _executable(self) -> List[str]:
         """Return the "dapp-runner" executable - either set by the env variable or the default.
 
         Env variable is intended mostly for the testing/debugging purposes.
         """
```

### Comparing `dapp_manager-0.1.2/dapp_manager/exceptions.py` & `dapp_manager-0.2.0/dapp_manager/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,7 +65,22 @@
                 stderr,
                 "--- pre-runner stdout ---",
                 stdout,
             ]
         )
 
         super().__init__(msg)
+
+
+class GaomApiUnavailable(DappManagerException):
+    """Exception raised the command requires the GAOM API to be available but is not present.
+
+    For the API to be available, the `dapp-manager` must be invoked with the `--api` option
+    specifying the hostname and port.
+    """
+
+    SHELL_EXIT_CODE = 7
+
+    def __init__(self, app_id):
+        super().__init__(
+            f"GAOM API unavailable for {app_id}. Please start the app with the `--app-port` option."
+        )
```

### Comparing `dapp_manager-0.1.2/dapp_manager/storage.py` & `dapp_manager-0.2.0/dapp_manager/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,32 +11,43 @@
 READ_FILE_ITER_CHUNK_SIZE = 1024
 
 RunnerFileType = Literal["data", "state", "log", "stdout", "stderr", "commands"]
 RunnerReadFileType = Literal["data", "state", "log", "stdout", "stderr"]
 
 
 class SimpleStorage:
+    _api_address: Optional[str]
+
     def __init__(self, app_id: str, data_dir: str):
         self.app_id = re.sub("[\n\r/\\\\.]", "", app_id)
         self.base_dir = Path(data_dir).resolve()
+        self._api_address = None
 
     def init(self) -> None:
         """Initialize storage for `self.app_id`.
 
         There is a separate method (instead of e.g. a call in `__init__`) because we want to do
         this only once per `app_id` and in a fully controlled manner.
         """
 
         self._data_dir.mkdir(parents=True)
 
     def save_pid(self, pid: int) -> None:
         # TODO: https://github.com/golemfactory/dapp-manager/issues/12
-        with open(self.pid_file, "w") as f:
+        with self.pid_file.open("w") as f:
             f.write(str(pid))
 
+    def save_api_host(self, api_host: str) -> None:
+        with self.api_host_file.open("w") as f:
+            f.write(api_host)
+
+    def save_api_port(self, api_port: int) -> None:
+        with self.api_port_file.open("w") as f:
+            f.write(str(api_port))
+
     def set_not_running(self) -> None:
         try:
             os.rename(self.pid_file, self.archived_pid_file)
         except FileNotFoundError:
             pass
 
     def delete(self) -> None:
@@ -134,15 +145,41 @@
     def pid_file(self) -> Path:
         return self.file_name("pid")
 
     @property
     def archived_pid_file(self) -> Path:
         return self.file_name("_old_pid")
 
-    def file_name(self, name: Union[RunnerFileType, Literal["pid", "_old_pid"]]) -> Path:
+    def fetch_api_address(self):
+        try:
+            with self.api_host_file.open("r") as f:
+                host = f.read()
+            with self.api_port_file.open("r") as f:
+                port = int(f.read())
+            self._api_address = f"http://{host}:{port}"
+        except FileNotFoundError:
+            pass
+
+    @property
+    def api(self) -> Optional[str]:
+        if not self._api_address:
+            self.fetch_api_address()
+        return self._api_address
+
+    @property
+    def api_host_file(self) -> Path:
+        return self.file_name("api_host")
+
+    @property
+    def api_port_file(self) -> Path:
+        return self.file_name("api_port")
+
+    def file_name(
+        self, name: Union[RunnerFileType, Literal["pid", "_old_pid", "api_host", "api_port"]]
+    ) -> Path:
         # NOTE: "Known app" test here is sufficient - this method will be called whenever any piece
         # of information related to self.app_id is retrieved or changed
         self._ensure_known_app()
         return self._data_dir / name
 
     def _ensure_known_app(self) -> None:
         if not os.path.isdir(self._data_dir):
```

### Comparing `dapp_manager-0.1.2/dapp_stats/__main__.py` & `dapp_manager-0.2.0/dapp_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/dapp_stats/dapp_size_resolver.py` & `dapp_manager-0.2.0/dapp_stats/dapp_size_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def _get_dapp_from_descriptor_paths(cls, descriptor_paths: Sequence[Path]) -> DappDescriptor:
         try:
             dapp_dict = load_yamls(*descriptor_paths)
         except FileNotFoundError as e:
             raise DappSizeResolverError(f"Failed to load descriptor files: {e}")
 
         try:
-            return DappDescriptor.load(dapp_dict)
+            return DappDescriptor(**dapp_dict)
         except Exception as e:
             raise DappSizeResolverError(f"Failed to validate descriptor files: {e}")
 
     @classmethod
     def _resolve_payload_size_for_vm_runtime(cls, payload: PayloadDescriptor) -> int:
         try:
             image_hash = payload.params["image_hash"]
```

### Comparing `dapp_manager-0.1.2/dapp_stats/dapp_stats.py` & `dapp_manager-0.2.0/dapp_stats/dapp_stats.py`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/dapp_stats/statistics/models.py` & `dapp_manager-0.2.0/dapp_stats/statistics/models.py`

 * *Files identical despite different names*

### Comparing `dapp_manager-0.1.2/pyproject.toml` & `dapp_manager-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapp-manager"
-version = "0.1.2"
+version = "0.2.0"
 description = "Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
@@ -31,15 +31,17 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 
 psutil = "^5.9"
 appdirs = "^1.4"
 click = "^7.0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
 pydantic = "^1.9"
-dapp-runner = "^0.1.2"
+dapp-runner = "0.2.0"
+mako = "^1.2.4"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "*"  # implicitly required by liccehck
 pip = "*"  # implicitly required by liccehck
 
 autoflake = "^1"
 black = "^21.0b0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
```

### Comparing `dapp_manager-0.1.2/PKG-INFO` & `dapp_manager-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapp-manager
-Version: 0.1.2
+Version: 0.2.0
 Summary: Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface
 Home-page: https://github.com/golemfactory/dapp-manager
 License: LGPL-3.0
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,17 +17,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: appdirs (>=1.4,<2.0)
 Requires-Dist: click (>=7.0,<8.0)
-Requires-Dist: dapp-runner (>=0.1.2,<0.2.0)
+Requires-Dist: dapp-runner (==0.2.0)
+Requires-Dist: mako (>=1.2.4,<2.0.0)
 Requires-Dist: psutil (>=5.9,<6.0)
 Requires-Dist: pydantic (>=1.9,<2.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/golemfactory/dapp-manager
 Description-Content-Type: text/markdown
 
 # Golem dApp Manager
 
 `dapp-manager` is a purposefully minimalistic manager for decentralized applications running on
 Golem. It works together with the [dapp-runner](https://github.com/golemfactory/dapp-runner/).
```

