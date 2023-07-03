# Comparing `tmp/dddmisc-mongo-uow-1.0.0.tar.gz` & `tmp/dddmisc_mongo_uow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dddmisc-mongo-uow-1.0.0.tar", max compression
+gzip compressed data, was "dddmisc_mongo_uow-1.0.1.tar", max compression
```

## Comparing `dddmisc-mongo-uow-1.0.0.tar` & `dddmisc_mongo_uow-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7799 2022-12-19 11:04:30.480029 dddmisc-mongo-uow-1.0.0/README.md
--rw-r--r--   0        0        0      895 2022-12-20 05:00:45.948789 dddmisc-mongo-uow-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      108 2022-12-19 11:00:39.349990 dddmisc-mongo-uow-1.0.0/src/dddmisc_mongo_uow/__init__.py
--rw-r--r--   0        0        0      558 2022-12-19 11:00:39.349990 dddmisc-mongo-uow-1.0.0/src/dddmisc_mongo_uow/abstraction.py
--rw-r--r--   0        0        0     2607 2022-12-19 11:00:39.349990 dddmisc-mongo-uow-1.0.0/src/dddmisc_mongo_uow/unit_of_work_tools.py
--rw-r--r--   0        0        0     8705 2022-12-20 05:00:46.652307 dddmisc-mongo-uow-1.0.0/setup.py
--rw-r--r--   0        0        0     8223 2022-12-20 05:00:46.652803 dddmisc-mongo-uow-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7799 2023-07-03 09:58:01.002002 dddmisc_mongo_uow-1.0.1/README.md
+-rw-r--r--   0        0        0      837 2023-07-03 10:03:23.056271 dddmisc_mongo_uow-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-03 09:58:01.004002 dddmisc_mongo_uow-1.0.1/src/dddmisc_mongo_uow/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-03 09:58:01.004002 dddmisc_mongo_uow-1.0.1/src/dddmisc_mongo_uow/abstraction.py
+-rw-r--r--   0        0        0     3212 2023-07-03 09:58:01.004002 dddmisc_mongo_uow-1.0.1/src/dddmisc_mongo_uow/unit_of_work_tools.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 dddmisc_mongo_uow-1.0.1/setup.py
+-rw-r--r--   0        0        0     8225 1970-01-01 00:00:00.000000 dddmisc_mongo_uow-1.0.1/PKG-INFO
```

### Comparing `dddmisc-mongo-uow-1.0.0/README.md` & `dddmisc_mongo_uow-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dddmisc-mongo-uow-1.0.0/pyproject.toml` & `dddmisc_mongo_uow-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "dddmisc-mongo-uow"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Aziz <walkingonadream2012@mail.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 motor = "3.*"
 ddd-misc = "^0.8.1"
 
-[tool.poetry.dev-dependencies]
-poethepoet = "^0.16.5"
+[tool.poetry.group.dev.dependencies]
+poethepoet = "^0.20.0"
 pylama = "^8.4.1"
-pytest-xdist = "^3.1.0"
-pytest-tornasync = "^0.6.0.post2"
-pytest-trio = "^0.8.0"
-pytest-asyncio = "^0.20.3"
 pytest = "^7.2.0"
-pydantic = {extras = ["python-dotenv"], version = "^1.10.2"}
-python-dotenv = "^0.21.0"
+python-dotenv = "^1.0.0"
 pytest-cov = {extras = ["toml"], version = "^4.0.0"}
+pydantic-settings = "^2.0.0"
+pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 lint = "poetry run pylama ./src/dddmisc_mongo_uow --ignore E501,W0611 --linters print,pyflakes --format pylint"
-test = "poetry run pytest --cov=. --cov-report=term-missing --cov-report=xml --junitxml=test-report.xml tests"
+test = "poetry run pytest --cov=. --cov-report=term-missing --cov-report=xml --junitxml=test-report.xml tests"
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
```

### Comparing `dddmisc-mongo-uow-1.0.0/src/dddmisc_mongo_uow/abstraction.py` & `dddmisc_mongo_uow-1.0.1/src/dddmisc_mongo_uow/abstraction.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 class AbstractMongoRepository(AbstractAsyncRepository, abc.ABC):
 
     def __init__(self, connection: AsyncIOMotorClientSession, collections: Mapping[str, AsyncIOMotorCollection]):
         super().__init__(connection)
         self._collections = collections
 
     def _get_mongo_collection(self, collection_name: str) -> AsyncIOMotorCollection:
-        return self._collections[collection_name]
+        return self._collections[collection_name]
```

### Comparing `dddmisc-mongo-uow-1.0.0/src/dddmisc_mongo_uow/unit_of_work_tools.py` & `dddmisc_mongo_uow-1.0.1/src/dddmisc_mongo_uow/unit_of_work_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,52 @@
+from bson import UuidRepresentation, CodecOptions
 from dddmisc import AbstractAsyncUnitOfWork
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorCollection, AsyncIOMotorClientSession
 from types import MappingProxyType
 from typing import Iterable, Mapping
 from functools import partial
 
 from .abstraction import AbstractMongoRepository
 
 
 class MongoEngine:
-    def __init__(self, address: str, db_name, collections: Iterable[str]):
+    def __init__(
+            self,
+            address: str,
+            db_name: str,
+            collections: Iterable[str],
+            codec_options: CodecOptions = None,
+    ):
         self._client = AsyncIOMotorClient(address)
         self._db = self._client[db_name]
-        collections_dict = dict()
-        for collection in collections:
-            collections_dict[collection] = self._db[collection]
-        self._collections = MappingProxyType(collections_dict)
+        collections_with_options = self._get_collections_with_options(collections, codec_options)
+        self._collections = MappingProxyType(collections_with_options)
 
     def get_collections(self) -> Mapping[str, AsyncIOMotorCollection]:
         return self._collections
 
     async def get_session(self) -> AsyncIOMotorClientSession:
         return await self._client.start_session()
 
+    def _get_collections_with_options(self, collections: Iterable[str], codec_options: CodecOptions):
+        collections_with_options = dict()
+        codec_options = codec_options or CodecOptions(
+            tz_aware=True,
+            uuid_representation=UuidRepresentation.STANDARD
+        )
+        for collection in collections:
+            collections_with_options[collection] = self._db[collection].with_options(codec_options)
+        return collections_with_options
+
 
 class MongoMotorUOW(AbstractAsyncUnitOfWork):
 
     def __init__(self, engine: MongoEngine, repository_class: AbstractMongoRepository):
         if not issubclass(repository_class, AbstractMongoRepository):
-            raise TypeError('Repository class in "MongoMotorUOW" can be subclass of "AbstractMongoRepository"')
+            raise TypeError('Repository class in "MongoMotorUOW" must be subclass of "AbstractMongoRepository"')
         repository_class = partial(repository_class, collections=engine.get_collections())
         super().__init__(engine, repository_class)
 
     async def _begin_transaction(self, mongo_engine: MongoEngine) -> AsyncIOMotorClientSession:
         self._mongo_session = await mongo_engine.get_session()
         session_context = await self._mongo_session.__aenter__()
         self._trn_context = session_context.start_transaction()
@@ -51,8 +66,8 @@
     async def _rollback_transaction(self, session_context) -> None:
         if hasattr(self, '_trn_context'):
             await session_context.abort_transaction()
             trn_context = self._trn_context
             await trn_context.__aexit__(None, None, None)
             delattr(self, '_trn_context')
             await self._mongo_session.__aexit__(None, None, None)
-            delattr(self, '_mongo_session')
+            delattr(self, '_mongo_session')
```

### Comparing `dddmisc-mongo-uow-1.0.0/setup.py` & `dddmisc_mongo_uow-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 {'': ['*']}
 
 install_requires = \
 ['ddd-misc>=0.8.1,<0.9.0', 'motor>=3.0.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'dddmisc-mongo-uow',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': '',
     'long_description': '# MongoDB async ddd-misc UnitOfWork\n\nMongoDB UnitOfWork на базе ddd-misc и библиотеки Motor: Asynchronous Python driver for MongoDB.\n\n\n## Классы\n\n**AbstractMongoRepository**\n\nAbstractMongoRepository - абстрактный класс для реализации репозитория с подключением к базе данных MongoDB. Класс реализует \nсигнатуру для инициализации с двумя параметрами помимо self и метод \'get_mongo_collection\':\n\n    - \'connection\' - параметр принимающий контекст инстанса класса AsyncIOMotorClientSession библиотеки Motor.\n\n    - \'collections\' - параметр принимающий структуру dict ключами которой являются название mongo коллекции в виде строки, а значениями объект класса AsyncIOMotorCollection библиотеки Motor.\n\n    \'_get_mongo_collection\' - метод класса AbstractMongoRepository, возвращающий mongo коллекцию по передаваемому названию в параметре в виде строки.\n\nДанный класс обязателен для наследования при реализации конкретного MongoDB репозитория в рамках UnitOfWork данного пакета.\n\nПример использования:\n```\nfrom dddmisc_mongo_uow import AbstractMongoRepository\n\n\nclass ConcreteMongoRepository(AbstractMongoRepository):\n    aggregate_class = ConcreteAggregateClass\n    \n    async def _add_to_storage(self, aggregate):\n        document = dict(\n            key=aggregate._key,\n            reference=str(aggregate.reference)\n        )\n        collection = self._get_mongo_collection(\'uow\')\n        await collection.update_one({\'reference\': document[\'reference\']}, {\'$set\' : document}, upsert=True, session=self._connection)\n```\n\n**MongoEngine**\n\nMongoEngine - класс для создания структуры engine MongoDB версии, engine передается в параметры при инициализации AsyncMessageBus.\nПри инициализации MongoEngine требует трех обязательных параметров:\n\n    - \'address\' - параметр принимающий строку для подключения к конкретной базе данных MongoDB, включающей в себя хост базы, а так же дополнительные параметры подключения. Пример - \'mongodb://localhost:27017/?directConnection=true\'. При инициализации по параметру создается объект AsyncIOMotorClient.\n\n    - \'db_name\' - параметр принимающий строку с названием базы данных. При инициализации создается объект AsyncIOMotorDatabase.\n\n    - \'collections\' - парамтер принимающий массив с названиями коллекции MongoDB в виде строк. При инициализации создается структура неизменяемого dict, ключами которой являются названия коллекции, а значениями объекты AsyncIOMotorCollection с подключением к данным коллекциям.\n\n    \'get_collections\' - метод возвращающий коллекции.\n\n    \'get_session\' - асинхронный метод возврщающий объект AsyncIOMotorClientSession для проведения транзакции.\n\nПример использования:\n```\nfrom dddmisc_mongo_uow import MongoEngine\n\n\nmongo_engine = MongoEngine(address=\'mongodb://localhost:27017/?directConnection=true\', db_name=\'mongo_uow\', collections=[\'uow\'])\n\ncollections = mongo_engine.get_collections()\n\nsession = await mongo_engine.get_session()\n```\n\n**MongoMotorUOW**\n\nMongoMotorUOW - класс на базе AbstractAsyncUnitOfWork, реализующий конкретный объект UnitOfWork и его стандартное поведение в рамках ddd-misc для выполнения транзакции в MongoDB.\n\nКласс реализует стандартную сигнатуру для создания объекта UnitOfWork в процессе выполнения хэндлера в объекте AsyncMessageBus, требующую двух параметров engine и repository_class. В процессе инициализации проверяется является ли repository_class субклассом AbstractMongoRepository, далее repository_class оборачивается классом декоратором вместе с параметром collections, чтобы UnitOfWork мог передавать один параметр connection при инициализации репозитория.\n\nПример использования:\n```\nfrom dddmisc import AsyncMessageBus\nfrom dddmisc_mongo_uow import MongoMotorUOW\n\nmessage_bus = AsyncMessageBus(\n    uow_class=MongoMotorUOW,\n    repository_class=ConcreteMongoRepository,\n    engine=mongo_engine\n)\n```\n\n\n## Основные параметры для запуска MongoDB в .gitlab-ci.yml:\n```\n  services:\n    - name: mongo:6.0\n      alias: mongo-svc\n      command: ["mongod", "--logpath=/dev/null", "--bind_ip_all", "--replSet=rs0"]\n  before_script:\n    - python -V\n    - python -m venv .venv\n    - poetry install\n    - apt-get update && apt-get install -y gnupg\n    - apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/*\n    - wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | apt-key add -\n    - echo "deb http://repo.mongodb.org/apt/debian buster/mongodb-org/6.0 main" |  tee /etc/apt/sources.list.d/mongodb-org-6.0.list\n    - apt-get update\n    - apt-get install -y mongodb-org\n    - mongosh --host mongo-svc --eval "rs.initiate({\'_id\':\'rs0\',\'members\':[{\'_id\':0,\'host\':\'127.0.0.1:27017\'}]});"\n  script:\n    - mongosh --host mongo-svc --eval "rs.status()"\n    - poetry run poe test\n```\n\nПри установке отличающейся версии MongoDB параметры установки нужно изменить на акутальную версию.\n\nКомманда `rs.initiate({\'_id\':\'rs0\',\'members\':[{\'_id\':0,\'host\':\'mongo-svc\'}]});` инициирует реплику.\n\n\nНа странице https://www.mongodb.com/docs/manual/reference/connection-string/ описан формат строки подключения и разные его варианты.\n\n\nСтандартный формат подключения:\n\n    - \'mongodb://localhost:27017/\'\n\nРабочий формат подключения на локальном компьютере при инициации \'rs.initiate()\':\n\n    - \'mongodb://localhost:27017/?directConnection=true\'\n\nПри инициации \'rs.initiate({\'_id\':\'rs0\',\'members\':[{\'_id\':0,\'host\':\'mongo-svc\'}]})\' создается конкретная реплика, их может быть несколько, например:\n\n```\n    rs.initiate(\n    {\n        _id: "rs0",\n        version: 1,\n        members: [\n            { _id: 0, host : "mongodb0.example.net:27017" },\n            { _id: 1, host : "mongodb1.example.net:27017" },\n            { _id: 2, host : "mongodb2.example.net:27017" }\n        ]\n    }\n    )\n```\n\'rs0\' - имя набора реплик, задается при поднятии базы, строка подключения на локалке:\n\n    - \'mongodb://localhost:27017/?directConnection=true&replicaSet=rs0',
     'author': 'Aziz',
     'author_email': 'walkingonadream2012@mail.ru',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `dddmisc-mongo-uow-1.0.0/PKG-INFO` & `dddmisc_mongo_uow-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dddmisc-mongo-uow
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Aziz
 Author-email: walkingonadream2012@mail.ru
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ddd-misc (>=0.8.1,<0.9.0)
 Requires-Dist: motor (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # MongoDB async ddd-misc UnitOfWork
 
 MongoDB UnitOfWork на базе ddd-misc и библиотеки Motor: Asynchronous Python driver for MongoDB.
```

