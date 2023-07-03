# Comparing `tmp/abin_sim-1.1.0.tar.gz` & `tmp/abin_sim-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-1.1.0.tar", max compression
+gzip compressed data, was "abin_sim-1.1.1.tar", max compression
```

## Comparing `abin_sim-1.1.0.tar` & `abin_sim-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-07-03 12:52:48.616804 abin_sim-1.1.0/LICENSE
--rw-r--r--   0        0        0     8593 2023-07-03 12:52:48.616804 abin_sim-1.1.0/README.md
--rw-r--r--   0        0        0       21 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/config.py
--rw-r--r--   0        0        0     1174 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     5320 2023-07-03 12:52:48.616804 abin_sim-1.1.0/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-07-03 12:52:48.616804 abin_sim-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9482 1970-01-01 00:00:00.000000 abin_sim-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-07-03 20:07:56.409411 abin_sim-1.1.1/LICENSE
+-rw-r--r--   0        0        0     8594 2023-07-03 20:07:56.409411 abin_sim-1.1.1/README.md
+-rw-r--r--   0        0        0       21 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/config.py
+-rw-r--r--   0        0        0     1174 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     5320 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-07-03 20:07:56.409411 abin_sim-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.1.1/PKG-INFO
```

### Comparing `abin_sim-1.1.0/README.md` & `abin_sim-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 
 ## Instalação
 
 Utilize o pipx para instalar o abin no seu computador.
 ```
 sudo apt install pipx
 pipx install abin_sim
-
 ```
 A versão da aplicação no README será atualizada sempre que um novo build rodar.
 
 Se você estiver rodando no PopOS precisa criar um link simbólico para a aplicação ou adicionar $HOME/.local/bin no path do SO
 ```
 sudo ln -s $HOME/.local/bin/abin /usr/local/bin/abin
 ```
 
 
 ## Configuração
 
 Após realizar a instalação do App, será necessário iniciar o arquivo de configuração
 Para isso execute a instrução abaixo:
 ```
-abin make-conf
+abin --configure
 ```
 
 A instrução acima criará um arquivo chamado 'settings.toml' em $HOME/abin/
 Com o arquivo em mãos, altere o valor de **vault_token** para o seu token, o valor deverá focar entre " "
 
 *vault_token* -> Seu token de autenticação no Vault
 
@@ -69,21 +68,21 @@
 
     Gera o arquivo de configuração da aplicação.
 
 ## LIST
     Uso: abin list
 
     Retorna a árvore de Secrets cadastradas no Path obedecendo a referência abaixp
-    ╭─ Referênvia ──────────────────╮
+    ╭─ Referência ──────────────────╮
     │                               │ 
     │ Vault Environment:            │
     │     ├── (env)-(proj)          │
     │     │    ├── (api)            │
     │                               │
-    ╰─ Referênvia ──────────────────╯
+    ╰─ Referência ──────────────────╯
 
 ### GET
     Uso: abin get [OPTIONS]                                                                                                                            
                                                                                                                                                       
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                        │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]               │
```

### Comparing `abin_sim-1.1.0/abin_sim/cli.py` & `abin_sim-1.1.1/abin_sim/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,21 +158,21 @@
     ret = update_secret(app, env, proj, secret, vault_token, vault_url, payload)
     console.print(ret)
 
 @app.command('list')
 def list():
     vault_environment = get_environment(settings.params.vault_token, settings.params.vault_url)
     console.print('''
-╭─ [i]Referênvia[/i] ──────────────────────╮
+╭─ [i]Referência[/i] ──────────────────────╮
 
     [b][cyan]Vault Environment:[/b][/]
         ├── [blue](env)-(proj)[/]
         │    ├── [green](api)[/]
 
-╰─ [i]Referênvia[/i] ──────────────────────╯
+╰─ [i]Referência[/i] ──────────────────────╯
     ''')
     tree = Tree('[cyan][b]Vault Environment[/b][/]')
     for k, v in vault_environment.items():
         kv = tree.add(f'[blue]{k}')
         for value in v:
             kv.add(f'[green]{value}')
```

### Comparing `abin_sim-1.1.0/abin_sim/core/file_manager.py` & `abin_sim-1.1.1/abin_sim/core/file_manager.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.0/abin_sim/core/functions.py` & `abin_sim-1.1.1/abin_sim/core/functions.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.0/pyproject.toml` & `abin_sim-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "1.1.0"
+version = "1.1.1"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-1.1.0/PKG-INFO` & `abin_sim-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 1.1.0
+Version: 1.1.1
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -27,30 +27,29 @@
 
 ## Instalação
 
 Utilize o pipx para instalar o abin no seu computador.
 ```
 sudo apt install pipx
 pipx install abin_sim
-
 ```
 A versão da aplicação no README será atualizada sempre que um novo build rodar.
 
 Se você estiver rodando no PopOS precisa criar um link simbólico para a aplicação ou adicionar $HOME/.local/bin no path do SO
 ```
 sudo ln -s $HOME/.local/bin/abin /usr/local/bin/abin
 ```
 
 
 ## Configuração
 
 Após realizar a instalação do App, será necessário iniciar o arquivo de configuração
 Para isso execute a instrução abaixo:
 ```
-abin make-conf
+abin --configure
 ```
 
 A instrução acima criará um arquivo chamado 'settings.toml' em $HOME/abin/
 Com o arquivo em mãos, altere o valor de **vault_token** para o seu token, o valor deverá focar entre " "
 
 *vault_token* -> Seu token de autenticação no Vault
 
@@ -92,21 +91,21 @@
 
     Gera o arquivo de configuração da aplicação.
 
 ## LIST
     Uso: abin list
 
     Retorna a árvore de Secrets cadastradas no Path obedecendo a referência abaixp
-    ╭─ Referênvia ──────────────────╮
+    ╭─ Referência ──────────────────╮
     │                               │ 
     │ Vault Environment:            │
     │     ├── (env)-(proj)          │
     │     │    ├── (api)            │
     │                               │
-    ╰─ Referênvia ──────────────────╯
+    ╰─ Referência ──────────────────╯
 
 ### GET
     Uso: abin get [OPTIONS]                                                                                                                            
                                                                                                                                                       
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app                  TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None] [required]                                        │
     │ *  --env                  TEXT  Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main). [default: None] [required]               │
```

