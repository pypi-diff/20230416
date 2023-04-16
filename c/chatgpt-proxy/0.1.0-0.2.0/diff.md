# Comparing `tmp/chatgpt-proxy-0.1.0.tar.gz` & `tmp/chatgpt-proxy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-proxy-0.1.0.tar", last modified: Wed Apr 12 14:33:41 2023, max compression
+gzip compressed data, was "chatgpt-proxy-0.2.0.tar", last modified: Sun Apr 16 05:27:04 2023, max compression
```

## Comparing `chatgpt-proxy-0.1.0.tar` & `chatgpt-proxy-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/chatgpt_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/chatgpt_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/chatgpt_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/chatgpt_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/chatgpt_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/chatgpt_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/chatgpt_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/chatgpt_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/setup.cfg
```

### Comparing `chatgpt-proxy-0.1.0/LICENSE` & `chatgpt-proxy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.1.0/PKG-INFO` & `chatgpt-proxy-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,83 @@
-Metadata-Version: 2.1
-Name: chatgpt-proxy
-Version: 0.1.0
-Summary: Reverse proxy for OpenAI chatgpt website API
-Author: 18870
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChatGPT-Proxy
 Python version of OpenAI's ChatGPT web API proxy  
-Python alternative to [ChatGPT-Proxy-V4](https://github.com/acheong08/ChatGPT-Proxy-V4)  
-Use cookie `_puid` to bypass Cloudflare browser check  
+Python alternative of [ChatGPT-Proxy-V4](https://github.com/acheong08/ChatGPT-Proxy-V4)  
+Use cookie `cf_clearance` to pass Cloudflare browser check  
+
+**`_puid` no longer works**
 
 ## Requirements
-- ChatGPT plus account
 - Access to chat.openai.com
 
 ## Install
 `pip install chatgpt-proxy`
 
 ## Usage
 ### Run as a service
 Set these environment variables:
-- `PUID`: Preset cookie `_puid`
-- `ACCESS_TOKEN`: (Optional) For automatic refresh of `_puid`, obtains from [here](https://chat.openai.com/api/auth/session)
+- `CF_CLEARANCE`: Cookie `cf_clearance`
+- `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
+- `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
-puid=YOUR_PUID
+cf_clearance=YOUR_CF_CLEARANCE
+user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
 ```
 
 Note that environment variables will override the values in `.env` file.
 
-Then run: `python -m chatgpt_proxy`
-The proxy will be avaliable at `http://host:port/backend-api/`
+Then run: `python -m chatgpt_proxy`  
+
+#### Success
+If you see this in console:
+`2023-01-01 00:00:00,000 - chatgpt_proxy.proxy - INFO - puid: user-xxxxxx`
+You are ready to go
+
+The proxy is avaliable at `http://host:port/backend-api/`
 
 ### Integrate into your FastAPI app
 Check out [\_\_main__.py](./chatgpt_proxy/__main__.py)
 ```python
 from chatgpt_proxy import WebChatGPTProxy
-proxy = WebChatGPTProxy(puid=PUID, access_token=ACCESS_TOKEN, trust=False)
-
-@asynccontextmanager
-async def lifespan(app: FastAPI):
-    # add this to start refresh puid task
-    refresh_puid_task = asyncio.create_task(proxy._refresh_task())
-    yield
-
-app = FastAPI(lifespan=lifespan)
+proxy = WebChatGPTProxy(cf_clearance=CF_CLEARANCE, user_agent=USER_AGENT, access_token=ACCESS_TOKEN, trust=False)
+app = FastAPI()
 proxy.attach(app, path="/backend-api")
 ```
 
 class `WebChatGPTProxy`:
-- `puid`: Preset cookie `_puid`
-- `access_token`: (Optional), for automatic refresh of `_puid`
-- `trust`: Trust requests from any client.
+- `cf_clearance`: Cookie `cf_clearance`
+- `user_agent`: User-agent of your browser when you get the cookie `cf_clearance`
+- `access_token`: (Optional)
+- `trust`: (Optional) Trust requests from any client.
     When set to True, any requests without an access_token will be given the above access_token.
     Default to False, which will only use for refresh puid.
 
+### Behind a http proxy
+**You need to use the same ip address you used to get the cookie `cf_clearance`**
+
+Set `HTTP_PROXY` and `HTTPS_PROXY` or `ALL_PROXY` environment variables.   
+This **cannot be set** in `.env` file becauce `httpx` (the package we used to send request) reads from environment variables only. See also [httpx#Proxies](https://www.python-httpx.org/environment_variables/#http_proxy-https_proxy-all_proxy).
 
 ## Credits
 - ChatGPT-Proxy-V4
 https://github.com/acheong08/ChatGPT-Proxy-V4
 - Implement reverse proxy in FastAPI
 https://github.com/tiangolo/fastapi/discussions/7382#discussioncomment-5136454
 
 ## License
 This work is licensed under the [GNU Affero General Public License v3.0](/LICENSE) or later, with the "CHATGPT-PROXY" exception.
 
 > **"CHATGPT-PROXY" EXCEPTION TO THE AGPL**
 >
 > As a special exception, using this work in the following ways does not cause your program to be covered by the AGPL:
 > 1. Bundling the unaltered code or binary of this work in your program; or
-> 2. Interacting with this work through the provided inter-process communication interface, such as the HTTP API.
+> 2. Interacting with this work through the provided inter-process communication interface, such as the HTTP API.
```

### Comparing `chatgpt-proxy-0.1.0/chatgpt_proxy/__main__.py` & `chatgpt-proxy-0.2.0/chatgpt_proxy/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,28 +13,31 @@
     level=logging.INFO,
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     handlers=[logging.StreamHandler()],
 )
 
 
 class Settings(BaseSettings):
-    puid: str
+    cf_clearance: str
+    user_agent: str
+
     access_token: str = None
     host: str = "127.0.0.1"
     port: int = 7800
     trust: bool = Field(default=False, env="proxy_trust_client")
 
     class Config:
         env_file = '.env'
 
 
 if __name__ == "__main__":
     env = Settings()
     proxy = WebChatGPTProxy(
-        puid=env.puid,
+        cf_clearance=env.cf_clearance,
+        user_agent=env.user_agent,
         access_token=env.access_token,
         trust=env.trust,
     )
 
     @asynccontextmanager
     async def lifespan(app: FastAPI):
         refresh_puid_task = asyncio.create_task(proxy._refresh_task())
```

### Comparing `chatgpt-proxy-0.1.0/chatgpt_proxy/proxy.py` & `chatgpt-proxy-0.2.0/chatgpt_proxy/proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,79 +98,80 @@
             description=f"Reverse proxy of {self.base_url}",
             **kwargs,
         )
 
 
 class WebChatGPTProxy(ReverseProxy):
     def __init__(
-        self, puid: str, access_token: Optional[str] = None, trust: bool = False
+        self, cf_clearance: str, user_agent: str, access_token: Optional[str] = None, trust: bool = False
     ) -> None:
         """
         :param puid: from `_puid` cookie
         :param access_token: from openai `access_token`
                              obtained from here https://chat.openai.com/api/auth/session
                              Used to refresh puid
         :param trust: Trust requests from any client.
                       When set to True, any requests without an access_token will be given the above access_token.
                       Default to False, which will only use for refresh puid.
         """
         super().__init__(base_url="https://chat.openai.com/backend-api/")
-        self.puid = puid
+        self.cf_clearance = cf_clearance
+        self.ua = user_agent
         self.access_token = access_token
         self.trust = trust
         self._app: Optional[FastAPI] = None
         self._path: Optional[str] = None
 
     async def _prepare_cookies(self, request: Request):
         cookies = await super()._prepare_cookies(request)
-        cookies.setdefault("_puid", self.puid)
+        cookies.setdefault("cf_clearance", self.cf_clearance)
         return cookies
 
     async def _prepare_headers(self, request: Request):
         headers = await super()._prepare_headers(request)
         headers["origin"] = "https://chat.openai.com"
         headers["referer"] = "https://chat.openai.com/chat"
-        headers[
-            "user-agent"
-        ] = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.54"
+        headers["user-agent"] = self.ua
         if self.trust and self.access_token:
             headers.setdefault("authorization", f"Bearer {self.access_token}")
         return headers
 
     async def _refresh_puid(self) -> None:
         """
         Send requests to /models through reverse proxy (current FastAPI app) to get a new puid
+        
+        Use to see if you pass cloudflare
         """
         if self._app is None:
-            logger.info("Not attached to any FastAPI app, skip refresh")
+            logger.info("Not attached to any FastAPI app, skip")
         async with httpx.AsyncClient(
             app=self._app, base_url=f"https://chat.openai.com{self._path}"
         ) as client:
             resp = await client.get(
                 "/models", headers={"authorization": f"Bearer {self.access_token}"}
             )
             puid = resp.cookies.get("_puid")
             if puid:
                 logger.info(f"puid: {puid}")
                 self.puid = puid
             else:
-                logger.error("Failed to refresh puid")
+                logger.error("Failed to get puid")
                 logger.error(f"Cookies: {resp.cookies}")
                 logger.error(f"Response: \n{resp.text}")
 
     async def _refresh_task(self) -> None:
         if self.access_token is None:
-            logger.info("access_token not found, skip refresh")
+            logger.info("access_token not found, skip")
             return
-        while True:
-            try:
-                await self._refresh_puid()
-            except Exception as e:
-                logger.exception(e)
-                await asyncio.sleep(60 * 60)
-                continue
-            await asyncio.sleep(60 * 60 * 6)
+
+        try:
+            await self._refresh_puid()
+        except Exception as e:
+            logger.exception(e)
+            # await asyncio.sleep(60 * 60)
+            # continue
+        # await asyncio.sleep(60 * 60 * 6)
 
     def attach(self, app: FastAPI, path: str) -> None:
         super().attach(app=app, path=path, include_in_schema=self.trust)
         self._app = app
         self._path = path
```

### Comparing `chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/PKG-INFO` & `chatgpt-proxy-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,85 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT-Proxy
 Python version of OpenAI's ChatGPT web API proxy  
-Python alternative to [ChatGPT-Proxy-V4](https://github.com/acheong08/ChatGPT-Proxy-V4)  
-Use cookie `_puid` to bypass Cloudflare browser check  
+Python alternative of [ChatGPT-Proxy-V4](https://github.com/acheong08/ChatGPT-Proxy-V4)  
+Use cookie `cf_clearance` to pass Cloudflare browser check  
+
+**`_puid` no longer works**
 
 ## Requirements
-- ChatGPT plus account
 - Access to chat.openai.com
 
 ## Install
 `pip install chatgpt-proxy`
 
 ## Usage
 ### Run as a service
 Set these environment variables:
-- `PUID`: Preset cookie `_puid`
-- `ACCESS_TOKEN`: (Optional) For automatic refresh of `_puid`, obtains from [here](https://chat.openai.com/api/auth/session)
+- `CF_CLEARANCE`: Cookie `cf_clearance`
+- `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
+- `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
-puid=YOUR_PUID
+cf_clearance=YOUR_CF_CLEARANCE
+user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
 ```
 
 Note that environment variables will override the values in `.env` file.
 
-Then run: `python -m chatgpt_proxy`
-The proxy will be avaliable at `http://host:port/backend-api/`
+Then run: `python -m chatgpt_proxy`  
+
+#### Success
+If you see this in console:
+`2023-01-01 00:00:00,000 - chatgpt_proxy.proxy - INFO - puid: user-xxxxxx`
+You are ready to go
+
+The proxy is avaliable at `http://host:port/backend-api/`
 
 ### Integrate into your FastAPI app
 Check out [\_\_main__.py](./chatgpt_proxy/__main__.py)
 ```python
 from chatgpt_proxy import WebChatGPTProxy
-proxy = WebChatGPTProxy(puid=PUID, access_token=ACCESS_TOKEN, trust=False)
-
-@asynccontextmanager
-async def lifespan(app: FastAPI):
-    # add this to start refresh puid task
-    refresh_puid_task = asyncio.create_task(proxy._refresh_task())
-    yield
-
-app = FastAPI(lifespan=lifespan)
+proxy = WebChatGPTProxy(cf_clearance=CF_CLEARANCE, user_agent=USER_AGENT, access_token=ACCESS_TOKEN, trust=False)
+app = FastAPI()
 proxy.attach(app, path="/backend-api")
 ```
 
 class `WebChatGPTProxy`:
-- `puid`: Preset cookie `_puid`
-- `access_token`: (Optional), for automatic refresh of `_puid`
-- `trust`: Trust requests from any client.
+- `cf_clearance`: Cookie `cf_clearance`
+- `user_agent`: User-agent of your browser when you get the cookie `cf_clearance`
+- `access_token`: (Optional)
+- `trust`: (Optional) Trust requests from any client.
     When set to True, any requests without an access_token will be given the above access_token.
     Default to False, which will only use for refresh puid.
 
+### Behind a http proxy
+**You need to use the same ip address you used to get the cookie `cf_clearance`**
+
+Set `HTTP_PROXY` and `HTTPS_PROXY` or `ALL_PROXY` environment variables.   
+This **cannot be set** in `.env` file becauce `httpx` (the package we used to send request) reads from environment variables only. See also [httpx#Proxies](https://www.python-httpx.org/environment_variables/#http_proxy-https_proxy-all_proxy).
 
 ## Credits
 - ChatGPT-Proxy-V4
 https://github.com/acheong08/ChatGPT-Proxy-V4
 - Implement reverse proxy in FastAPI
 https://github.com/tiangolo/fastapi/discussions/7382#discussioncomment-5136454
```

