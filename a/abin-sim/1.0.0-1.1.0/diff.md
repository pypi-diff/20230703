# Comparing `tmp/abin_sim-1.0.0.tar.gz` & `tmp/abin_sim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-1.0.0.tar", max compression
+gzip compressed data, was "abin_sim-1.1.0.tar", max compression
```

## Comparing `abin_sim-1.0.0.tar` & `abin_sim-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-06-26 17:15:54.510261 abin_sim-1.0.0/LICENSE
--rw-r--r--   0        0        0     7972 2023-06-26 17:15:54.510261 abin_sim-1.0.0/README.md
--rw-r--r--   0        0        0       21 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/__init__.py
--rw-r--r--   0        0        0     7472 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/config.py
--rw-r--r--   0        0        0     1174 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     4337 2023-06-26 17:15:54.510261 abin_sim-1.0.0/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-06-26 17:15:54.510261 abin_sim-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 abin_sim-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-07-03 12:52:48.616804 abin_sim-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8593 2023-07-03 12:52:48.616804 abin_sim-1.1.0/README.md
+-rw-r--r--   0        0        0       21 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/config.py
+-rw-r--r--   0        0        0     1174 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     5320 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-07-03 12:52:48.616804 abin_sim-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9482 1970-01-01 00:00:00.000000 abin_sim-1.1.0/PKG-INFO
```

### Comparing `abin_sim-1.0.0/README.md` & `abin_sim-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,54 +55,73 @@
 
     Retorna uma breve explicação sobre a funcionalidade do CLI.
     Traz exemplos de uso e link para projeto no GitHub
 
 ### VERSION
     Uso: abin --version
 
+    Retorna a versão atualmente instalada no SO.
+    Para atualizá-la:
+
+    pipx upgrade abin_sim
+
 ### CONFIGURE
     Uso: abin --configure
-   
+
+    Gera o arquivo de configuração da aplicação.
+
+## LIST
+    Uso: abin list
+
+    Retorna a árvore de Secrets cadastradas no Path obedecendo a referência abaixp
+    ╭─ Referênvia ──────────────────╮
+    │                               │ 
+    │ Vault Environment:            │
+    │     ├── (env)-(proj)          │
+    │     │    ├── (api)            │
+    │                               │
+    ╰─ Referênvia ──────────────────╯
+
 ### GET
-    Usage: abin get [OPTIONS]                                                                                                                            
+    Uso: abin get [OPTIONS]                                                                                                                            
                                                                                                                                                       
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                        │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]               │
-    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required] │
+    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua) [default: None] [required]     │
     │    --file    --no-file          Cria um arquivo para cada path cadastrada no secrets. [default: file]                                                │
     │    --help                       Show this message and exit.                                                                                          │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
-    For example:
+    Examplo:
     * Imprime os dados no StdOut (Tela)
-        abin get --app api-auth --env dev --proj simlabs --no-file
+        abin get --app api-auth --env dev --proj sim --no-file
     * Imprime os dados em arquivo (Com base no arquivo $HOME/abin/settings.toml)
-        abin get --app api-auth --env dev --proj simlabs
+        abin get --app api-auth --env dev --proj sim
 
 ### UPDATE
-    Usage: abin update [OPTIONS] 
+    Uso: abin update [OPTIONS] 
                                                
     ╭─ Options─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app         TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None]  [required]                                        │
     │ *  --env         TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                │
-    │ *  --proj        TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required]  │
+    │ *  --proj        TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua) [default: None] [required]      │
     │    --secret      TEXT  Secret que será atualizada no Vault (Ex.: env, gcp.json, config.yaml ...) [default: env]                              │
     │ *  --file        TEXT  Arquivo com variárias de ambiente [default: None] [required]                                                          │
     │    --help              Show this message and exit.                                                                                           │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
-    For example:
-        abin update --app api-auth --env dev --proj simlabs --file .env  (para atualizar outro secret use --secret NOME)
+    Eexamplo:
+        abin update --app api-auth --env dev --proj sim --file .env  (para atualizar outro secret use --secret NOME)
 
 ### COMPARE
-    Usage: abin compare [OPTIONS]
+    Uso: abin compare [OPTIONS]
 
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                            │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                   │
-    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required]     │
+    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua) [default: None] [required]         │
     │    --help                       Show this message and exit.                                                                                              │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
-    For example:
-        abin compare --app api-auth --env qa,dev --proj simlabs
+    Eexamplo:
+        abin compare --app api-auth --env qa,dev --proj sim
```

### Comparing `abin_sim-1.0.0/abin_sim/cli.py` & `abin_sim-1.1.0/abin_sim/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from rich.console import Console
 from rich.table import Table
+from rich.tree import Tree
 from typer import Context, Exit, Option, Typer
 
 from abin_sim import __version__
 
 from .config import settings
 from .core.file_manager import make_return
 from .core.functions import (
     convert_to_json,
+    get_environment,
     get_metadata,
     get_secret,
     make_conf,
     update_secret,
 )
 
 console = Console()
@@ -40,43 +42,47 @@
     configure: bool = Option(False, callback=conf_func, is_flag=True),
 ):
     message = """
 [b]ABIN[/] - SIM Tech Solutions
 
 Forma de uso: [b]abin [SUBCOMANDO] [ARGUMENTOS][/]
 
-Existem 3 subcomandos disponíveis para essa aplicação
+Existem 4 subcomandos disponíveis para essa aplicação
 
+- [b]list[/]: Fornece, em tela, uma árvore com todas as aplicações e ambientes cadastrados no Vault
 - [b]get[/]: Fornece os secrets cadastrados em uma aplicação. Este retorno pode ser em tela ou arquivo
 - [b]update[/]: Envia uma nova coleção de ENV para uma determinada aplicação [red](Uso restrito, somente TL e SRE)[/]
 - [b]compare[/]: Compara o ENV de uma aplicação em 2 ambientes
 
 [b]Exemplos de uso:[/]
+ [b][blue]LIST[/][/]
+    [green][b]abin[/][/] [b]list[/]
+
  [b][blue]GET[/][/]
-    [green][b]abin[/][/] [b]get[/] --app api-auth --env dev --proj simlabs [magenta](para retorno em tela use [green][b]--no-file[/][/])[/]
+    [green][b]abin[/][/] [b]get[/] --app api-auth --env dev --proj sim [magenta](para retorno em tela use [green][b]--no-file[/][/])[/]
 
  [b][blue]UPDATE[/][/]
-    [green][b]abin[/][/] [b]update[/] --app api-auth --env dev --proj simlabs --file .env [magenta](para atualizar outro secret use [green][b]--secret NOME[/][/])[/]
+    [green][b]abin[/][/] [b]update[/] --app api-auth --env dev --proj sim --file .env [magenta](para atualizar outro secret use [green][b]--secret NOME[/][/])[/]
 
  [b][blue]COMPARE[/][/]
-    [green][b]abin[/][/] [b]compare[/] --app api-auth --env qa,dev --proj simlabs
+    [green][b]abin[/][/] [b]compare[/] --app api-auth --env qa,dev --proj sim
 
 ---
 [b]Help:[/]
  [b]Para mais informações[/]
     [green][b]abin[/][/] --help
 
  [b]Para ver a versão instalada[/]
     [green][b]abin[/][/] --version
 
  [b]Para gerar o arquivo de configuração[/]
     [green][b]abin[/][/] --configure
 
  [b]Para informações detalhadas
-    [blue][link=https://github.com/SIM-Rede/abin-sim/tree/main]Repo no GIT SIM[/]
+    [blue][link=https://github.com/SIM-Rede/abin-sim/tree/main]Repo no GIT SIM[/][/] | [blue][link=https://pypi.org/project/abin-sim/]Publicação no PyPI[/][/]
 """
     if ctx.invoked_subcommand:
         return
     console.print(message)
 
 @app.command('get')
 def get(
@@ -86,15 +92,15 @@
     ),
     env: str = Option(
         ...,
         help='Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main).'
     ),
     proj: str = Option(
         ...,
-        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua)'
+        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua)'
     ),
     file: bool = Option(
         True,
         help='Cria um arquivo .env para armazenar os secrets.',
     ),
 ):
     vault_token = settings.params.vault_token
@@ -128,15 +134,15 @@
     ),
     env: str = Option(
         ...,
         help='Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main).'
     ),
     proj: str = Option(
         ...,
-        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua)'
+        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua)'
     ),
     secret: str = Option(
         default='env',
         help='Secret que será atualizada no Vault (Ex.: env, gcp.json, config.yaml ...)',
     ),
     file: str = Option(
         ...,
@@ -148,27 +154,47 @@
     if secret == 'env':
         payload = convert_to_json(file)
     else:
         payload = file
     ret = update_secret(app, env, proj, secret, vault_token, vault_url, payload)
     console.print(ret)
 
+@app.command('list')
+def list():
+    vault_environment = get_environment(settings.params.vault_token, settings.params.vault_url)
+    console.print('''
+╭─ [i]Referênvia[/i] ──────────────────────╮
+
+    [b][cyan]Vault Environment:[/b][/]
+        ├── [blue](env)-(proj)[/]
+        │    ├── [green](api)[/]
+
+╰─ [i]Referênvia[/i] ──────────────────────╯
+    ''')
+    tree = Tree('[cyan][b]Vault Environment[/b][/]')
+    for k, v in vault_environment.items():
+        kv = tree.add(f'[blue]{k}')
+        for value in v:
+            kv.add(f'[green]{value}') 
+    
+    console.print(tree)
+
 @app.command('compare')
 def compare(
     app: str = Option(
         ...,
         help='Nome da aplicação que deseja recuperar os secrets.',
     ),
     env: str = Option(
         ...,
         help='Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main).'
     ),
     proj: str = Option(
         ...,
-        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua)'
+        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua)'
     ),
 ):
     # envs = []
     envs_a = []
     envs_b = []
     envs = env.split(',')
     if len(envs) == 2:
```

### Comparing `abin_sim-1.0.0/abin_sim/core/file_manager.py` & `abin_sim-1.1.0/abin_sim/core/file_manager.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.0.0/abin_sim/core/functions.py` & `abin_sim-1.1.0/abin_sim/core/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 def convert_to_json(
     file: str,
 ) -> dict:
     with open(file, 'r') as f:
         content = f.readlines()
 
-    contentList = [x.strip().split('#')[0].split('=', 1) for x in content if '=' in x.split('#')[0]]
+    contentList = [x.strip().split('^#')[0].split('=', 1) for x in content if '=' in x.split('^#')[0]]
     contentDict = dict(contentList)
     for k, v in contentList:
         for i, x in enumerate(v.split('$')[1:]):
             key = re.findall(r'\w+', x)[0]
             v = v.replace('$' + key, contentDict[key])
         contentDict[k] = v.strip()
 
@@ -130,15 +130,45 @@
 def make_conf() -> dict:
     home_dir = environ['HOME']
     try:
         path = Path(home_dir) / 'abin'
         path.mkdir()
         arq_conf = open(f'{path}/settings.toml', 'w')
     except Exception as e:
-        erro = f'Arquivo de configuração já criado ou pasta já existe em {home_dir}.\n Comando retornorou {e}'
+        erro = f'Arquivo de configuração já criado ou pasta já existe em {home_dir}.\n Comando retornou {e}'
         retorno = {'Message': erro, 'Status': False}
     else:
         arq_conf.write('name = "ABIN"\n\n[params]\nvault_token = "ALTERAR"\nvault_url = "https://aspirina.simtech.solutions"\npath = "./"\n\n[console]\ntable_width = 40')
         arq_conf.close()
         retorno = {'Message': f'Arquivo de configuração criado em {path}', 'Status': False}
     return retorno
 
+def get_environment(
+    token: str,
+    vault_url: str,
+) -> dict:
+    headers = {'X-Vault-Token': token }
+    try:
+        mounts = requests.request('GET', url=vault_url + '/v1/sys/mounts', headers=headers)
+    except Exception as e:
+        retorno = {'Status': f'Erro: {e}'}
+    
+    if mounts.status_code == 200:
+        search = ['local', 'dev', 'qa', 'main']
+        matches = []
+
+        for k, v in mounts.json().items():
+            if any([x in k for x in search]):
+                matches.append(k)
+        matches.sort()
+
+        paths_metadata = {}
+        for path in matches:
+            paths_response = requests.request('LIST', url=f'https://aspirina.simtech.solutions/v1/{path}metadata', headers=headers)
+            if paths_response.status_code == 200:
+                paths_metadata[path] = paths_response.json()['data']['keys']
+            
+        retorno = paths_metadata
+    else:
+        retorno = {'Status': f'Erro: {mounts.text}'}
+    
+    return retorno
```

### Comparing `abin_sim-1.0.0/pyproject.toml` & `abin_sim-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "1.0.0"
+version = "1.1.0"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-1.0.0/PKG-INFO` & `abin_sim-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 1.0.0
+Version: 1.1.0
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -78,54 +78,73 @@
 
     Retorna uma breve explicação sobre a funcionalidade do CLI.
     Traz exemplos de uso e link para projeto no GitHub
 
 ### VERSION
     Uso: abin --version
 
+    Retorna a versão atualmente instalada no SO.
+    Para atualizá-la:
+
+    pipx upgrade abin_sim
+
 ### CONFIGURE
     Uso: abin --configure
-   
+
+    Gera o arquivo de configuração da aplicação.
+
+## LIST
+    Uso: abin list
+
+    Retorna a árvore de Secrets cadastradas no Path obedecendo a referência abaixp
+    ╭─ Referênvia ──────────────────╮
+    │                               │ 
+    │ Vault Environment:            │
+    │     ├── (env)-(proj)          │
+    │     │    ├── (api)            │
+    │                               │
+    ╰─ Referênvia ──────────────────╯
+
 ### GET
-    Usage: abin get [OPTIONS]                                                                                                                            
+    Uso: abin get [OPTIONS]                                                                                                                            
                                                                                                                                                       
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                        │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]               │
-    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required] │
+    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua) [default: None] [required]     │
     │    --file    --no-file          Cria um arquivo para cada path cadastrada no secrets. [default: file]                                                │
     │    --help                       Show this message and exit.                                                                                          │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
-    For example:
+    Examplo:
     * Imprime os dados no StdOut (Tela)
-        abin get --app api-auth --env dev --proj simlabs --no-file
+        abin get --app api-auth --env dev --proj sim --no-file
     * Imprime os dados em arquivo (Com base no arquivo $HOME/abin/settings.toml)
-        abin get --app api-auth --env dev --proj simlabs
+        abin get --app api-auth --env dev --proj sim
 
 ### UPDATE
-    Usage: abin update [OPTIONS] 
+    Uso: abin update [OPTIONS] 
                                                
     ╭─ Options─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app         TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None]  [required]                                        │
     │ *  --env         TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                │
-    │ *  --proj        TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required]  │
+    │ *  --proj        TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua) [default: None] [required]      │
     │    --secret      TEXT  Secret que será atualizada no Vault (Ex.: env, gcp.json, config.yaml ...) [default: env]                              │
     │ *  --file        TEXT  Arquivo com variárias de ambiente [default: None] [required]                                                          │
     │    --help              Show this message and exit.                                                                                           │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
-    For example:
-        abin update --app api-auth --env dev --proj simlabs --file .env  (para atualizar outro secret use --secret NOME)
+    Eexamplo:
+        abin update --app api-auth --env dev --proj sim --file .env  (para atualizar outro secret use --secret NOME)
 
 ### COMPARE
-    Usage: abin compare [OPTIONS]
+    Uso: abin compare [OPTIONS]
 
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                            │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]                   │
-    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: simlabs, charrua) [default: None] [required]     │
+    │ *  --proj                 TEXT  Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua) [default: None] [required]         │
     │    --help                       Show this message and exit.                                                                                              │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
-    For example:
-        abin compare --app api-auth --env qa,dev --proj simlabs
+    Eexamplo:
+        abin compare --app api-auth --env qa,dev --proj sim
```

