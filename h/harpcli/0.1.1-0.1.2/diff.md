# Comparing `tmp/harpcli-0.1.1.tar.gz` & `tmp/harpcli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpcli-0.1.1.tar", last modified: Tue Jun 20 20:03:54 2023, max compression
+gzip compressed data, was "harpcli-0.1.2.tar", last modified: Mon Jul  3 19:46:55 2023, max compression
```

## Comparing `harpcli-0.1.1.tar` & `harpcli-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mnida      (501) staff       (20)        0 2023-06-20 20:03:54.223087 harpcli-0.1.1/
--rw-r--r--   0 mnida      (501) staff       (20)      111 2023-06-20 20:03:54.222889 harpcli-0.1.1/PKG-INFO
-drwxr-xr-x   0 mnida      (501) staff       (20)        0 2023-06-20 20:03:54.222607 harpcli-0.1.1/harpcli.egg-info/
--rw-r--r--   0 mnida      (501) staff       (20)      111 2023-06-20 20:03:54.000000 harpcli-0.1.1/harpcli.egg-info/PKG-INFO
--rw-r--r--   0 mnida      (501) staff       (20)      234 2023-06-20 20:03:54.000000 harpcli-0.1.1/harpcli.egg-info/SOURCES.txt
--rw-r--r--   0 mnida      (501) staff       (20)        1 2023-06-20 20:03:54.000000 harpcli-0.1.1/harpcli.egg-info/dependency_links.txt
--rw-r--r--   0 mnida      (501) staff       (20)       34 2023-06-20 20:03:54.000000 harpcli-0.1.1/harpcli.egg-info/entry_points.txt
--rw-r--r--   0 mnida      (501) staff       (20)        1 2023-06-20 17:05:10.000000 harpcli-0.1.1/harpcli.egg-info/not-zip-safe
--rw-r--r--   0 mnida      (501) staff       (20)       15 2023-06-20 20:03:54.000000 harpcli-0.1.1/harpcli.egg-info/requires.txt
--rw-r--r--   0 mnida      (501) staff       (20)        5 2023-06-20 20:03:54.000000 harpcli-0.1.1/harpcli.egg-info/top_level.txt
--rw-r--r--   0 mnida      (501) staff       (20)     3327 2023-06-20 19:54:57.000000 harpcli-0.1.1/main.py
--rw-r--r--   0 mnida      (501) staff       (20)       38 2023-06-20 20:03:54.223142 harpcli-0.1.1/setup.cfg
--rw-r--r--   0 mnida      (501) staff       (20)      464 2023-06-20 20:02:18.000000 harpcli-0.1.1/setup.py
+drwxr-xr-x   0 mnida      (501) staff       (20)        0 2023-07-03 19:46:55.917133 harpcli-0.1.2/
+-rw-r--r--   0 mnida      (501) staff       (20)      111 2023-07-03 19:46:55.916947 harpcli-0.1.2/PKG-INFO
+drwxr-xr-x   0 mnida      (501) staff       (20)        0 2023-07-03 19:46:55.916705 harpcli-0.1.2/harpcli.egg-info/
+-rw-r--r--   0 mnida      (501) staff       (20)      111 2023-07-03 19:46:55.000000 harpcli-0.1.2/harpcli.egg-info/PKG-INFO
+-rw-r--r--   0 mnida      (501) staff       (20)      234 2023-07-03 19:46:55.000000 harpcli-0.1.2/harpcli.egg-info/SOURCES.txt
+-rw-r--r--   0 mnida      (501) staff       (20)        1 2023-07-03 19:46:55.000000 harpcli-0.1.2/harpcli.egg-info/dependency_links.txt
+-rw-r--r--   0 mnida      (501) staff       (20)       34 2023-07-03 19:46:55.000000 harpcli-0.1.2/harpcli.egg-info/entry_points.txt
+-rw-r--r--   0 mnida      (501) staff       (20)        1 2023-06-20 17:05:10.000000 harpcli-0.1.2/harpcli.egg-info/not-zip-safe
+-rw-r--r--   0 mnida      (501) staff       (20)       15 2023-07-03 19:46:55.000000 harpcli-0.1.2/harpcli.egg-info/requires.txt
+-rw-r--r--   0 mnida      (501) staff       (20)        5 2023-07-03 19:46:55.000000 harpcli-0.1.2/harpcli.egg-info/top_level.txt
+-rw-r--r--   0 mnida      (501) staff       (20)     5026 2023-07-03 19:36:00.000000 harpcli-0.1.2/main.py
+-rw-r--r--   0 mnida      (501) staff       (20)       38 2023-07-03 19:46:55.917188 harpcli-0.1.2/setup.cfg
+-rw-r--r--   0 mnida      (501) staff       (20)      464 2023-07-03 19:46:20.000000 harpcli-0.1.2/setup.py
```

### Comparing `harpcli-0.1.1/main.py` & `harpcli-0.1.2/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,156 @@
 import os
 import webbrowser
-from typing import List
+from json import JSONDecodeError
+from typing import List, TypedDict
 from uuid import UUID
 
 import requests
 import typer
 
 app = typer.Typer()
 
-url_prefix = "v1/buyer"
-api_token = os.getenv("API_TOKEN", "")
+api_token = os.getenv("API_TOKEN")
 headers = {"Authorization": f"Bearer {api_token}"}
+ngrok_url = os.getenv("NGROK_URL", "https://api.useharp.com")
+
+
+def check_api_token():
+    if api_token is None:
+        typer.echo(
+            "API_TOKEN is not set. Please set your API token in the environment variables."
+        )
+        raise SystemExit
+
+
+class Product(TypedDict):
+    product_id: str
+    quantity: int
 
 
 @app.command()
 def add_payment_method():
+    check_api_token()
     typer.echo("Let's add a new payment method.")
 
     # Let's assume your FastAPI server is running locally on port 8000
-    fastapi_url = os.getenv("FASTAPI_URL", "http://localhost:8000")
+    fastapi_url = os.getenv("FASTAPI_URL", ngrok_url)
     ### Add prefix after localhost
-    fastapi_url = f"{fastapi_url}/{url_prefix}"
-
-    typer.echo(fastapi_url)
+    request_url = f"{fastapi_url}/v1/buyer/create-checkout-session"
 
     # Request to generate a new Stripe Payment Method
-    response = requests.post(f"{fastapi_url}/create-checkout-session", headers=headers)
+    response = requests.post(request_url, headers=headers)
     if response.status_code == 200:
         response_json = response.json()
 
         stripe_payment_url = response_json["data"]
 
         # Open the Stripe Checkout page
         webbrowser.open(stripe_payment_url)
 
         # Once the user completes the payment on the Stripe Checkout page, Stripe will redirect them to your specified return_url (you will need to set this up on your FastAPI backend).
         # On the return page, you can retrieve the PaymentMethod ID from the URL parameters and send it back to the FastAPI backend to associate it with the user and save it in the database.
     else:
         typer.echo(response.status_code)
-        typer.echo("Something went wrong. It was reported to the devs. Slack us if you need help.")
+        typer.echo(
+            "Something went wrong. It was reported to the devs. Slack us if you need help."
+        )
+
+
+@app.command()
+def seller_connect():
+    check_api_token()
+    typer.echo("Let's connect your shopify store to harp.")
+
+    # Let's assume your FastAPI server is running locally on port 8000
+    fastapi_url = os.getenv("FASTAPI_URL", ngrok_url)
+    ### Add prefix after localhost
+    request_url = f"{fastapi_url}/v1/seller/stores/register/shopify/redirect"
+
+    # Prompt user for shopify store name
+    store_name = None
+    while store_name is None:
+        store_id_str = typer.prompt("Enter the Shopify store name")
+        store_name = store_id_str
+
+    # build request body
+
+    request_body = {"shop_name": store_name, "origin_url": request_url}
+    response = requests.post(request_url, json=request_body, headers=headers)
+    if response.status_code == 200:
+        response_json = response.json()
+
+        auth_url = response_json["data"]["auth_url"]
+        typer.echo(auth_url)
+
+        # Open the Shopify Oauth connect
+        # webbrowser.open(auth_url)
+
+    else:
+        typer.echo(response.status_code)
+        typer.echo(
+            "Something went wrong. It was reported to the devs. Slack us if you need help."
+        )
 
 
 @app.command()
 def order():
+    check_api_token()
     typer.echo("Let's create a new order.")
 
     # Prompt user for each field
     store_id = None
+    store_id_str: str = ""
     while store_id is None:
-        store_id_str = typer.prompt("Enter the store_id")
+        store_id_str: str = typer.prompt("Enter the store_id")
         try:
             store_id = UUID(store_id_str)
         except ValueError:
             typer.echo("Invalid UUID format, please try again.")
-    products: List[dict] = []
+    products: List[Product] = []
 
     # Request the first product ID and quantity
     product_id = typer.prompt("Enter product id")
     quantity = int(typer.prompt(f"Enter quantity for product {product_id}"))
     products.append({"product_id": product_id, "quantity": quantity})
 
     # For the second and next products, give the option to quit
     while True:
-        product_id = typer.prompt("Enter next product id (or 'q' to quit)")
-        if product_id.lower() == "q":
+        product_id = typer.prompt("Enter next product id (or 'c' to complete order)")
+        if product_id.lower() == "c":
             break
         quantity = int(typer.prompt(f"Enter quantity for product {product_id}"))
         products.append({"product_id": product_id, "quantity": quantity})
 
     # If no products are added, print error message and exit
     if not products:
         typer.echo("You must order at least one product!")
         return
 
     # Let's assume your FastAPI server is running locally on port 8000
-    fastapi_url = os.getenv("FASTAPI_URL", "http://localhost:8000")
-    fastapi_url = f"{fastapi_url}/{url_prefix}"
+    fastapi_url = os.getenv("FASTAPI_URL", ngrok_url)
 
-    order_params = {"products": products, "store_id": store_id}
+    order_params = {"products": products, "store_id": store_id_str}
 
     # Send request to create new order
-    response = requests.post(f"{fastapi_url}/order", json=order_params, headers=headers)
+    request_url = f"{fastapi_url}/v1/buyer/orders"
+    response = requests.post(request_url, json=order_params, headers=headers)
 
     if response.status_code == 201:
         typer.echo("Order created successfully!")
     else:
         typer.echo(response.status_code)
-        typer.echo(response.json())
-        typer.echo("Something went wrong. It was reported to the devs. Slack us if you need help.")
+        try:
+            typer.echo(response.json())
+        except JSONDecodeError:
+            typer.echo(response)
+        typer.echo(
+            "Something went wrong. It was reported to the devs. Slack us if you need help."
+        )
 
 
 if __name__ == "__main__":
     app()
+
+
+# id: cba16cf7-ac5d-477f-8d09-828552ea0b14
+# name: 45322386931994
```

