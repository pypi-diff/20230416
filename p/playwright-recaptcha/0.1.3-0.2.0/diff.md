# Comparing `tmp/playwright-recaptcha-0.1.3.tar.gz` & `tmp/playwright-recaptcha-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright-recaptcha-0.1.3.tar", last modified: Sun Mar 19 19:17:46 2023, max compression
+gzip compressed data, was "playwright-recaptcha-0.2.0.tar", last modified: Sun Apr 16 21:45:00 2023, max compression
```

## Comparing `playwright-recaptcha-0.1.3.tar` & `playwright-recaptcha-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 19:17:46.280484 playwright-recaptcha-0.1.3/
--rw-rw-rw-   0        0        0     1082 2023-01-19 00:03:47.000000 playwright-recaptcha-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     7066 2023-03-19 19:17:46.279484 playwright-recaptcha-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6173 2023-03-19 19:01:52.000000 playwright-recaptcha-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-19 19:17:46.248487 playwright-recaptcha-0.1.3/playwright_recaptcha/
--rw-rw-rw-   0        0        0      840 2023-03-19 19:09:35.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/__init__.py
--rw-rw-rw-   0        0        0     1061 2023-03-19 19:02:25.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/errors.py
-drwxrwxrwx   0        0        0        0 2023-03-19 19:17:46.271484 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/
--rw-rw-rw-   0        0        0      226 2023-01-28 18:33:28.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/__init__.py
--rw-rw-rw-   0        0        0     8811 2023-03-14 02:03:38.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/async_solver.py
--rw-rw-rw-   0        0        0    16008 2023-02-19 05:29:07.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/recaptcha_box.py
--rw-rw-rw-   0        0        0     7961 2023-03-14 02:00:24.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/sync_solver.py
-drwxrwxrwx   0        0        0        0 2023-03-19 19:17:46.274484 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav3/
--rw-rw-rw-   0        0        0      226 2023-01-28 18:33:28.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav3/__init__.py
--rw-rw-rw-   0        0        0     3068 2023-03-19 19:02:35.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav3/async_solver.py
--rw-rw-rw-   0        0        0     3025 2023-03-19 19:02:14.000000 playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav3/sync_solver.py
-drwxrwxrwx   0        0        0        0 2023-03-19 19:17:46.266483 playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/
--rw-rw-rw-   0        0        0     7066 2023-03-19 19:17:46.000000 playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2023-03-19 19:17:46.000000 playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 19:17:46.000000 playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-03-19 19:17:46.000000 playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-19 19:17:46.000000 playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-19 19:17:46.280484 playwright-recaptcha-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1289 2023-03-19 19:17:16.000000 playwright-recaptcha-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-19 19:17:46.278484 playwright-recaptcha-0.1.3/tests/
--rw-rw-rw-   0        0        0     1792 2023-02-19 00:09:23.000000 playwright-recaptcha-0.1.3/tests/test_async_recaptchav2.py
--rw-rw-rw-   0        0        0     1548 2023-03-19 19:12:10.000000 playwright-recaptcha-0.1.3/tests/test_async_recaptchav3.py
--rw-rw-rw-   0        0        0     1594 2023-02-19 00:09:52.000000 playwright-recaptcha-0.1.3/tests/test_sync_recaptchav2.py
--rw-rw-rw-   0        0        0     1350 2023-03-19 19:12:18.000000 playwright-recaptcha-0.1.3/tests/test_sync_recaptchav3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.484198 playwright-recaptcha-0.2.0/playwright_recaptcha/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/recaptcha_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_async_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_async_recaptchav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_sync_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_sync_recaptchav3.py
```

### Comparing `playwright-recaptcha-0.1.3/LICENSE` & `playwright-recaptcha-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Xewdy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Xewdy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `playwright-recaptcha-0.1.3/PKG-INFO` & `playwright-recaptcha-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-Metadata-Version: 2.1
-Name: playwright-recaptcha
-Version: 0.1.3
-Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
-Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
-Author: Xewdy444
-Author-email: xewdy@xewdy.tech
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
-Classifier: Framework :: AsyncIO
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![PyPI](https://img.shields.io/pypi/v/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
-[![Downloads](https://img.shields.io/pypi/dm/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
-[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Xewdy444/Playwright-reCAPTCHA/blob/main/LICENSE)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-# Playwright-reCAPTCHA
-A Python library for solving reCAPTCHA v2 and v3 with Playwright.
-
-## Solving reCAPTCHA v2
-reCAPTCHA v2 is solved by transcribing the audio challenge using the Google speech recognition API and entering the text as the response.
-
-## Solving reCAPTCHA v3
-The solving of reCAPTCHA v3 is done by the browser itself, so this library simply waits for the browser to make a POST request to https://www.google.com/recaptcha/api2/reload or https://www.google.com/recaptcha/enterprise/reload and parses the response to get the `g-recaptcha-response` token.
-
----
-
-All solvers return the `g-recaptcha-response` token, which is required for form submissions.
-
-It's important to note that reCAPTCHA v3 uses a token-based scoring system. Each user's token is automatically assigned a score based on their interactions with the website. The score is used to determine the likelihood of the user being a human or a bot. The token is then passed to the web server, and the website owner decides what action to take based on the score.
-
-# Installation
-```
-pip install playwright-recaptcha
-```
-
-This library requires FFmpeg to be installed on your system in order to convert the audio challenge from reCAPTCHA v2 into text.
-
-|   OS    |           Command           |
-| :-----: | :-------------------------: |
-| Debian  | sudo apt-get install ffmpeg |
-|  MacOS  |     brew install ffmpeg     |
-| Windows |    choco install ffmpeg     |
-
-You can also download the latest static build from [here](https://ffmpeg.org/download.html).
-
-> **Note**
-> Make sure to have the ffmpeg and ffprobe binaries in your system's PATH so that the SpeechRecognition library can find them.
-
-# Examples
-
-## reCAPTCHA v2
-
-### Synchronous
-```py
-from playwright.sync_api import sync_playwright
-from playwright_recaptcha import recaptchav2
-
-with sync_playwright() as playwright:
-    browser = playwright.firefox.launch()
-    page = browser.new_page()
-
-    page.goto(
-        "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-    )
-
-    with recaptchav2.SyncSolver(page) as solver:
-        token = solver.solve_recaptcha()
-        print(token)
-```
-
-### Asynchronous
-```py
-import asyncio
-from playwright.async_api import async_playwright
-from playwright_recaptcha import recaptchav2
-
-async def main() -> None:
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
-
-        async with recaptchav2.AsyncSolver(page) as solver:
-            token = await solver.solve_recaptcha()
-            print(token)
-
-asyncio.run(main())
-```
-
-## reCAPTCHA v3
-
-### Synchronous
-```py
-from playwright.sync_api import sync_playwright
-from playwright_recaptcha import recaptchav3
-
-with sync_playwright() as playwright:
-    browser = playwright.firefox.launch()
-    page = browser.new_page()
-    page.goto("https://antcpt.com/score_detector/")
-
-    with recaptchav3.SyncSolver(page) as solver:
-        token = solver.solve_recaptcha()
-        print(token)
-```
-
-### Asynchronous
-```py
-import asyncio
-from playwright.async_api import async_playwright
-from playwright_recaptcha import recaptchav3
-
-async def main() -> None:
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-        await page.goto("https://antcpt.com/score_detector/")
-
-        async with recaptchav3.AsyncSolver(page) as solver:
-            token = await solver.solve_recaptcha()
-            print(token)
-
-asyncio.run(main())
-```
-
-# Exceptions
-|        Exception        |                                                                      Description                                                                      |
-| :---------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
-|     RecaptchaError      |                            The base class for reCAPTCHA exceptions, used as a catch-all for any reCAPTCHA-related errors.                             |
-|   RecaptchaSolveError   |                An exception raised when the reCAPTCHA could not be solved, used as a catch-all for any reCAPTCHA solve-related errors.                |
-| RecaptchaNotFoundError  |                                        An exception raised when the reCAPTCHA v2 was not found on the website.                                        |
-| RecaptchaRateLimitError | An exception raised when the reCAPTCHA rate limit has been exceeded. This can happen if the library is being used to solve reCAPTCHA v2s too quickly. |
-|  RecaptchaTimeoutError  |                                An exception raised when the reCAPTCHA v3 was not solved within the specified timeout.                                 |
-
-# Disclaimer
-This library is intended for use in automated testing and development environments only and should not be used for any illegal or malicious purposes. Any use of this library for activities that violate the terms of service of any website or service is strictly prohibited. The contributors of this library will not be held liable for any damages or legal issues that may arise from the use of this library. By using this library, you agree to these terms and take full responsibility for your actions.
+Metadata-Version: 2.1
+Name: playwright-recaptcha
+Version: 0.2.0
+Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
+Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
+Author: Xewdy444
+Author-email: xewdy@xewdy.tech
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
+Classifier: Framework :: AsyncIO
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![PyPI](https://img.shields.io/pypi/v/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
+[![Downloads](https://img.shields.io/pypi/dm/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
+[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Xewdy444/Playwright-reCAPTCHA/blob/main/LICENSE)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# Playwright-reCAPTCHA
+A Python library for solving reCAPTCHA v2 and v3 with Playwright.
+
+## Solving reCAPTCHA v2
+reCAPTCHA v2 is solved by transcribing the audio challenge using the Google speech recognition API and entering the text as the response.
+
+## Solving reCAPTCHA v3
+The solving of reCAPTCHA v3 is done by the browser itself, so this library simply waits for the browser to make a POST request to https://www.google.com/recaptcha/api2/reload or https://www.google.com/recaptcha/enterprise/reload and parses the response to get the `g-recaptcha-response` token.
+
+---
+
+All solvers return the `g-recaptcha-response` token, which is required for form submissions.
+
+It's important to note that reCAPTCHA v3 uses a token-based scoring system. Each user's token is automatically assigned a score based on their interactions with the website. The score is used to determine the likelihood of the user being a human or a bot. The token is then passed to the web server, and the website owner decides what action to take based on the score.
+
+# Installation
+```
+pip install playwright-recaptcha
+```
+
+This library requires FFmpeg to be installed on your system in order to convert the audio challenge from reCAPTCHA v2 into text.
+
+|   OS    |           Command           |
+| :-----: | :-------------------------: |
+| Debian  | sudo apt-get install ffmpeg |
+|  MacOS  |     brew install ffmpeg     |
+| Windows |    choco install ffmpeg     |
+
+You can also download the latest static build from [here](https://ffmpeg.org/download.html).
+
+> **Note**
+> Make sure to have the ffmpeg and ffprobe binaries in your system's PATH so that the SpeechRecognition library can find them.
+
+# Examples
+
+## reCAPTCHA v2
+
+### Synchronous
+```py
+from playwright.sync_api import sync_playwright
+from playwright_recaptcha import recaptchav2
+
+with sync_playwright() as playwright:
+    browser = playwright.firefox.launch()
+    page = browser.new_page()
+
+    page.goto(
+        "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+    )
+
+    with recaptchav2.SyncSolver(page) as solver:
+        token = solver.solve_recaptcha()
+        print(token)
+```
+
+### Asynchronous
+```py
+import asyncio
+from playwright.async_api import async_playwright
+from playwright_recaptcha import recaptchav2
+
+async def main() -> None:
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+
+        await page.goto(
+            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+        )
+
+        async with recaptchav2.AsyncSolver(page) as solver:
+            token = await solver.solve_recaptcha()
+            print(token)
+
+asyncio.run(main())
+```
+
+## reCAPTCHA v3
+
+### Synchronous
+```py
+from playwright.sync_api import sync_playwright
+from playwright_recaptcha import recaptchav3
+
+with sync_playwright() as playwright:
+    browser = playwright.firefox.launch()
+    page = browser.new_page()
+    page.goto("https://antcpt.com/score_detector/")
+
+    with recaptchav3.SyncSolver(page) as solver:
+        token = solver.solve_recaptcha()
+        print(token)
+```
+
+### Asynchronous
+```py
+import asyncio
+from playwright.async_api import async_playwright
+from playwright_recaptcha import recaptchav3
+
+async def main() -> None:
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+        await page.goto("https://antcpt.com/score_detector/")
+
+        async with recaptchav3.AsyncSolver(page) as solver:
+            token = await solver.solve_recaptcha()
+            print(token)
+
+asyncio.run(main())
+```
+
+# Exceptions
+|        Exception        |                                                                      Description                                                                      |
+| :---------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
+|     RecaptchaError      |                            The base class for reCAPTCHA exceptions, used as a catch-all for any reCAPTCHA-related errors.                             |
+|   RecaptchaSolveError   |                An exception raised when the reCAPTCHA could not be solved, used as a catch-all for any reCAPTCHA solve-related errors.                |
+| RecaptchaNotFoundError  |                                        An exception raised when the reCAPTCHA v2 was not found on the website.                                        |
+| RecaptchaRateLimitError | An exception raised when the reCAPTCHA rate limit has been exceeded. This can happen if the library is being used to solve reCAPTCHA v2s too quickly. |
+|  RecaptchaTimeoutError  |                                An exception raised when the reCAPTCHA v3 was not solved within the specified timeout.                                 |
+
+# Disclaimer
+This library is intended for use in automated testing and development environments only and should not be used for any illegal or malicious purposes. Any use of this library for activities that violate the terms of service of any website or service is strictly prohibited. The contributors of this library will not be held liable for any damages or legal issues that may arise from the use of this library. By using this library, you agree to these terms and take full responsibility for your actions.
```

### Comparing `playwright-recaptcha-0.1.3/README.md` & `playwright-recaptcha-0.2.0/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![PyPI](https://img.shields.io/pypi/v/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
-[![Downloads](https://img.shields.io/pypi/dm/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
-[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Xewdy444/Playwright-reCAPTCHA/blob/main/LICENSE)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-# Playwright-reCAPTCHA
-A Python library for solving reCAPTCHA v2 and v3 with Playwright.
-
-## Solving reCAPTCHA v2
-reCAPTCHA v2 is solved by transcribing the audio challenge using the Google speech recognition API and entering the text as the response.
-
-## Solving reCAPTCHA v3
-The solving of reCAPTCHA v3 is done by the browser itself, so this library simply waits for the browser to make a POST request to https://www.google.com/recaptcha/api2/reload or https://www.google.com/recaptcha/enterprise/reload and parses the response to get the `g-recaptcha-response` token.
-
----
-
-All solvers return the `g-recaptcha-response` token, which is required for form submissions.
-
-It's important to note that reCAPTCHA v3 uses a token-based scoring system. Each user's token is automatically assigned a score based on their interactions with the website. The score is used to determine the likelihood of the user being a human or a bot. The token is then passed to the web server, and the website owner decides what action to take based on the score.
-
-# Installation
-```
-pip install playwright-recaptcha
-```
-
-This library requires FFmpeg to be installed on your system in order to convert the audio challenge from reCAPTCHA v2 into text.
-
-|   OS    |           Command           |
-| :-----: | :-------------------------: |
-| Debian  | sudo apt-get install ffmpeg |
-|  MacOS  |     brew install ffmpeg     |
-| Windows |    choco install ffmpeg     |
-
-You can also download the latest static build from [here](https://ffmpeg.org/download.html).
-
-> **Note**
-> Make sure to have the ffmpeg and ffprobe binaries in your system's PATH so that the SpeechRecognition library can find them.
-
-# Examples
-
-## reCAPTCHA v2
-
-### Synchronous
-```py
-from playwright.sync_api import sync_playwright
-from playwright_recaptcha import recaptchav2
-
-with sync_playwright() as playwright:
-    browser = playwright.firefox.launch()
-    page = browser.new_page()
-
-    page.goto(
-        "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-    )
-
-    with recaptchav2.SyncSolver(page) as solver:
-        token = solver.solve_recaptcha()
-        print(token)
-```
-
-### Asynchronous
-```py
-import asyncio
-from playwright.async_api import async_playwright
-from playwright_recaptcha import recaptchav2
-
-async def main() -> None:
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
-
-        async with recaptchav2.AsyncSolver(page) as solver:
-            token = await solver.solve_recaptcha()
-            print(token)
-
-asyncio.run(main())
-```
-
-## reCAPTCHA v3
-
-### Synchronous
-```py
-from playwright.sync_api import sync_playwright
-from playwright_recaptcha import recaptchav3
-
-with sync_playwright() as playwright:
-    browser = playwright.firefox.launch()
-    page = browser.new_page()
-    page.goto("https://antcpt.com/score_detector/")
-
-    with recaptchav3.SyncSolver(page) as solver:
-        token = solver.solve_recaptcha()
-        print(token)
-```
-
-### Asynchronous
-```py
-import asyncio
-from playwright.async_api import async_playwright
-from playwright_recaptcha import recaptchav3
-
-async def main() -> None:
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-        await page.goto("https://antcpt.com/score_detector/")
-
-        async with recaptchav3.AsyncSolver(page) as solver:
-            token = await solver.solve_recaptcha()
-            print(token)
-
-asyncio.run(main())
-```
-
-# Exceptions
-|        Exception        |                                                                      Description                                                                      |
-| :---------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
-|     RecaptchaError      |                            The base class for reCAPTCHA exceptions, used as a catch-all for any reCAPTCHA-related errors.                             |
-|   RecaptchaSolveError   |                An exception raised when the reCAPTCHA could not be solved, used as a catch-all for any reCAPTCHA solve-related errors.                |
-| RecaptchaNotFoundError  |                                        An exception raised when the reCAPTCHA v2 was not found on the website.                                        |
-| RecaptchaRateLimitError | An exception raised when the reCAPTCHA rate limit has been exceeded. This can happen if the library is being used to solve reCAPTCHA v2s too quickly. |
-|  RecaptchaTimeoutError  |                                An exception raised when the reCAPTCHA v3 was not solved within the specified timeout.                                 |
-
-# Disclaimer
-This library is intended for use in automated testing and development environments only and should not be used for any illegal or malicious purposes. Any use of this library for activities that violate the terms of service of any website or service is strictly prohibited. The contributors of this library will not be held liable for any damages or legal issues that may arise from the use of this library. By using this library, you agree to these terms and take full responsibility for your actions.
+[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![PyPI](https://img.shields.io/pypi/v/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
+[![Downloads](https://img.shields.io/pypi/dm/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
+[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Xewdy444/Playwright-reCAPTCHA/blob/main/LICENSE)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# Playwright-reCAPTCHA
+A Python library for solving reCAPTCHA v2 and v3 with Playwright.
+
+## Solving reCAPTCHA v2
+reCAPTCHA v2 is solved by transcribing the audio challenge using the Google speech recognition API and entering the text as the response.
+
+## Solving reCAPTCHA v3
+The solving of reCAPTCHA v3 is done by the browser itself, so this library simply waits for the browser to make a POST request to https://www.google.com/recaptcha/api2/reload or https://www.google.com/recaptcha/enterprise/reload and parses the response to get the `g-recaptcha-response` token.
+
+---
+
+All solvers return the `g-recaptcha-response` token, which is required for form submissions.
+
+It's important to note that reCAPTCHA v3 uses a token-based scoring system. Each user's token is automatically assigned a score based on their interactions with the website. The score is used to determine the likelihood of the user being a human or a bot. The token is then passed to the web server, and the website owner decides what action to take based on the score.
+
+# Installation
+```
+pip install playwright-recaptcha
+```
+
+This library requires FFmpeg to be installed on your system in order to convert the audio challenge from reCAPTCHA v2 into text.
+
+|   OS    |           Command           |
+| :-----: | :-------------------------: |
+| Debian  | sudo apt-get install ffmpeg |
+|  MacOS  |     brew install ffmpeg     |
+| Windows |    choco install ffmpeg     |
+
+You can also download the latest static build from [here](https://ffmpeg.org/download.html).
+
+> **Note**
+> Make sure to have the ffmpeg and ffprobe binaries in your system's PATH so that the SpeechRecognition library can find them.
+
+# Examples
+
+## reCAPTCHA v2
+
+### Synchronous
+```py
+from playwright.sync_api import sync_playwright
+from playwright_recaptcha import recaptchav2
+
+with sync_playwright() as playwright:
+    browser = playwright.firefox.launch()
+    page = browser.new_page()
+
+    page.goto(
+        "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+    )
+
+    with recaptchav2.SyncSolver(page) as solver:
+        token = solver.solve_recaptcha()
+        print(token)
+```
+
+### Asynchronous
+```py
+import asyncio
+from playwright.async_api import async_playwright
+from playwright_recaptcha import recaptchav2
+
+async def main() -> None:
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+
+        await page.goto(
+            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+        )
+
+        async with recaptchav2.AsyncSolver(page) as solver:
+            token = await solver.solve_recaptcha()
+            print(token)
+
+asyncio.run(main())
+```
+
+## reCAPTCHA v3
+
+### Synchronous
+```py
+from playwright.sync_api import sync_playwright
+from playwright_recaptcha import recaptchav3
+
+with sync_playwright() as playwright:
+    browser = playwright.firefox.launch()
+    page = browser.new_page()
+    page.goto("https://antcpt.com/score_detector/")
+
+    with recaptchav3.SyncSolver(page) as solver:
+        token = solver.solve_recaptcha()
+        print(token)
+```
+
+### Asynchronous
+```py
+import asyncio
+from playwright.async_api import async_playwright
+from playwright_recaptcha import recaptchav3
+
+async def main() -> None:
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+        await page.goto("https://antcpt.com/score_detector/")
+
+        async with recaptchav3.AsyncSolver(page) as solver:
+            token = await solver.solve_recaptcha()
+            print(token)
+
+asyncio.run(main())
+```
+
+# Exceptions
+|        Exception        |                                                                      Description                                                                      |
+| :---------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
+|     RecaptchaError      |                            The base class for reCAPTCHA exceptions, used as a catch-all for any reCAPTCHA-related errors.                             |
+|   RecaptchaSolveError   |                An exception raised when the reCAPTCHA could not be solved, used as a catch-all for any reCAPTCHA solve-related errors.                |
+| RecaptchaNotFoundError  |                                        An exception raised when the reCAPTCHA v2 was not found on the website.                                        |
+| RecaptchaRateLimitError | An exception raised when the reCAPTCHA rate limit has been exceeded. This can happen if the library is being used to solve reCAPTCHA v2s too quickly. |
+|  RecaptchaTimeoutError  |                                An exception raised when the reCAPTCHA v3 was not solved within the specified timeout.                                 |
+
+# Disclaimer
+This library is intended for use in automated testing and development environments only and should not be used for any illegal or malicious purposes. Any use of this library for activities that violate the terms of service of any website or service is strictly prohibited. The contributors of this library will not be held liable for any damages or legal issues that may arise from the use of this library. By using this library, you agree to these terms and take full responsibility for your actions.
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha/__init__.py` & `playwright-recaptcha-0.2.0/playwright_recaptcha/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""A library for solving reCAPTCHA v2 and v3 with Playwright."""
-from playwright_recaptcha.errors import (
-    RecaptchaError,
-    RecaptchaNotFoundError,
-    RecaptchaRateLimitError,
-    RecaptchaSolveError,
-    RecaptchaTimeoutError,
-)
-from playwright_recaptcha.recaptchav2.async_solver import AsyncSolver as AsyncSolverV2
-from playwright_recaptcha.recaptchav2.sync_solver import SyncSolver as SyncSolverV2
-from playwright_recaptcha.recaptchav3.async_solver import AsyncSolver as AsyncSolverV3
-from playwright_recaptcha.recaptchav3.sync_solver import SyncSolver as SyncSolverV3
-
-__all__ = [
-    "RecaptchaError",
-    "RecaptchaNotFoundError",
-    "RecaptchaRateLimitError",
-    "RecaptchaSolveError",
-    "RecaptchaTimeoutError",
-    "AsyncSolverV2",
-    "SyncSolverV2",
-    "AsyncSolverV3",
-    "SyncSolverV3",
-]
+"""A library for solving reCAPTCHA v2 and v3 with Playwright."""
+from playwright_recaptcha.errors import (
+    RecaptchaError,
+    RecaptchaNotFoundError,
+    RecaptchaRateLimitError,
+    RecaptchaSolveError,
+    RecaptchaTimeoutError,
+)
+from playwright_recaptcha.recaptchav2.async_solver import AsyncSolver as AsyncSolverV2
+from playwright_recaptcha.recaptchav2.sync_solver import SyncSolver as SyncSolverV2
+from playwright_recaptcha.recaptchav3.async_solver import AsyncSolver as AsyncSolverV3
+from playwright_recaptcha.recaptchav3.sync_solver import SyncSolver as SyncSolverV3
+
+__all__ = [
+    "RecaptchaError",
+    "RecaptchaNotFoundError",
+    "RecaptchaRateLimitError",
+    "RecaptchaSolveError",
+    "RecaptchaTimeoutError",
+    "AsyncSolverV2",
+    "SyncSolverV2",
+    "AsyncSolverV3",
+    "SyncSolverV3",
+]
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha/errors.py` & `playwright-recaptcha-0.2.0/playwright_recaptcha/errors.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Optional
-
-
-class RecaptchaError(Exception):
-    """Base class for reCAPTCHA exceptions."""
-
-
-class RecaptchaSolveError(RecaptchaError):
-    """Base class for reCAPTCHA solve exceptions."""
-
-    def __init__(self, message: Optional[str] = None) -> None:
-        super().__init__(message or "The reCAPTCHA could not be solved.")
-
-
-class RecaptchaNotFoundError(RecaptchaError):
-    """An exception raised when the reCAPTCHA was not found."""
-
-    def __init__(self) -> None:
-        super().__init__("The reCAPTCHA was not found.")
-
-
-class RecaptchaRateLimitError(RecaptchaSolveError):
-    """An exception raised when the reCAPTCHA rate limit has been exceeded."""
-
-    def __init__(self) -> None:
-        super().__init__("The reCAPTCHA rate limit has been exceeded.")
-
-
-class RecaptchaTimeoutError(RecaptchaSolveError):
-    """An exception raised when the reCAPTCHA solve timeout has been exceeded."""
-
-    def __init__(self) -> None:
-        super().__init__("The reCAPTCHA solve timeout has been exceeded.")
+from typing import Optional
+
+
+class RecaptchaError(Exception):
+    """Base class for reCAPTCHA exceptions."""
+
+
+class RecaptchaSolveError(RecaptchaError):
+    """Base class for reCAPTCHA solve exceptions."""
+
+    def __init__(self, message: Optional[str] = None) -> None:
+        super().__init__(message or "The reCAPTCHA could not be solved.")
+
+
+class RecaptchaNotFoundError(RecaptchaError):
+    """An exception raised when the reCAPTCHA was not found."""
+
+    def __init__(self) -> None:
+        super().__init__("The reCAPTCHA was not found.")
+
+
+class RecaptchaRateLimitError(RecaptchaSolveError):
+    """An exception raised when the reCAPTCHA rate limit has been exceeded."""
+
+    def __init__(self) -> None:
+        super().__init__("The reCAPTCHA rate limit has been exceeded.")
+
+
+class RecaptchaTimeoutError(RecaptchaSolveError):
+    """An exception raised when the reCAPTCHA solve timeout has been exceeded."""
+
+    def __init__(self) -> None:
+        super().__init__("The reCAPTCHA solve timeout has been exceeded.")
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/async_solver.py` & `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/async_solver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,289 +1,306 @@
-from __future__ import annotations
-
-import asyncio
-import functools
-import io
-import random
-import re
-from concurrent.futures import ThreadPoolExecutor
-from typing import Any, Optional
-
-import httpx
-import pydub
-import speech_recognition
-from playwright.async_api import Page, Response
-
-from playwright_recaptcha.errors import (
-    RecaptchaNotFoundError,
-    RecaptchaRateLimitError,
-    RecaptchaSolveError,
-)
-from playwright_recaptcha.recaptchav2.recaptcha_box import AsyncRecaptchaBox
-
-
-class AsyncSolver:
-    """
-    A class used to solve reCAPTCHA v2 asynchronously.
-
-    Parameters
-    ----------
-    page : Page
-        The playwright page to solve the reCAPTCHA on.
-    attempts : int, optional
-        The number of solve attempts, by default 3.
-
-    Attributes
-    ----------
-    token : Optional[str]
-        The g-recaptcha-response token.
-
-    Methods
-    -------
-    close() -> None
-        Remove the userverify response listener.
-    solve_recaptcha(attempts: Optional[int] = None) -> str
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaRateLimitError
-        If the reCAPTCHA rate limit has been exceeded.
-    RecaptchaSolveError
-        If the reCAPTCHA could not be solved.
-    """
-
-    def __init__(self, page: Page, attempts: int = 3) -> None:
-        self._page = page
-        self._attempts = attempts
-        self.token: Optional[str] = None
-
-    def __repr__(self) -> str:
-        return f"AsyncSolver(page={self._page!r}, attempts={self._attempts!r})"
-
-    async def __aenter__(self) -> AsyncSolver:
-        return self
-
-    async def __aexit__(self, *args: Any) -> None:
-        self.close()
-
-    @staticmethod
-    async def _convert_audio_to_text(audio_url: str) -> Optional[str]:
-        """
-        Convert the reCAPTCHA audio to text.
-
-        Parameters
-        ----------
-        audio_url : str
-            The reCAPTCHA audio URL.
-
-        Returns
-        -------
-        Optional[str]
-            The reCAPTCHA audio text.
-        """
-        loop = asyncio.get_event_loop()
-
-        async with httpx.AsyncClient() as client:
-            response = await client.get(audio_url)
-
-        wav_audio = io.BytesIO()
-        mp3_audio = io.BytesIO(response.content)
-
-        with ThreadPoolExecutor() as executor:
-            audio = await loop.run_in_executor(
-                executor, pydub.AudioSegment.from_mp3, mp3_audio
-            )
-
-            await loop.run_in_executor(
-                executor, functools.partial(audio.export, wav_audio, format="wav")
-            )
-
-            recognizer = speech_recognition.Recognizer()
-
-            with speech_recognition.AudioFile(wav_audio) as source:
-                audio_data = await loop.run_in_executor(
-                    executor, recognizer.record, source
-                )
-
-            try:
-                return await loop.run_in_executor(
-                    executor, recognizer.recognize_google, audio_data
-                )
-            except speech_recognition.UnknownValueError:
-                return None
-
-    async def _random_delay(self) -> None:
-        """Delay the execution for a random amount of time between 1 and 4 seconds."""
-        await self._page.wait_for_timeout(random.randint(1000, 4000))
-
-    async def _extract_token(self, response: Response) -> None:
-        """
-        Extract the g-recaptcha-response token from the userverify response.
-
-        Parameters
-        ----------
-        response : Response
-            The response to extract the g-recaptcha-response token from.
-        """
-        if re.search("/recaptcha/(api2|enterprise)/userverify", response.url) is None:
-            return
-
-        token_match = re.search('"uvresp","(.*?)"', await response.text())
-
-        if token_match is not None:
-            self.token = token_match.group(1)
-
-    async def _get_audio_url(self, recaptcha_box: AsyncRecaptchaBox) -> str:
-        """
-        Get the reCAPTCHA audio URL.
-
-        Parameters
-        ----------
-        recaptcha_box : AsyncRecaptchaBox
-            The reCAPTCHA box.
-
-        Returns
-        -------
-        str
-            The reCAPTCHA audio URL.
-
-        Raises
-        ------
-        RecaptchaRateLimitError
-            If the reCAPTCHA rate limit has been exceeded.
-        """
-        if await recaptcha_box.audio_challenge_button.is_visible():
-            await recaptcha_box.audio_challenge_button.click(force=True)
-
-        while True:
-            if await recaptcha_box.audio_challenge_is_visible():
-                break
-
-            if await recaptcha_box.rate_limit_is_visible():
-                raise RecaptchaRateLimitError
-
-            await self._page.wait_for_timeout(100)
-
-        return await recaptcha_box.audio_download_button.get_attribute("href")
-
-    async def _submit_audio_text(
-        self, recaptcha_box: AsyncRecaptchaBox, text: str
-    ) -> None:
-        """
-        Submit the reCAPTCHA audio text.
-
-        Parameters
-        ----------
-        recaptcha_box : AsyncRecaptchaBox
-            The reCAPTCHA box.
-        text : str
-            The reCAPTCHA audio text.
-
-        Raises
-        ------
-        RecaptchaRateLimitError
-            If the reCAPTCHA rate limit has been exceeded.
-        """
-        await recaptcha_box.audio_challenge_textbox.fill(text)
-        await recaptcha_box.audio_challenge_verify_button.click()
-
-        while recaptcha_box.frames_are_attached():
-            if (
-                await recaptcha_box.checkbox.is_checked()
-                or await recaptcha_box.solve_failure_is_visible()
-            ):
-                break
-
-            if await recaptcha_box.rate_limit_is_visible():
-                raise RecaptchaRateLimitError
-
-            await self._page.wait_for_timeout(100)
-
-    def close(self) -> None:
-        """Remove the userverify response listener."""
-        try:
-            self._page.remove_listener("response", self._extract_token)
-        except KeyError:
-            pass
-
-    async def solve_recaptcha(self, attempts: Optional[int] = None) -> str:
-        """
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-        Parameters
-        ----------
-        attempts : Optional[int], optional
-            The number of solve attempts, by default 3.
-
-        Returns
-        -------
-        str
-            The g-recaptcha-response token.
-
-        Raises
-        ------
-        RecaptchaNotFoundError
-            If the reCAPTCHA was not found.
-        RecaptchaRateLimitError
-            If the reCAPTCHA rate limit has been exceeded.
-        RecaptchaSolveError
-            If the reCAPTCHA could not be solved.
-        """
-        self.token = None
-        self._page.on("response", self._extract_token)
-
-        attempts = attempts or self._attempts
-        recaptcha_box = await AsyncRecaptchaBox.from_frames(self._page.frames)
-
-        if await recaptcha_box.checkbox.is_hidden():
-            raise RecaptchaNotFoundError
-
-        await recaptcha_box.checkbox.click(force=True)
-
-        while True:
-            if (
-                await recaptcha_box.audio_challenge_is_visible()
-                or await recaptcha_box.audio_challenge_button.is_visible()
-                and await recaptcha_box.audio_challenge_button.is_enabled()
-            ):
-                break
-
-            if (
-                not recaptcha_box.frames_are_attached()
-                or await recaptcha_box.checkbox.is_checked()
-            ):
-                if self.token is None:
-                    raise RecaptchaSolveError
-
-                return self.token
-
-            await self._page.wait_for_timeout(100)
-
-        while attempts > 0:
-            await self._random_delay()
-            url = await self._get_audio_url(recaptcha_box)
-            text = await self._convert_audio_to_text(url)
-
-            if text is None:
-                await recaptcha_box.new_challenge_button.click()
-                attempts -= 1
-                continue
-
-            await self._random_delay()
-            await self._submit_audio_text(recaptcha_box, text)
-
-            if (
-                not recaptcha_box.frames_are_attached()
-                or await recaptcha_box.checkbox.is_checked()
-            ):
-                if self.token is None:
-                    raise RecaptchaSolveError
-
-                return self.token
-
-            await recaptcha_box.new_challenge_button.click()
-            attempts -= 1
-
-        raise RecaptchaSolveError
+from __future__ import annotations
+
+import asyncio
+import functools
+import io
+import random
+import re
+from concurrent.futures import ThreadPoolExecutor
+from typing import Any, Optional
+
+import pydub
+import speech_recognition
+from playwright.async_api import Page, Response
+
+from playwright_recaptcha.errors import (
+    RecaptchaNotFoundError,
+    RecaptchaRateLimitError,
+    RecaptchaSolveError,
+)
+from playwright_recaptcha.recaptchav2.recaptcha_box import AsyncRecaptchaBox
+
+
+class AsyncSolver:
+    """
+    A class used to solve reCAPTCHA v2 asynchronously.
+
+    Parameters
+    ----------
+    page : Page
+        The playwright page to solve the reCAPTCHA on.
+    attempts : int, optional
+        The number of solve attempts, by default 3.
+
+    Attributes
+    ----------
+    token : Optional[str]
+        The g-recaptcha-response token.
+
+    Methods
+    -------
+    close() -> None
+        Remove the userverify response listener.
+    solve_recaptcha(attempts: Optional[int] = None) -> str
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+    Raises
+    ------
+    RecaptchaNotFoundError
+        If the reCAPTCHA was not found.
+    RecaptchaRateLimitError
+        If the reCAPTCHA rate limit has been exceeded.
+    RecaptchaSolveError
+        If the reCAPTCHA could not be solved.
+    """
+
+    def __init__(self, page: Page, attempts: int = 3) -> None:
+        self._page = page
+        self._attempts = attempts
+        self.token: Optional[str] = None
+
+    def __repr__(self) -> str:
+        return f"AsyncSolver(page={self._page!r}, attempts={self._attempts!r})"
+
+    async def __aenter__(self) -> AsyncSolver:
+        return self
+
+    async def __aexit__(self, *args: Any) -> None:
+        self.close()
+
+    async def _convert_audio_to_text(self, audio_url: str) -> Optional[str]:
+        """
+        Convert the reCAPTCHA audio to text.
+
+        Parameters
+        ----------
+        audio_url : str
+            The reCAPTCHA audio URL.
+
+        Returns
+        -------
+        Optional[str]
+            The reCAPTCHA audio text.
+        """
+        loop = asyncio.get_event_loop()
+        response = await self._page.request.get(audio_url)
+
+        wav_audio = io.BytesIO()
+        mp3_audio = io.BytesIO(await response.body())
+
+        with ThreadPoolExecutor() as executor:
+            audio = await loop.run_in_executor(
+                executor, pydub.AudioSegment.from_mp3, mp3_audio
+            )
+
+            await loop.run_in_executor(
+                executor, functools.partial(audio.export, wav_audio, format="wav")
+            )
+
+            recognizer = speech_recognition.Recognizer()
+
+            with speech_recognition.AudioFile(wav_audio) as source:
+                audio_data = await loop.run_in_executor(
+                    executor, recognizer.record, source
+                )
+
+            try:
+                return await loop.run_in_executor(
+                    executor, recognizer.recognize_google, audio_data
+                )
+            except speech_recognition.UnknownValueError:
+                return None
+
+    async def _random_delay(self) -> None:
+        """Delay the execution for a random amount of time between 1 and 4 seconds."""
+        await self._page.wait_for_timeout(random.randint(1000, 4000))
+
+    async def _extract_token(self, response: Response) -> None:
+        """
+        Extract the g-recaptcha-response token from the userverify response.
+
+        Parameters
+        ----------
+        response : Response
+            The response to extract the g-recaptcha-response token from.
+        """
+        if re.search("/recaptcha/(api2|enterprise)/userverify", response.url) is None:
+            return
+
+        token_match = re.search('"uvresp","(.*?)"', await response.text())
+
+        if token_match is not None:
+            self.token = token_match.group(1)
+
+    async def _click_checkbox(self, recaptcha_box: AsyncRecaptchaBox) -> None:
+        """
+        Click the reCAPTCHA checkbox.
+
+        Parameters
+        ----------
+        recaptcha_box : AsyncRecaptchaBox
+            The reCAPTCHA box.
+        """
+        await recaptcha_box.checkbox.click(force=True)
+
+        while recaptcha_box.frames_are_attached():
+            if await recaptcha_box.is_solved():
+                if self.token is None:
+                    raise RecaptchaSolveError
+
+                break
+
+            if (
+                await recaptcha_box.audio_challenge_is_visible()
+                or await recaptcha_box.audio_challenge_button.is_visible()
+                and await recaptcha_box.audio_challenge_button.is_enabled()
+            ):
+                break
+
+            await self._page.wait_for_timeout(250)
+
+    async def _get_audio_url(self, recaptcha_box: AsyncRecaptchaBox) -> str:
+        """
+        Get the reCAPTCHA audio URL.
+
+        Parameters
+        ----------
+        recaptcha_box : AsyncRecaptchaBox
+            The reCAPTCHA box.
+
+        Returns
+        -------
+        str
+            The reCAPTCHA audio URL.
+
+        Raises
+        ------
+        RecaptchaRateLimitError
+            If the reCAPTCHA rate limit has been exceeded.
+        """
+        if await recaptcha_box.audio_challenge_button.is_visible():
+            await recaptcha_box.audio_challenge_button.click(force=True)
+
+        while True:
+            if await recaptcha_box.rate_limit_is_visible():
+                raise RecaptchaRateLimitError
+
+            if await recaptcha_box.audio_challenge_is_visible():
+                break
+
+            await self._page.wait_for_timeout(250)
+
+        return await recaptcha_box.audio_download_button.get_attribute("href")
+
+    async def _submit_audio_text(
+        self, recaptcha_box: AsyncRecaptchaBox, text: str
+    ) -> None:
+        """
+        Submit the reCAPTCHA audio text.
+
+        Parameters
+        ----------
+        recaptcha_box : AsyncRecaptchaBox
+            The reCAPTCHA box.
+        text : str
+            The reCAPTCHA audio text.
+
+        Raises
+        ------
+        RecaptchaRateLimitError
+            If the reCAPTCHA rate limit has been exceeded.
+        """
+        await recaptcha_box.audio_challenge_textbox.fill(text)
+
+        async with self._page.expect_response(
+            re.compile("/recaptcha/(api2|enterprise)/userverify")
+        ):
+            await recaptcha_box.audio_challenge_verify_button.click()
+
+        while recaptcha_box.frames_are_attached():
+            if await recaptcha_box.rate_limit_is_visible():
+                raise RecaptchaRateLimitError
+
+            if (
+                await recaptcha_box.new_challenge_button.is_disabled()
+                or await recaptcha_box.solve_failure_is_visible()
+                or await recaptcha_box.is_solved()
+            ):
+                break
+
+            await self._page.wait_for_timeout(250)
+
+    def close(self) -> None:
+        """Remove the userverify response listener."""
+        try:
+            self._page.remove_listener("response", self._extract_token)
+        except KeyError:
+            pass
+
+    async def solve_recaptcha(self, attempts: Optional[int] = None) -> str:
+        """
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+        Parameters
+        ----------
+        attempts : Optional[int], optional
+            The number of solve attempts, by default 3.
+
+        Returns
+        -------
+        str
+            The g-recaptcha-response token.
+
+        Raises
+        ------
+        RecaptchaNotFoundError
+            If the reCAPTCHA was not found.
+        RecaptchaRateLimitError
+            If the reCAPTCHA rate limit has been exceeded.
+        RecaptchaSolveError
+            If the reCAPTCHA could not be solved.
+        """
+        self.token = None
+        self._page.on("response", self._extract_token)
+
+        attempts = attempts or self._attempts
+        recaptcha_box = await AsyncRecaptchaBox.from_frames(self._page.frames)
+
+        if (
+            await recaptcha_box.checkbox.is_hidden()
+            and await recaptcha_box.audio_challenge_button.is_disabled()
+        ):
+            raise RecaptchaNotFoundError
+
+        if await recaptcha_box.checkbox.is_visible():
+            await self._click_checkbox(recaptcha_box)
+
+            if self.token is not None:
+                return self.token
+
+        while attempts > 0:
+            await self._random_delay()
+            url = await self._get_audio_url(recaptcha_box)
+            text = await self._convert_audio_to_text(url)
+
+            if text is None:
+                await recaptcha_box.new_challenge_button.click()
+                attempts -= 1
+                continue
+
+            await self._random_delay()
+            await self._submit_audio_text(recaptcha_box, text)
+
+            if (
+                recaptcha_box.frames_are_detached()
+                or await recaptcha_box.new_challenge_button.is_disabled()
+                or await recaptcha_box.is_solved()
+            ):
+                if self.token is None:
+                    raise RecaptchaSolveError
+
+                return self.token
+
+            await recaptcha_box.new_challenge_button.click()
+            attempts -= 1
+
+        raise RecaptchaSolveError
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/recaptcha_box.py` & `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/recaptcha_box.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,503 +1,623 @@
-from __future__ import annotations
-
-import re
-from abc import ABC, abstractmethod
-from typing import Iterable, List, Tuple, Union
-
-from playwright.async_api import Frame as AsyncFrame
-from playwright.async_api import Locator as AsyncLocator
-from playwright.sync_api import Frame as SyncFrame
-from playwright.sync_api import Locator as SyncLocator
-
-from playwright_recaptcha.errors import RecaptchaNotFoundError, RecaptchaSolveError
-
-Locator = Union[AsyncLocator, SyncLocator]
-Frame = Union[AsyncFrame, SyncFrame]
-
-
-class RecaptchaBox(ABC):
-    """
-    The base class for reCAPTCHA v2 boxes.
-
-    Attributes
-    ----------
-    anchor_frame : Frame
-        The reCAPTCHA anchor frame.
-    bframe_frame : Frame
-        The reCAPTCHA bframe frame.
-    checkbox : Locator
-        The reCAPTCHA checkbox locator.
-    audio_challenge_button : Locator
-        The reCAPTCHA audio challenge button locator.
-    new_challenge_button : Locator
-        The reCAPTCHA new challenge button locator.
-    audio_download_button : Locator
-        The reCAPTCHA audio download button locator.
-    audio_challenge_textbox : Locator
-        The reCAPTCHA audio challenge textbox locator.
-    audio_challenge_verify_button : Locator
-        The reCAPTCHA audio challenge verify button locator.
-
-    Methods
-    -------
-    from_frames(frames: Iterable[Frame]) -> Union[AsyncRecaptchaBox, SyncRecaptchaBox]
-        Create a reCAPTCHA box using a list of frames.
-    frames_are_attached() -> bool
-        Check if the reCAPTCHA frames are attached.
-    rate_limit_is_visible() -> bool
-        Check if the reCAPTCHA rate limit message is visible.
-    solve_failure_is_visible() -> bool
-        Check if the reCAPTCHA solve failure message is visible.
-    audio_challenge_is_visible() -> bool
-        Check if the reCAPTCHA audio challenge is visible.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaSolveError
-        If no unchecked reCAPTCHA boxes were found.
-    """
-
-    @staticmethod
-    def _get_recaptcha_frame_pairs(
-        frames: Iterable[Frame],
-    ) -> List[Tuple[Frame, Frame]]:
-        """
-        Get the reCAPTCHA anchor and bframe frame pairs.
-
-        Parameters
-        ----------
-        frames : Iterable[Frame]
-            A list of frames to search for the reCAPTCHA anchor and bframe frames.
-
-        Returns
-        -------
-        List[Tuple[Frame, Frame]]
-            A list of reCAPTCHA anchor and bframe frame pairs.
-
-        Raises
-        ------
-        RecaptchaNotFoundError
-            If no reCAPTCHA anchor and bframe frame pairs were found.
-        """
-        anchor_frames = list(
-            filter(
-                lambda frame: re.search(
-                    "/recaptcha/(api2|enterprise)/anchor", frame.url
-                )
-                is not None,
-                frames,
-            )
-        )
-
-        bframe_frames = list(
-            filter(
-                lambda frame: re.search(
-                    "/recaptcha/(api2|enterprise)/bframe", frame.url
-                )
-                is not None,
-                frames,
-            )
-        )
-
-        frame_pairs = []
-
-        for anchor_frame in anchor_frames:
-            frame_id = anchor_frame.name[2:]
-
-            for bframe_frame in bframe_frames:
-                if frame_id in bframe_frame.name:
-                    frame_pairs.append((anchor_frame, bframe_frame))
-
-        if not frame_pairs:
-            raise RecaptchaNotFoundError
-
-        return frame_pairs
-
-    @property
-    def checkbox(self) -> Locator:
-        """The reCAPTCHA checkbox locator."""
-        return self.anchor_frame.get_by_role("checkbox", name="I'm not a robot")
-
-    @property
-    def audio_challenge_button(self) -> Locator:
-        """The reCAPTCHA audio challenge button locator."""
-        return self.bframe_frame.get_by_role("button", name="Get an audio challenge")
-
-    @property
-    def new_challenge_button(self) -> Locator:
-        """The reCAPTCHA new challenge button locator."""
-        return self.bframe_frame.get_by_role("button", name="Get a new challenge")
-
-    @property
-    def audio_download_button(self) -> Locator:
-        """The reCAPTCHA audio download button locator."""
-        return self.bframe_frame.get_by_role(
-            "link", name="Alternatively, download audio as MP3"
-        )
-
-    @property
-    def audio_challenge_textbox(self) -> Locator:
-        """The reCAPTCHA audio challenge textbox locator."""
-        return self.bframe_frame.get_by_role("textbox", name="Enter what you hear")
-
-    @property
-    def audio_challenge_verify_button(self) -> Locator:
-        """The reCAPTCHA audio challenge verify button locator."""
-        return self.bframe_frame.get_by_role("button", name="Verify")
-
-    def frames_are_attached(self) -> bool:
-        """
-        Check if the reCAPTCHA frames are attached.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA frames are attached, False otherwise.
-        """
-        return (
-            not self.bframe_frame.is_detached() and not self.anchor_frame.is_detached()
-        )
-
-    @property
-    @abstractmethod
-    def anchor_frame(self) -> Frame:
-        """The reCAPTCHA anchor frame."""
-
-    @property
-    @abstractmethod
-    def bframe_frame(self) -> Frame:
-        """The reCAPTCHA bframe frame."""
-
-    @classmethod
-    @abstractmethod
-    def from_frames(
-        cls,
-        frames: Iterable[Frame],
-    ) -> Union[AsyncRecaptchaBox, SyncRecaptchaBox]:
-        """
-        Create a reCAPTCHA box using a list of frames.
-
-        Parameters
-        ----------
-        frames : Iterable[Frame]
-            A list of frames to search for the reCAPTCHA frames.
-
-        Returns
-        -------
-        Union[AsyncRecaptchaBox, SyncRecaptchaBox]
-            The reCAPTCHA box.
-
-        Raises
-        ------
-        RecaptchaNotFoundError
-            If the reCAPTCHA frames were not found.
-        RecaptchaSolveError
-            If no unchecked reCAPTCHA boxes were found.
-        """
-
-    @abstractmethod
-    def rate_limit_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA rate limit message is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA rate limit message is visible, False otherwise.
-        """
-
-    @abstractmethod
-    def solve_failure_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA solve failure message is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA solve failure message is visible, False otherwise.
-        """
-
-    @abstractmethod
-    def audio_challenge_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA audio challenge is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA audio challenge is visible, False otherwise.
-        """
-
-
-class SyncRecaptchaBox(RecaptchaBox):
-    """
-    The synchronous class for reCAPTCHA v2 boxes.
-
-    Parameters
-    ----------
-    anchor_frame : SyncFrame
-        The reCAPTCHA anchor frame.
-    bframe_frame : SyncFrame
-        The reCAPTCHA bframe frame.
-
-    Attributes
-    ----------
-    anchor_frame : Frame
-        The reCAPTCHA anchor frame.
-    bframe_frame : Frame
-        The reCAPTCHA bframe frame.
-    checkbox : Locator
-        The reCAPTCHA checkbox locator.
-    audio_challenge_button : Locator
-        The reCAPTCHA audio challenge button locator.
-    new_challenge_button : Locator
-        The reCAPTCHA new challenge button locator.
-    audio_download_button : Locator
-        The reCAPTCHA audio download button locator.
-    audio_challenge_textbox : Locator
-        The reCAPTCHA audio challenge textbox locator.
-    audio_challenge_verify_button : Locator
-        The reCAPTCHA audio challenge verify button locator.
-
-    Methods
-    -------
-    from_frames(frames: Iterable[SyncFrame]) -> SyncRecaptchaBox
-        Create a reCAPTCHA box using a list of frames.
-    frames_are_attached() -> bool
-        Check if the reCAPTCHA frames are attached.
-    rate_limit_is_visible() -> bool
-        Check if the reCAPTCHA rate limit message is visible.
-    solve_failure_is_visible() -> bool
-        Check if the reCAPTCHA solve failure message is visible.
-    audio_challenge_is_visible() -> bool
-        Check if the reCAPTCHA audio challenge is visible.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaSolveError
-        If no unchecked reCAPTCHA boxes were found.
-    """
-
-    def __init__(self, anchor_frame: SyncFrame, bframe_frame: SyncFrame) -> None:
-        self._anchor_frame = anchor_frame
-        self._bframe_frame = bframe_frame
-
-    def __repr__(self) -> str:
-        return f"SyncRecaptchaBox(anchor_frame={self._anchor_frame!r}, bframe_frame={self._bframe_frame!r})"
-
-    @classmethod
-    def from_frames(cls, frames: Iterable[SyncFrame]) -> SyncRecaptchaBox:
-        """
-        Create a reCAPTCHA box using a list of frames.
-
-        Parameters
-        ----------
-        frames : Iterable[SyncFrame]
-            A list of frames to search for the reCAPTCHA frames.
-
-        Returns
-        -------
-        SyncRecaptchaBox
-            The reCAPTCHA box.
-
-        Raises
-        ------
-        RecaptchaNotFoundError
-            If the reCAPTCHA frames were not found.
-        RecaptchaSolveError
-            If no unchecked reCAPTCHA boxes were found.
-        """
-        frame_pairs = cls._get_recaptcha_frame_pairs(frames)
-
-        for anchor_frame, bframe_frame in frame_pairs:
-            if not anchor_frame.get_by_role(
-                "checkbox", name="I'm not a robot"
-            ).is_checked():
-                return cls(anchor_frame, bframe_frame)
-
-        raise RecaptchaSolveError("No unchecked reCAPTCHA boxes were found.")
-
-    @property
-    def anchor_frame(self) -> SyncFrame:
-        """The reCAPTCHA anchor frame."""
-        return self._anchor_frame
-
-    @property
-    def bframe_frame(self) -> SyncFrame:
-        """The reCAPTCHA bframe frame."""
-        return self._bframe_frame
-
-    def rate_limit_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA rate limit message is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA rate limit message is visible, False otherwise.
-        """
-        return self.bframe_frame.get_by_text("Try again later").is_visible()
-
-    def solve_failure_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA solve failure message is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA solve failure message is visible, False otherwise.
-        """
-        return self.bframe_frame.get_by_text(
-            "Multiple correct solutions required - please solve more."
-        ).is_visible()
-
-    def audio_challenge_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA audio challenge is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA audio challenge is visible, False otherwise.
-        """
-        return self.bframe_frame.get_by_text("Press PLAY to listen").is_visible()
-
-
-class AsyncRecaptchaBox(RecaptchaBox):
-    """
-    The asynchronous class for reCAPTCHA v2 boxes.
-
-    Parameters
-    ----------
-    anchor_frame : AsyncFrame
-        The reCAPTCHA anchor frame.
-    bframe_frame : AsyncFrame
-        The reCAPTCHA bframe frame.
-
-    Attributes
-    ----------
-    anchor_frame : Frame
-        The reCAPTCHA anchor frame.
-    bframe_frame : Frame
-        The reCAPTCHA bframe frame.
-    checkbox : Locator
-        The reCAPTCHA checkbox locator.
-    audio_challenge_button : Locator
-        The reCAPTCHA audio challenge button locator.
-    new_challenge_button : Locator
-        The reCAPTCHA new challenge button locator.
-    audio_download_button : Locator
-        The reCAPTCHA audio download button locator.
-    audio_challenge_textbox : Locator
-        The reCAPTCHA audio challenge textbox locator.
-    audio_challenge_verify_button : Locator
-        The reCAPTCHA audio challenge verify button locator.
-
-    Methods
-    -------
-    from_frames(frames: Iterable[AsyncFrame]) -> AsyncRecaptchaBox
-        Create a reCAPTCHA box using a list of frames.
-    frames_are_attached() -> bool
-        Check if the reCAPTCHA frames are attached.
-    rate_limit_is_visible() -> bool
-        Check if the reCAPTCHA rate limit message is visible.
-    solve_failure_is_visible() -> bool
-        Check if the reCAPTCHA solve failure message is visible.
-    audio_challenge_is_visible() -> bool
-        Check if the reCAPTCHA audio challenge is visible.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaSolveError
-        If no unchecked reCAPTCHA boxes were found.
-    """
-
-    def __init__(self, anchor_frame: AsyncFrame, bframe_frame: AsyncFrame) -> None:
-        self._anchor_frame = anchor_frame
-        self._bframe_frame = bframe_frame
-
-    def __repr__(self) -> str:
-        return f"AsyncRecaptchaBox(anchor_frame={self._anchor_frame!r}, bframe_frame={self._bframe_frame!r})"
-
-    @classmethod
-    async def from_frames(cls, frames: Iterable[AsyncFrame]) -> AsyncRecaptchaBox:
-        """
-        Create a reCAPTCHA box using a list of frames.
-
-        Parameters
-        ----------
-        frames : Iterable[AsyncFrame]
-            A list of frames to search for the reCAPTCHA frames.
-
-        Returns
-        -------
-        AsyncRecaptchaBox
-            The reCAPTCHA box.
-
-        Raises
-        ------
-        RecaptchaNotFoundError
-            If the reCAPTCHA frames were not found.
-        RecaptchaSolveError
-            If no unchecked reCAPTCHA boxes were found.
-        """
-        frame_pairs = cls._get_recaptcha_frame_pairs(frames)
-
-        for anchor_frame, bframe_frame in frame_pairs:
-            if not await anchor_frame.get_by_role(
-                "checkbox", name="I'm not a robot"
-            ).is_checked():
-                return cls(anchor_frame, bframe_frame)
-
-        raise RecaptchaSolveError("No unchecked reCAPTCHA boxes were found.")
-
-    @property
-    def anchor_frame(self) -> AsyncFrame:
-        """The reCAPTCHA anchor frame."""
-        return self._anchor_frame
-
-    @property
-    def bframe_frame(self) -> AsyncFrame:
-        """The reCAPTCHA bframe frame."""
-        return self._bframe_frame
-
-    async def rate_limit_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA rate limit message is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA rate limit message is visible, False otherwise.
-        """
-        return await self.bframe_frame.get_by_text("Try again later").is_visible()
-
-    async def solve_failure_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA solve failure message is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA solve failure message is visible, False otherwise.
-        """
-        return await self.bframe_frame.get_by_text(
-            "Multiple correct solutions required - please solve more."
-        ).is_visible()
-
-    async def audio_challenge_is_visible(self) -> bool:
-        """
-        Check if the reCAPTCHA audio challenge is visible.
-
-        Returns
-        -------
-        bool
-            True if the reCAPTCHA audio challenge is visible, False otherwise.
-        """
-        return await self.bframe_frame.get_by_text("Press PLAY to listen").is_visible()
+from __future__ import annotations
+
+import asyncio
+import re
+from abc import ABC, abstractmethod
+from functools import wraps
+from typing import Awaitable, Callable, Iterable, List, Tuple, Union
+
+from playwright.async_api import Frame as AsyncFrame
+from playwright.async_api import Locator as AsyncLocator
+from playwright.sync_api import Frame as SyncFrame
+from playwright.sync_api import Locator as SyncLocator
+
+from playwright_recaptcha.errors import RecaptchaNotFoundError, RecaptchaSolveError
+
+Locator = Union[AsyncLocator, SyncLocator]
+Frame = Union[AsyncFrame, SyncFrame]
+
+
+class RecaptchaBox(ABC):
+    """
+    The base class for reCAPTCHA v2 boxes.
+
+    Attributes
+    ----------
+    anchor_frame : Frame
+        The reCAPTCHA anchor frame.
+    bframe_frame : Frame
+        The reCAPTCHA bframe frame.
+    checkbox : Locator
+        The reCAPTCHA checkbox locator.
+    audio_challenge_button : Locator
+        The reCAPTCHA audio challenge button locator.
+    new_challenge_button : Locator
+        The reCAPTCHA new challenge button locator.
+    audio_download_button : Locator
+        The reCAPTCHA audio download button locator.
+    audio_challenge_textbox : Locator
+        The reCAPTCHA audio challenge textbox locator.
+    audio_challenge_verify_button : Locator
+        The reCAPTCHA audio challenge verify button locator.
+
+    Methods
+    -------
+    from_frames(frames: Iterable[Frame]) -> Union[AsyncRecaptchaBox, SyncRecaptchaBox]
+        Create a reCAPTCHA box using a list of frames.
+    frames_are_attached() -> bool
+        Check if the reCAPTCHA frames are attached.
+    rate_limit_is_visible() -> bool
+        Check if the reCAPTCHA rate limit message is visible.
+    solve_failure_is_visible() -> bool
+        Check if the reCAPTCHA solve failure message is visible.
+    audio_challenge_is_visible() -> bool
+        Check if the reCAPTCHA audio challenge is visible.
+    is_solved() -> bool
+        Check if the reCAPTCHA challenge is solved.
+
+    Raises
+    ------
+    RecaptchaNotFoundError
+        If the reCAPTCHA was not found.
+    RecaptchaSolveError
+        If no unchecked reCAPTCHA boxes were found.
+    """
+
+    @staticmethod
+    def _get_recaptcha_frame_pairs(
+        frames: Iterable[Frame],
+    ) -> List[Tuple[Frame, Frame]]:
+        """
+        Get the reCAPTCHA anchor and bframe frame pairs.
+
+        Parameters
+        ----------
+        frames : Iterable[Frame]
+            A list of frames to search for the reCAPTCHA anchor and bframe frames.
+
+        Returns
+        -------
+        List[Tuple[Frame, Frame]]
+            A list of reCAPTCHA anchor and bframe frame pairs.
+
+        Raises
+        ------
+        RecaptchaNotFoundError
+            If no reCAPTCHA anchor and bframe frame pairs were found.
+        """
+        anchor_frames = list(
+            filter(
+                lambda frame: re.search(
+                    "/recaptcha/(api2|enterprise)/anchor", frame.url
+                )
+                is not None,
+                frames,
+            )
+        )
+
+        bframe_frames = list(
+            filter(
+                lambda frame: re.search(
+                    "/recaptcha/(api2|enterprise)/bframe", frame.url
+                )
+                is not None,
+                frames,
+            )
+        )
+
+        frame_pairs = []
+
+        for anchor_frame in anchor_frames:
+            frame_id = anchor_frame.name[2:]
+
+            for bframe_frame in bframe_frames:
+                if frame_id in bframe_frame.name:
+                    frame_pairs.append((anchor_frame, bframe_frame))
+
+        if not frame_pairs:
+            raise RecaptchaNotFoundError
+
+        return frame_pairs
+
+    @staticmethod
+    def _check_if_attached(
+        func: Union[
+            Callable[[AsyncRecaptchaBox], Awaitable[bool]],
+            Callable[[SyncRecaptchaBox], bool],
+        ]
+    ) -> Union[
+        Callable[[AsyncRecaptchaBox], Awaitable[bool]],
+        Callable[[SyncRecaptchaBox], bool],
+    ]:
+        """
+        Check if the reCAPTCHA frames are attached before running the decorated function,
+        otherwise return False.
+
+        Parameters
+        ----------
+        func : Union[
+            Callable[[AsyncRecaptchaBox], Awaitable[bool]], Callable[[SyncRecaptchaBox], bool]
+        ]
+            The function to decorate.
+
+        Returns
+        -------
+        Union[
+            Callable[[AsyncRecaptchaBox], Awaitable[bool]], Callable[[SyncRecaptchaBox], bool]
+        ]
+            The decorated function.
+        """
+
+        @wraps(func)
+        def sync_wrapper(self: SyncRecaptchaBox) -> bool:
+            if self.frames_are_detached():
+                return False
+
+            return func(self)
+
+        @wraps(func)
+        async def async_wrapper(self: AsyncRecaptchaBox) -> bool:
+            if self.frames_are_detached():
+                return False
+
+            return await func(self)
+
+        if asyncio.iscoroutinefunction(func):
+            return async_wrapper
+
+        return sync_wrapper
+
+    @property
+    def checkbox(self) -> Locator:
+        """The reCAPTCHA checkbox locator."""
+        return self.anchor_frame.get_by_role("checkbox", name="I'm not a robot")
+
+    @property
+    def audio_challenge_button(self) -> Locator:
+        """The reCAPTCHA audio challenge button locator."""
+        return self.bframe_frame.get_by_role("button", name="Get an audio challenge")
+
+    @property
+    def new_challenge_button(self) -> Locator:
+        """The reCAPTCHA new challenge button locator."""
+        return self.bframe_frame.get_by_role("button", name="Get a new challenge")
+
+    @property
+    def audio_download_button(self) -> Locator:
+        """The reCAPTCHA audio download button locator."""
+        return self.bframe_frame.get_by_role(
+            "link", name="Alternatively, download audio as MP3"
+        )
+
+    @property
+    def audio_challenge_textbox(self) -> Locator:
+        """The reCAPTCHA audio challenge textbox locator."""
+        return self.bframe_frame.get_by_role("textbox", name="Enter what you hear")
+
+    @property
+    def audio_challenge_verify_button(self) -> Locator:
+        """The reCAPTCHA audio challenge verify button locator."""
+        return self.bframe_frame.get_by_role("button", name="Verify")
+
+    def frames_are_attached(self) -> bool:
+        """
+        Check if the reCAPTCHA frames are attached.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA frames are attached, False otherwise.
+        """
+        return (
+            not self.anchor_frame.is_detached() and not self.bframe_frame.is_detached()
+        )
+
+    def frames_are_detached(self) -> bool:
+        """
+        Check if any of the reCAPTCHA frames are detached.
+
+        Returns
+        -------
+        bool
+            True if any of the reCAPTCHA frames are detached, False otherwise.
+        """
+        return self.anchor_frame.is_detached() or self.bframe_frame.is_detached()
+
+    @property
+    @abstractmethod
+    def anchor_frame(self) -> Frame:
+        """The reCAPTCHA anchor frame."""
+
+    @property
+    @abstractmethod
+    def bframe_frame(self) -> Frame:
+        """The reCAPTCHA bframe frame."""
+
+    @classmethod
+    @abstractmethod
+    def from_frames(
+        cls,
+        frames: Iterable[Frame],
+    ) -> Union[AsyncRecaptchaBox, SyncRecaptchaBox]:
+        """
+        Create a reCAPTCHA box using a list of frames.
+
+        Parameters
+        ----------
+        frames : Iterable[Frame]
+            A list of frames to search for the reCAPTCHA frames.
+
+        Returns
+        -------
+        Union[AsyncRecaptchaBox, SyncRecaptchaBox]
+            The reCAPTCHA box.
+
+        Raises
+        ------
+        RecaptchaNotFoundError
+            If the reCAPTCHA frames were not found.
+        RecaptchaSolveError
+            If no unchecked reCAPTCHA boxes were found.
+        """
+
+    @abstractmethod
+    def rate_limit_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA rate limit message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA rate limit message is visible, False otherwise.
+        """
+
+    @abstractmethod
+    def solve_failure_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA solve failure message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA solve failure message is visible, False otherwise.
+        """
+
+    @abstractmethod
+    def audio_challenge_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA audio challenge is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA audio challenge is visible, False otherwise.
+        """
+
+    @abstractmethod
+    def is_solved(self) -> bool:
+        """
+        Check if the reCAPTCHA challenge is solved.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA challenge is solved, False otherwise.
+        """
+
+
+class SyncRecaptchaBox(RecaptchaBox):
+    """
+    The synchronous class for reCAPTCHA v2 boxes.
+
+    Parameters
+    ----------
+    anchor_frame : SyncFrame
+        The reCAPTCHA anchor frame.
+    bframe_frame : SyncFrame
+        The reCAPTCHA bframe frame.
+
+    Attributes
+    ----------
+    anchor_frame : Frame
+        The reCAPTCHA anchor frame.
+    bframe_frame : Frame
+        The reCAPTCHA bframe frame.
+    checkbox : Locator
+        The reCAPTCHA checkbox locator.
+    audio_challenge_button : Locator
+        The reCAPTCHA audio challenge button locator.
+    new_challenge_button : Locator
+        The reCAPTCHA new challenge button locator.
+    audio_download_button : Locator
+        The reCAPTCHA audio download button locator.
+    audio_challenge_textbox : Locator
+        The reCAPTCHA audio challenge textbox locator.
+    audio_challenge_verify_button : Locator
+        The reCAPTCHA audio challenge verify button locator.
+
+    Methods
+    -------
+    from_frames(frames: Iterable[SyncFrame]) -> SyncRecaptchaBox
+        Create a reCAPTCHA box using a list of frames.
+    frames_are_attached() -> bool
+        Check if the reCAPTCHA frames are attached.
+    rate_limit_is_visible() -> bool
+        Check if the reCAPTCHA rate limit message is visible.
+    solve_failure_is_visible() -> bool
+        Check if the reCAPTCHA solve failure message is visible.
+    audio_challenge_is_visible() -> bool
+        Check if the reCAPTCHA audio challenge is visible.
+    is_solved() -> bool
+        Check if the reCAPTCHA challenge is solved.
+
+    Raises
+    ------
+    RecaptchaNotFoundError
+        If the reCAPTCHA was not found.
+    RecaptchaSolveError
+        If no unchecked reCAPTCHA boxes were found.
+    """
+
+    def __init__(self, anchor_frame: SyncFrame, bframe_frame: SyncFrame) -> None:
+        self._anchor_frame = anchor_frame
+        self._bframe_frame = bframe_frame
+
+    def __repr__(self) -> str:
+        return f"SyncRecaptchaBox(anchor_frame={self._anchor_frame!r}, bframe_frame={self._bframe_frame!r})"
+
+    @classmethod
+    def from_frames(cls, frames: Iterable[SyncFrame]) -> SyncRecaptchaBox:
+        """
+        Create a reCAPTCHA box using a list of frames.
+
+        Parameters
+        ----------
+        frames : Iterable[SyncFrame]
+            A list of frames to search for the reCAPTCHA frames.
+
+        Returns
+        -------
+        SyncRecaptchaBox
+            The reCAPTCHA box.
+
+        Raises
+        ------
+        RecaptchaNotFoundError
+            If the reCAPTCHA frames were not found.
+        RecaptchaSolveError
+            If no unchecked reCAPTCHA boxes were found.
+        """
+        frame_pairs = cls._get_recaptcha_frame_pairs(frames)
+
+        for anchor_frame, bframe_frame in frame_pairs:
+            checkbox = anchor_frame.get_by_role("checkbox", name="I'm not a robot")
+
+            if (
+                bframe_frame.get_by_role(
+                    "button", name="Get an audio challenge"
+                ).is_visible()
+                or checkbox.is_visible()
+                and not checkbox.is_checked()
+            ):
+                return cls(anchor_frame, bframe_frame)
+
+        raise RecaptchaSolveError("No unchecked reCAPTCHA boxes were found.")
+
+    @property
+    def anchor_frame(self) -> SyncFrame:
+        """The reCAPTCHA anchor frame."""
+        return self._anchor_frame
+
+    @property
+    def bframe_frame(self) -> SyncFrame:
+        """The reCAPTCHA bframe frame."""
+        return self._bframe_frame
+
+    @RecaptchaBox._check_if_attached
+    def rate_limit_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA rate limit message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA rate limit message is visible, False otherwise.
+        """
+        return self.bframe_frame.get_by_text("Try again later").is_visible()
+
+    @RecaptchaBox._check_if_attached
+    def solve_failure_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA solve failure message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA solve failure message is visible, False otherwise.
+        """
+        return self.bframe_frame.get_by_text(
+            "Multiple correct solutions required - please solve more."
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    def audio_challenge_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA audio challenge is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA audio challenge is visible, False otherwise.
+        """
+        return self.bframe_frame.get_by_text("Press PLAY to listen").is_visible()
+
+    @RecaptchaBox._check_if_attached
+    def is_solved(self) -> bool:
+        """
+        Check if the reCAPTCHA challenge is solved.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA challenge is solved, False otherwise.
+        """
+        return self.checkbox.is_visible() and self.checkbox.is_checked()
+
+
+class AsyncRecaptchaBox(RecaptchaBox):
+    """
+    The asynchronous class for reCAPTCHA v2 boxes.
+
+    Parameters
+    ----------
+    anchor_frame : AsyncFrame
+        The reCAPTCHA anchor frame.
+    bframe_frame : AsyncFrame
+        The reCAPTCHA bframe frame.
+
+    Attributes
+    ----------
+    anchor_frame : Frame
+        The reCAPTCHA anchor frame.
+    bframe_frame : Frame
+        The reCAPTCHA bframe frame.
+    checkbox : Locator
+        The reCAPTCHA checkbox locator.
+    audio_challenge_button : Locator
+        The reCAPTCHA audio challenge button locator.
+    new_challenge_button : Locator
+        The reCAPTCHA new challenge button locator.
+    audio_download_button : Locator
+        The reCAPTCHA audio download button locator.
+    audio_challenge_textbox : Locator
+        The reCAPTCHA audio challenge textbox locator.
+    audio_challenge_verify_button : Locator
+        The reCAPTCHA audio challenge verify button locator.
+
+    Methods
+    -------
+    from_frames(frames: Iterable[AsyncFrame]) -> AsyncRecaptchaBox
+        Create a reCAPTCHA box using a list of frames.
+    frames_are_attached() -> bool
+        Check if the reCAPTCHA frames are attached.
+    rate_limit_is_visible() -> bool
+        Check if the reCAPTCHA rate limit message is visible.
+    solve_failure_is_visible() -> bool
+        Check if the reCAPTCHA solve failure message is visible.
+    audio_challenge_is_visible() -> bool
+        Check if the reCAPTCHA audio challenge is visible.
+    is_solved() -> bool
+        Check if the reCAPTCHA challenge is solved.
+
+    Raises
+    ------
+    RecaptchaNotFoundError
+        If the reCAPTCHA was not found.
+    RecaptchaSolveError
+        If no unchecked reCAPTCHA boxes were found.
+    """
+
+    def __init__(self, anchor_frame: AsyncFrame, bframe_frame: AsyncFrame) -> None:
+        self._anchor_frame = anchor_frame
+        self._bframe_frame = bframe_frame
+
+    def __repr__(self) -> str:
+        return f"AsyncRecaptchaBox(anchor_frame={self._anchor_frame!r}, bframe_frame={self._bframe_frame!r})"
+
+    @classmethod
+    async def from_frames(cls, frames: Iterable[AsyncFrame]) -> AsyncRecaptchaBox:
+        """
+        Create a reCAPTCHA box using a list of frames.
+
+        Parameters
+        ----------
+        frames : Iterable[AsyncFrame]
+            A list of frames to search for the reCAPTCHA frames.
+
+        Returns
+        -------
+        AsyncRecaptchaBox
+            The reCAPTCHA box.
+
+        Raises
+        ------
+        RecaptchaNotFoundError
+            If the reCAPTCHA frames were not found.
+        RecaptchaSolveError
+            If no unchecked reCAPTCHA boxes were found.
+        """
+        frame_pairs = cls._get_recaptcha_frame_pairs(frames)
+
+        for anchor_frame, bframe_frame in frame_pairs:
+            checkbox = anchor_frame.get_by_role("checkbox", name="I'm not a robot")
+
+            if (
+                await bframe_frame.get_by_role(
+                    "button", name="Get an audio challenge"
+                ).is_visible()
+                or await checkbox.is_visible()
+                and not await checkbox.is_checked()
+            ):
+                return cls(anchor_frame, bframe_frame)
+
+        raise RecaptchaSolveError("No unchecked reCAPTCHA boxes were found.")
+
+    @property
+    def anchor_frame(self) -> AsyncFrame:
+        """The reCAPTCHA anchor frame."""
+        return self._anchor_frame
+
+    @property
+    def bframe_frame(self) -> AsyncFrame:
+        """The reCAPTCHA bframe frame."""
+        return self._bframe_frame
+
+    @RecaptchaBox._check_if_attached
+    async def rate_limit_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA rate limit message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA rate limit message is visible, False otherwise.
+        """
+        return await self.bframe_frame.get_by_text("Try again later").is_visible()
+
+    @RecaptchaBox._check_if_attached
+    async def solve_failure_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA solve failure message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA solve failure message is visible, False otherwise.
+        """
+        return await self.bframe_frame.get_by_text(
+            "Multiple correct solutions required - please solve more."
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    async def audio_challenge_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA audio challenge is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA audio challenge is visible, False otherwise.
+        """
+        return await self.bframe_frame.get_by_text("Press PLAY to listen").is_visible()
+
+    @RecaptchaBox._check_if_attached
+    async def is_solved(self) -> bool:
+        """
+        Check if the reCAPTCHA challenge is solved.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA challenge is solved, False otherwise.
+        """
+        return await self.checkbox.is_visible() and await self.checkbox.is_checked()
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav2/sync_solver.py` & `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/sync_solver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,270 +1,289 @@
-from __future__ import annotations
-
-import io
-import random
-import re
-from typing import Any, Optional
-
-import httpx
-import pydub
-import speech_recognition
-from playwright.sync_api import Page, Response
-
-from playwright_recaptcha.errors import (
-    RecaptchaNotFoundError,
-    RecaptchaRateLimitError,
-    RecaptchaSolveError,
-)
-from playwright_recaptcha.recaptchav2.recaptcha_box import SyncRecaptchaBox
-
-
-class SyncSolver:
-    """
-    A class used to solve reCAPTCHA v2 synchronously.
-
-    Parameters
-    ----------
-    page : Page
-        The playwright page to solve the reCAPTCHA on.
-    attempts : int, optional
-        The number of solve attempts, by default 3.
-
-    Attributes
-    ----------
-    token : Optional[str]
-        The g-recaptcha-response token.
-
-    Methods
-    -------
-    close() -> None
-        Remove the userverify response listener.
-    solve_recaptcha(attempts: Optional[int] = None) -> str
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaRateLimitError
-        If the reCAPTCHA rate limit has been exceeded.
-    RecaptchaSolveError
-        If the reCAPTCHA could not be solved.
-    """
-
-    def __init__(self, page: Page, attempts: int = 3) -> None:
-        self._page = page
-        self._attempts = attempts
-        self.token: Optional[str] = None
-
-    def __repr__(self) -> str:
-        return f"SyncSolver(page={self._page!r}, attempts={self._attempts!r})"
-
-    def __enter__(self) -> SyncSolver:
-        return self
-
-    def __exit__(self, *args: Any) -> None:
-        self.close()
-
-    @staticmethod
-    def _convert_audio_to_text(audio_url: str) -> Optional[str]:
-        """
-        Convert the reCAPTCHA audio to text.
-
-        Parameters
-        ----------
-        audio_url : str
-            The reCAPTCHA audio URL.
-
-        Returns
-        -------
-        Optional[str]
-            The reCAPTCHA audio text.
-        """
-        response = httpx.get(audio_url)
-
-        wav_audio = io.BytesIO()
-        mp3_audio = io.BytesIO(response.content)
-        audio = pydub.AudioSegment.from_mp3(mp3_audio)
-        audio.export(wav_audio, format="wav")
-
-        recognizer = speech_recognition.Recognizer()
-
-        with speech_recognition.AudioFile(wav_audio) as source:
-            audio_data = recognizer.record(source)
-
-        try:
-            return recognizer.recognize_google(audio_data)
-        except speech_recognition.UnknownValueError:
-            return None
-
-    def _random_delay(self) -> None:
-        """Delay the execution for a random amount of time between 1 and 4 seconds."""
-        self._page.wait_for_timeout(random.randint(1000, 4000))
-
-    def _extract_token(self, response: Response) -> None:
-        """
-        Extract the g-recaptcha-response token from the userverify response.
-
-        Parameters
-        ----------
-        response : Response
-            The response to extract the g-recaptcha-response token from.
-        """
-        if re.search("/recaptcha/(api2|enterprise)/userverify", response.url) is None:
-            return
-
-        token_match = re.search('"uvresp","(.*?)"', response.text())
-
-        if token_match is not None:
-            self.token = token_match.group(1)
-
-    def _get_audio_url(self, recaptcha_box: SyncRecaptchaBox) -> str:
-        """
-        Get the reCAPTCHA audio URL.
-
-        Parameters
-        ----------
-        recaptcha_box : SyncRecaptchaBox
-            The reCAPTCHA box.
-
-        Returns
-        -------
-        str
-            The reCAPTCHA audio URL.
-
-        Raises
-        ------
-        RecaptchaRateLimitError
-            If the reCAPTCHA rate limit has been exceeded.
-        """
-        if recaptcha_box.audio_challenge_button.is_visible():
-            recaptcha_box.audio_challenge_button.click(force=True)
-
-        while True:
-            if recaptcha_box.audio_challenge_is_visible():
-                break
-
-            if recaptcha_box.rate_limit_is_visible():
-                raise RecaptchaRateLimitError
-
-            self._page.wait_for_timeout(100)
-
-        return recaptcha_box.audio_download_button.get_attribute("href")
-
-    def _submit_audio_text(self, recaptcha_box: SyncRecaptchaBox, text: str) -> None:
-        """
-        Submit the reCAPTCHA audio text.
-
-        Parameters
-        ----------
-        recaptcha_box : SyncRecaptchaBox
-            The reCAPTCHA box.
-        text : str
-            The reCAPTCHA audio text.
-
-        Raises
-        ------
-        RecaptchaRateLimitError
-            If the reCAPTCHA rate limit has been exceeded.
-        """
-        recaptcha_box.audio_challenge_textbox.fill(text)
-        recaptcha_box.audio_challenge_verify_button.click()
-
-        while recaptcha_box.frames_are_attached():
-            if (
-                recaptcha_box.checkbox.is_checked()
-                or recaptcha_box.solve_failure_is_visible()
-            ):
-                break
-
-            if recaptcha_box.rate_limit_is_visible():
-                raise RecaptchaRateLimitError
-
-            self._page.wait_for_timeout(100)
-
-    def close(self) -> None:
-        """Remove the userverify response listener."""
-        try:
-            self._page.remove_listener("response", self._extract_token)
-        except KeyError:
-            pass
-
-    def solve_recaptcha(self, attempts: Optional[int] = None) -> str:
-        """
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-        Parameters
-        ----------
-        attempts : Optional[int], optional
-            The number of solve attempts, by default 3.
-
-        Returns
-        -------
-        str
-            The g-recaptcha-response token.
-
-        Raises
-        ------
-        RecaptchaNotFoundError
-            If the reCAPTCHA was not found.
-        RecaptchaRateLimitError
-            If the reCAPTCHA rate limit has been exceeded.
-        RecaptchaSolveError
-            If the reCAPTCHA could not be solved.
-        """
-        self.token = None
-        self._page.on("response", self._extract_token)
-
-        attempts = attempts or self._attempts
-        recaptcha_box = SyncRecaptchaBox.from_frames(self._page.frames)
-
-        if recaptcha_box.checkbox.is_hidden():
-            raise RecaptchaNotFoundError
-
-        recaptcha_box.checkbox.click(force=True)
-
-        while True:
-            if (
-                recaptcha_box.audio_challenge_is_visible()
-                or recaptcha_box.audio_challenge_button.is_visible()
-                and recaptcha_box.audio_challenge_button.is_enabled()
-            ):
-                break
-
-            if (
-                not recaptcha_box.frames_are_attached()
-                or recaptcha_box.checkbox.is_checked()
-            ):
-                if self.token is None:
-                    raise RecaptchaSolveError
-
-                return self.token
-
-            self._page.wait_for_timeout(100)
-
-        while attempts > 0:
-            self._random_delay()
-            url = self._get_audio_url(recaptcha_box)
-            text = self._convert_audio_to_text(url)
-
-            if text is None:
-                recaptcha_box.new_challenge_button.click()
-                attempts -= 1
-                continue
-
-            self._random_delay()
-            self._submit_audio_text(recaptcha_box, text)
-
-            if (
-                not recaptcha_box.frames_are_attached()
-                or recaptcha_box.checkbox.is_checked()
-            ):
-                if self.token is None:
-                    raise RecaptchaSolveError
-
-                return self.token
-
-            recaptcha_box.new_challenge_button.click()
-            attempts -= 1
-
-        raise RecaptchaSolveError
+from __future__ import annotations
+
+import io
+import random
+import re
+from typing import Any, Optional
+
+import pydub
+import speech_recognition
+from playwright.sync_api import Page, Response
+
+from playwright_recaptcha.errors import (
+    RecaptchaNotFoundError,
+    RecaptchaRateLimitError,
+    RecaptchaSolveError,
+)
+from playwright_recaptcha.recaptchav2.recaptcha_box import SyncRecaptchaBox
+
+
+class SyncSolver:
+    """
+    A class used to solve reCAPTCHA v2 synchronously.
+
+    Parameters
+    ----------
+    page : Page
+        The playwright page to solve the reCAPTCHA on.
+    attempts : int, optional
+        The number of solve attempts, by default 3.
+
+    Attributes
+    ----------
+    token : Optional[str]
+        The g-recaptcha-response token.
+
+    Methods
+    -------
+    close() -> None
+        Remove the userverify response listener.
+    solve_recaptcha(attempts: Optional[int] = None) -> str
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+    Raises
+    ------
+    RecaptchaNotFoundError
+        If the reCAPTCHA was not found.
+    RecaptchaRateLimitError
+        If the reCAPTCHA rate limit has been exceeded.
+    RecaptchaSolveError
+        If the reCAPTCHA could not be solved.
+    """
+
+    def __init__(self, page: Page, attempts: int = 3) -> None:
+        self._page = page
+        self._attempts = attempts
+        self.token: Optional[str] = None
+
+    def __repr__(self) -> str:
+        return f"SyncSolver(page={self._page!r}, attempts={self._attempts!r})"
+
+    def __enter__(self) -> SyncSolver:
+        return self
+
+    def __exit__(self, *args: Any) -> None:
+        self.close()
+
+    def _convert_audio_to_text(self, audio_url: str) -> Optional[str]:
+        """
+        Convert the reCAPTCHA audio to text.
+
+        Parameters
+        ----------
+        audio_url : str
+            The reCAPTCHA audio URL.
+
+        Returns
+        -------
+        Optional[str]
+            The reCAPTCHA audio text.
+        """
+        response = self._page.request.get(audio_url)
+
+        wav_audio = io.BytesIO()
+        mp3_audio = io.BytesIO(response.body())
+        audio = pydub.AudioSegment.from_mp3(mp3_audio)
+        audio.export(wav_audio, format="wav")
+
+        recognizer = speech_recognition.Recognizer()
+
+        with speech_recognition.AudioFile(wav_audio) as source:
+            audio_data = recognizer.record(source)
+
+        try:
+            return recognizer.recognize_google(audio_data)
+        except speech_recognition.UnknownValueError:
+            return None
+
+    def _random_delay(self) -> None:
+        """Delay the execution for a random amount of time between 1 and 4 seconds."""
+        self._page.wait_for_timeout(random.randint(1000, 4000))
+
+    def _extract_token(self, response: Response) -> None:
+        """
+        Extract the g-recaptcha-response token from the userverify response.
+
+        Parameters
+        ----------
+        response : Response
+            The response to extract the g-recaptcha-response token from.
+        """
+        if re.search("/recaptcha/(api2|enterprise)/userverify", response.url) is None:
+            return
+
+        token_match = re.search('"uvresp","(.*?)"', response.text())
+
+        if token_match is not None:
+            self.token = token_match.group(1)
+
+    def _click_checkbox(self, recaptcha_box: SyncRecaptchaBox) -> None:
+        """
+        Click the reCAPTCHA checkbox.
+
+        Parameters
+        ----------
+        recaptcha_box : SyncRecaptchaBox
+            The reCAPTCHA box.
+        """
+        recaptcha_box.checkbox.click(force=True)
+
+        while recaptcha_box.frames_are_attached():
+            if recaptcha_box.is_solved():
+                if self.token is None:
+                    raise RecaptchaSolveError
+
+                break
+
+            if (
+                recaptcha_box.audio_challenge_is_visible()
+                or recaptcha_box.audio_challenge_button.is_visible()
+                and recaptcha_box.audio_challenge_button.is_enabled()
+            ):
+                break
+
+            self._page.wait_for_timeout(250)
+
+    def _get_audio_url(self, recaptcha_box: SyncRecaptchaBox) -> str:
+        """
+        Get the reCAPTCHA audio URL.
+
+        Parameters
+        ----------
+        recaptcha_box : SyncRecaptchaBox
+            The reCAPTCHA box.
+
+        Returns
+        -------
+        str
+            The reCAPTCHA audio URL.
+
+        Raises
+        ------
+        RecaptchaRateLimitError
+            If the reCAPTCHA rate limit has been exceeded.
+        """
+        if recaptcha_box.audio_challenge_button.is_visible():
+            recaptcha_box.audio_challenge_button.click(force=True)
+
+        while True:
+            if recaptcha_box.rate_limit_is_visible():
+                raise RecaptchaRateLimitError
+
+            if recaptcha_box.audio_challenge_is_visible():
+                break
+
+            self._page.wait_for_timeout(250)
+
+        return recaptcha_box.audio_download_button.get_attribute("href")
+
+    def _submit_audio_text(self, recaptcha_box: SyncRecaptchaBox, text: str) -> None:
+        """
+        Submit the reCAPTCHA audio text.
+
+        Parameters
+        ----------
+        recaptcha_box : SyncRecaptchaBox
+            The reCAPTCHA box.
+        text : str
+            The reCAPTCHA audio text.
+
+        Raises
+        ------
+        RecaptchaRateLimitError
+            If the reCAPTCHA rate limit has been exceeded.
+        """
+        recaptcha_box.audio_challenge_textbox.fill(text)
+
+        with self._page.expect_response(
+            re.compile("/recaptcha/(api2|enterprise)/userverify")
+        ):
+            recaptcha_box.audio_challenge_verify_button.click()
+
+        while recaptcha_box.frames_are_attached():
+            if recaptcha_box.rate_limit_is_visible():
+                raise RecaptchaRateLimitError
+
+            if (
+                recaptcha_box.new_challenge_button.is_disabled()
+                or recaptcha_box.solve_failure_is_visible()
+                or recaptcha_box.is_solved()
+            ):
+                break
+
+            self._page.wait_for_timeout(250)
+
+    def close(self) -> None:
+        """Remove the userverify response listener."""
+        try:
+            self._page.remove_listener("response", self._extract_token)
+        except KeyError:
+            pass
+
+    def solve_recaptcha(self, attempts: Optional[int] = None) -> str:
+        """
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+        Parameters
+        ----------
+        attempts : Optional[int], optional
+            The number of solve attempts, by default 3.
+
+        Returns
+        -------
+        str
+            The g-recaptcha-response token.
+
+        Raises
+        ------
+        RecaptchaNotFoundError
+            If the reCAPTCHA was not found.
+        RecaptchaRateLimitError
+            If the reCAPTCHA rate limit has been exceeded.
+        RecaptchaSolveError
+            If the reCAPTCHA could not be solved.
+        """
+        self.token = None
+        self._page.on("response", self._extract_token)
+
+        attempts = attempts or self._attempts
+        recaptcha_box = SyncRecaptchaBox.from_frames(self._page.frames)
+
+        if (
+            recaptcha_box.checkbox.is_hidden()
+            and recaptcha_box.audio_challenge_button.is_disabled()
+        ):
+            raise RecaptchaNotFoundError
+
+        if recaptcha_box.checkbox.is_visible():
+            self._click_checkbox(recaptcha_box)
+
+            if self.token is not None:
+                return self.token
+
+        while attempts > 0:
+            self._random_delay()
+            url = self._get_audio_url(recaptcha_box)
+            text = self._convert_audio_to_text(url)
+
+            if text is None:
+                recaptcha_box.new_challenge_button.click()
+                attempts -= 1
+                continue
+
+            self._random_delay()
+            self._submit_audio_text(recaptcha_box, text)
+
+            if (
+                recaptcha_box.frames_are_detached()
+                or recaptcha_box.new_challenge_button.is_disabled()
+                or recaptcha_box.is_solved()
+            ):
+                if self.token is None:
+                    raise RecaptchaSolveError
+
+                return self.token
+
+            recaptcha_box.new_challenge_button.click()
+            attempts -= 1
+
+        raise RecaptchaSolveError
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav3/async_solver.py` & `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/async_solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from __future__ import annotations
-
-import re
-import time
-from typing import Any, Optional
-
-from playwright.async_api import Page, Response
-
-from playwright_recaptcha.errors import RecaptchaTimeoutError
-
-
-class AsyncSolver:
-    """
-    A class used to solve reCAPTCHA v3 asynchronously.
-
-    Parameters
-    ----------
-    page : Page
-        The playwright page to solve the reCAPTCHA on.
-    timeout : int, optional
-        The solve timeout in seconds, by default 30.
-
-    Attributes
-    ----------
-    token : Optional[str]
-        The g-recaptcha-response token.
-
-    Methods
-    -------
-    close() -> None
-        Remove the reload response listener.
-    solve_recaptcha(timeout: Optional[int] = None) -> str
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-    Raises
-    ------
-    RecaptchaTimeoutError
-        If the solve timeout has been exceeded.
-    """
-
-    def __init__(self, page: Page, timeout: int = 30) -> None:
-        self._page = page
-        self._timeout = timeout
-        self.token: Optional[str] = None
-
-    def __repr__(self) -> str:
-        return f"AsyncSolver(page={self._page!r}, timeout={self._timeout!r})"
-
-    async def __aenter__(self) -> AsyncSolver:
-        return self
-
-    async def __aexit__(self, *args: Any) -> None:
-        self.close()
-
-    async def _extract_token(self, response: Response) -> None:
-        """
-        Extract the g-recaptcha-response token from the userverify response.
-
-        Parameters
-        ----------
-        response : Response
-            The response to extract the g-recaptcha-response token from.
-        """
-        if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
-            return
-
-        token_match = re.search('"rresp","(.*?)"', await response.text())
-
-        if token_match is not None:
-            self.token = token_match.group(1)
-
-    def close(self) -> None:
-        """Remove the reload response listener."""
-        try:
-            self._page.remove_listener("response", self._extract_token)
-        except KeyError:
-            pass
-
-    async def solve_recaptcha(self, timeout: Optional[int] = None) -> str:
-        """
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-        Parameters
-        ----------
-        timeout : Optional[int], optional
-            The solve timeout in seconds, by default 30.
-
-        Returns
-        -------
-        str
-            The g-recaptcha-response token.
-
-        Raises
-        ------
-        RecaptchaTimeoutError
-            If the solve timeout has been exceeded.
-        """
-        self.token = None
-        self._page.on("response", self._extract_token)
-
-        timeout = timeout or self._timeout
-        start_time = time.time()
-
-        while self.token is None:
-            if time.time() - start_time >= timeout:
-                raise RecaptchaTimeoutError
-
-            await self._page.wait_for_timeout(100)
-
-        return self.token
+from __future__ import annotations
+
+import re
+import time
+from typing import Any, Optional
+
+from playwright.async_api import Page, Response
+
+from playwright_recaptcha.errors import RecaptchaTimeoutError
+
+
+class AsyncSolver:
+    """
+    A class used to solve reCAPTCHA v3 asynchronously.
+
+    Parameters
+    ----------
+    page : Page
+        The playwright page to solve the reCAPTCHA on.
+    timeout : int, optional
+        The solve timeout in seconds, by default 30.
+
+    Attributes
+    ----------
+    token : Optional[str]
+        The g-recaptcha-response token.
+
+    Methods
+    -------
+    close() -> None
+        Remove the reload response listener.
+    solve_recaptcha(timeout: Optional[int] = None) -> str
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+    Raises
+    ------
+    RecaptchaTimeoutError
+        If the solve timeout has been exceeded.
+    """
+
+    def __init__(self, page: Page, timeout: int = 30) -> None:
+        self._page = page
+        self._timeout = timeout
+        self.token: Optional[str] = None
+
+    def __repr__(self) -> str:
+        return f"AsyncSolver(page={self._page!r}, timeout={self._timeout!r})"
+
+    async def __aenter__(self) -> AsyncSolver:
+        return self
+
+    async def __aexit__(self, *args: Any) -> None:
+        self.close()
+
+    async def _extract_token(self, response: Response) -> None:
+        """
+        Extract the g-recaptcha-response token from the userverify response.
+
+        Parameters
+        ----------
+        response : Response
+            The response to extract the g-recaptcha-response token from.
+        """
+        if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
+            return
+
+        token_match = re.search('"rresp","(.*?)"', await response.text())
+
+        if token_match is not None:
+            self.token = token_match.group(1)
+
+    def close(self) -> None:
+        """Remove the reload response listener."""
+        try:
+            self._page.remove_listener("response", self._extract_token)
+        except KeyError:
+            pass
+
+    async def solve_recaptcha(self, timeout: Optional[int] = None) -> str:
+        """
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+        Parameters
+        ----------
+        timeout : Optional[int], optional
+            The solve timeout in seconds, by default 30.
+
+        Returns
+        -------
+        str
+            The g-recaptcha-response token.
+
+        Raises
+        ------
+        RecaptchaTimeoutError
+            If the solve timeout has been exceeded.
+        """
+        self.token = None
+        self._page.on("response", self._extract_token)
+
+        timeout = timeout or self._timeout
+        start_time = time.time()
+
+        while self.token is None:
+            if time.time() - start_time >= timeout:
+                raise RecaptchaTimeoutError
+
+            await self._page.wait_for_timeout(250)
+
+        return self.token
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha/recaptchav3/sync_solver.py` & `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/sync_solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from __future__ import annotations
-
-import re
-import time
-from typing import Any, Optional
-
-from playwright.sync_api import Page, Response
-
-from playwright_recaptcha.errors import RecaptchaTimeoutError
-
-
-class SyncSolver:
-    """
-    A class used to solve reCAPTCHA v3 synchronously.
-
-    Parameters
-    ----------
-    page : Page
-        The playwright page to solve the reCAPTCHA on.
-    timeout : int, optional
-        The solve timeout in seconds, by default 30.
-
-    Attributes
-    ----------
-    token : Optional[str]
-        The g-recaptcha-response token.
-
-    Methods
-    -------
-    close() -> None
-        Remove the reload response listener.
-    solve_recaptcha(timeout: Optional[int] = None) -> str
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-    Raises
-    ------
-    RecaptchaTimeoutError
-        If the solve timeout has been exceeded.
-    """
-
-    def __init__(self, page: Page, timeout: int = 30) -> None:
-        self._page = page
-        self._timeout = timeout
-        self.token: Optional[str] = None
-
-    def __repr__(self) -> str:
-        return f"SyncSolver(page={self._page!r}, timeout={self._timeout!r})"
-
-    def __enter__(self) -> SyncSolver:
-        return self
-
-    def __exit__(self, *args: Any) -> None:
-        self.close()
-
-    def _extract_token(self, response: Response) -> None:
-        """
-        Extract the g-recaptcha-response token from the userverify response.
-
-        Parameters
-        ----------
-        response : Response
-            The response to extract the g-recaptcha-response token from.
-        """
-        if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
-            return
-
-        token_match = re.search('"rresp","(.*?)"', response.text())
-
-        if token_match is not None:
-            self.token = token_match.group(1)
-
-    def close(self) -> None:
-        """Remove the reload response listener."""
-        try:
-            self._page.remove_listener("response", self._extract_token)
-        except KeyError:
-            pass
-
-    def solve_recaptcha(self, timeout: Optional[int] = None) -> str:
-        """
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-        Parameters
-        ----------
-        timeout : Optional[int], optional
-            The solve timeout in seconds, by default 30.
-
-        Returns
-        -------
-        str
-            The g-recaptcha-response token.
-
-        Raises
-        ------
-        RecaptchaTimeoutError
-            If the solve timeout has been exceeded.
-        """
-        self.token = None
-        self._page.on("response", self._extract_token)
-
-        timeout = timeout or self._timeout
-        start_time = time.time()
-
-        while self.token is None:
-            if time.time() - start_time >= timeout:
-                raise RecaptchaTimeoutError
-
-            self._page.wait_for_timeout(100)
-
-        return self.token
+from __future__ import annotations
+
+import re
+import time
+from typing import Any, Optional
+
+from playwright.sync_api import Page, Response
+
+from playwright_recaptcha.errors import RecaptchaTimeoutError
+
+
+class SyncSolver:
+    """
+    A class used to solve reCAPTCHA v3 synchronously.
+
+    Parameters
+    ----------
+    page : Page
+        The playwright page to solve the reCAPTCHA on.
+    timeout : int, optional
+        The solve timeout in seconds, by default 30.
+
+    Attributes
+    ----------
+    token : Optional[str]
+        The g-recaptcha-response token.
+
+    Methods
+    -------
+    close() -> None
+        Remove the reload response listener.
+    solve_recaptcha(timeout: Optional[int] = None) -> str
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+    Raises
+    ------
+    RecaptchaTimeoutError
+        If the solve timeout has been exceeded.
+    """
+
+    def __init__(self, page: Page, timeout: int = 30) -> None:
+        self._page = page
+        self._timeout = timeout
+        self.token: Optional[str] = None
+
+    def __repr__(self) -> str:
+        return f"SyncSolver(page={self._page!r}, timeout={self._timeout!r})"
+
+    def __enter__(self) -> SyncSolver:
+        return self
+
+    def __exit__(self, *args: Any) -> None:
+        self.close()
+
+    def _extract_token(self, response: Response) -> None:
+        """
+        Extract the g-recaptcha-response token from the userverify response.
+
+        Parameters
+        ----------
+        response : Response
+            The response to extract the g-recaptcha-response token from.
+        """
+        if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
+            return
+
+        token_match = re.search('"rresp","(.*?)"', response.text())
+
+        if token_match is not None:
+            self.token = token_match.group(1)
+
+    def close(self) -> None:
+        """Remove the reload response listener."""
+        try:
+            self._page.remove_listener("response", self._extract_token)
+        except KeyError:
+            pass
+
+    def solve_recaptcha(self, timeout: Optional[int] = None) -> str:
+        """
+        Solve the reCAPTCHA and return the g-recaptcha-response token.
+
+        Parameters
+        ----------
+        timeout : Optional[int], optional
+            The solve timeout in seconds, by default 30.
+
+        Returns
+        -------
+        str
+            The g-recaptcha-response token.
+
+        Raises
+        ------
+        RecaptchaTimeoutError
+            If the solve timeout has been exceeded.
+        """
+        self.token = None
+        self._page.on("response", self._extract_token)
+
+        timeout = timeout or self._timeout
+        start_time = time.time()
+
+        while self.token is None:
+            if time.time() - start_time >= timeout:
+                raise RecaptchaTimeoutError
+
+            self._page.wait_for_timeout(250)
+
+        return self.token
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/PKG-INFO` & `playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-Metadata-Version: 2.1
-Name: playwright-recaptcha
-Version: 0.1.3
-Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
-Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
-Author: Xewdy444
-Author-email: xewdy@xewdy.tech
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
-Classifier: Framework :: AsyncIO
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![PyPI](https://img.shields.io/pypi/v/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
-[![Downloads](https://img.shields.io/pypi/dm/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
-[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Xewdy444/Playwright-reCAPTCHA/blob/main/LICENSE)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-# Playwright-reCAPTCHA
-A Python library for solving reCAPTCHA v2 and v3 with Playwright.
-
-## Solving reCAPTCHA v2
-reCAPTCHA v2 is solved by transcribing the audio challenge using the Google speech recognition API and entering the text as the response.
-
-## Solving reCAPTCHA v3
-The solving of reCAPTCHA v3 is done by the browser itself, so this library simply waits for the browser to make a POST request to https://www.google.com/recaptcha/api2/reload or https://www.google.com/recaptcha/enterprise/reload and parses the response to get the `g-recaptcha-response` token.
-
----
-
-All solvers return the `g-recaptcha-response` token, which is required for form submissions.
-
-It's important to note that reCAPTCHA v3 uses a token-based scoring system. Each user's token is automatically assigned a score based on their interactions with the website. The score is used to determine the likelihood of the user being a human or a bot. The token is then passed to the web server, and the website owner decides what action to take based on the score.
-
-# Installation
-```
-pip install playwright-recaptcha
-```
-
-This library requires FFmpeg to be installed on your system in order to convert the audio challenge from reCAPTCHA v2 into text.
-
-|   OS    |           Command           |
-| :-----: | :-------------------------: |
-| Debian  | sudo apt-get install ffmpeg |
-|  MacOS  |     brew install ffmpeg     |
-| Windows |    choco install ffmpeg     |
-
-You can also download the latest static build from [here](https://ffmpeg.org/download.html).
-
-> **Note**
-> Make sure to have the ffmpeg and ffprobe binaries in your system's PATH so that the SpeechRecognition library can find them.
-
-# Examples
-
-## reCAPTCHA v2
-
-### Synchronous
-```py
-from playwright.sync_api import sync_playwright
-from playwright_recaptcha import recaptchav2
-
-with sync_playwright() as playwright:
-    browser = playwright.firefox.launch()
-    page = browser.new_page()
-
-    page.goto(
-        "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-    )
-
-    with recaptchav2.SyncSolver(page) as solver:
-        token = solver.solve_recaptcha()
-        print(token)
-```
-
-### Asynchronous
-```py
-import asyncio
-from playwright.async_api import async_playwright
-from playwright_recaptcha import recaptchav2
-
-async def main() -> None:
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
-
-        async with recaptchav2.AsyncSolver(page) as solver:
-            token = await solver.solve_recaptcha()
-            print(token)
-
-asyncio.run(main())
-```
-
-## reCAPTCHA v3
-
-### Synchronous
-```py
-from playwright.sync_api import sync_playwright
-from playwright_recaptcha import recaptchav3
-
-with sync_playwright() as playwright:
-    browser = playwright.firefox.launch()
-    page = browser.new_page()
-    page.goto("https://antcpt.com/score_detector/")
-
-    with recaptchav3.SyncSolver(page) as solver:
-        token = solver.solve_recaptcha()
-        print(token)
-```
-
-### Asynchronous
-```py
-import asyncio
-from playwright.async_api import async_playwright
-from playwright_recaptcha import recaptchav3
-
-async def main() -> None:
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-        await page.goto("https://antcpt.com/score_detector/")
-
-        async with recaptchav3.AsyncSolver(page) as solver:
-            token = await solver.solve_recaptcha()
-            print(token)
-
-asyncio.run(main())
-```
-
-# Exceptions
-|        Exception        |                                                                      Description                                                                      |
-| :---------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
-|     RecaptchaError      |                            The base class for reCAPTCHA exceptions, used as a catch-all for any reCAPTCHA-related errors.                             |
-|   RecaptchaSolveError   |                An exception raised when the reCAPTCHA could not be solved, used as a catch-all for any reCAPTCHA solve-related errors.                |
-| RecaptchaNotFoundError  |                                        An exception raised when the reCAPTCHA v2 was not found on the website.                                        |
-| RecaptchaRateLimitError | An exception raised when the reCAPTCHA rate limit has been exceeded. This can happen if the library is being used to solve reCAPTCHA v2s too quickly. |
-|  RecaptchaTimeoutError  |                                An exception raised when the reCAPTCHA v3 was not solved within the specified timeout.                                 |
-
-# Disclaimer
-This library is intended for use in automated testing and development environments only and should not be used for any illegal or malicious purposes. Any use of this library for activities that violate the terms of service of any website or service is strictly prohibited. The contributors of this library will not be held liable for any damages or legal issues that may arise from the use of this library. By using this library, you agree to these terms and take full responsibility for your actions.
+Metadata-Version: 2.1
+Name: playwright-recaptcha
+Version: 0.2.0
+Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
+Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
+Author: Xewdy444
+Author-email: xewdy@xewdy.tech
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
+Classifier: Framework :: AsyncIO
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![PyPI](https://img.shields.io/pypi/v/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
+[![Downloads](https://img.shields.io/pypi/dm/playwright-recaptcha.svg)](https://pypi.org/project/playwright-recaptcha/)
+[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Xewdy444/Playwright-reCAPTCHA/blob/main/LICENSE)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# Playwright-reCAPTCHA
+A Python library for solving reCAPTCHA v2 and v3 with Playwright.
+
+## Solving reCAPTCHA v2
+reCAPTCHA v2 is solved by transcribing the audio challenge using the Google speech recognition API and entering the text as the response.
+
+## Solving reCAPTCHA v3
+The solving of reCAPTCHA v3 is done by the browser itself, so this library simply waits for the browser to make a POST request to https://www.google.com/recaptcha/api2/reload or https://www.google.com/recaptcha/enterprise/reload and parses the response to get the `g-recaptcha-response` token.
+
+---
+
+All solvers return the `g-recaptcha-response` token, which is required for form submissions.
+
+It's important to note that reCAPTCHA v3 uses a token-based scoring system. Each user's token is automatically assigned a score based on their interactions with the website. The score is used to determine the likelihood of the user being a human or a bot. The token is then passed to the web server, and the website owner decides what action to take based on the score.
+
+# Installation
+```
+pip install playwright-recaptcha
+```
+
+This library requires FFmpeg to be installed on your system in order to convert the audio challenge from reCAPTCHA v2 into text.
+
+|   OS    |           Command           |
+| :-----: | :-------------------------: |
+| Debian  | sudo apt-get install ffmpeg |
+|  MacOS  |     brew install ffmpeg     |
+| Windows |    choco install ffmpeg     |
+
+You can also download the latest static build from [here](https://ffmpeg.org/download.html).
+
+> **Note**
+> Make sure to have the ffmpeg and ffprobe binaries in your system's PATH so that the SpeechRecognition library can find them.
+
+# Examples
+
+## reCAPTCHA v2
+
+### Synchronous
+```py
+from playwright.sync_api import sync_playwright
+from playwright_recaptcha import recaptchav2
+
+with sync_playwright() as playwright:
+    browser = playwright.firefox.launch()
+    page = browser.new_page()
+
+    page.goto(
+        "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+    )
+
+    with recaptchav2.SyncSolver(page) as solver:
+        token = solver.solve_recaptcha()
+        print(token)
+```
+
+### Asynchronous
+```py
+import asyncio
+from playwright.async_api import async_playwright
+from playwright_recaptcha import recaptchav2
+
+async def main() -> None:
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+
+        await page.goto(
+            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+        )
+
+        async with recaptchav2.AsyncSolver(page) as solver:
+            token = await solver.solve_recaptcha()
+            print(token)
+
+asyncio.run(main())
+```
+
+## reCAPTCHA v3
+
+### Synchronous
+```py
+from playwright.sync_api import sync_playwright
+from playwright_recaptcha import recaptchav3
+
+with sync_playwright() as playwright:
+    browser = playwright.firefox.launch()
+    page = browser.new_page()
+    page.goto("https://antcpt.com/score_detector/")
+
+    with recaptchav3.SyncSolver(page) as solver:
+        token = solver.solve_recaptcha()
+        print(token)
+```
+
+### Asynchronous
+```py
+import asyncio
+from playwright.async_api import async_playwright
+from playwright_recaptcha import recaptchav3
+
+async def main() -> None:
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+        await page.goto("https://antcpt.com/score_detector/")
+
+        async with recaptchav3.AsyncSolver(page) as solver:
+            token = await solver.solve_recaptcha()
+            print(token)
+
+asyncio.run(main())
+```
+
+# Exceptions
+|        Exception        |                                                                      Description                                                                      |
+| :---------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
+|     RecaptchaError      |                            The base class for reCAPTCHA exceptions, used as a catch-all for any reCAPTCHA-related errors.                             |
+|   RecaptchaSolveError   |                An exception raised when the reCAPTCHA could not be solved, used as a catch-all for any reCAPTCHA solve-related errors.                |
+| RecaptchaNotFoundError  |                                        An exception raised when the reCAPTCHA v2 was not found on the website.                                        |
+| RecaptchaRateLimitError | An exception raised when the reCAPTCHA rate limit has been exceeded. This can happen if the library is being used to solve reCAPTCHA v2s too quickly. |
+|  RecaptchaTimeoutError  |                                An exception raised when the reCAPTCHA v3 was not solved within the specified timeout.                                 |
+
+# Disclaimer
+This library is intended for use in automated testing and development environments only and should not be used for any illegal or malicious purposes. Any use of this library for activities that violate the terms of service of any website or service is strictly prohibited. The contributors of this library will not be held liable for any damages or legal issues that may arise from the use of this library. By using this library, you agree to these terms and take full responsibility for your actions.
```

### Comparing `playwright-recaptcha-0.1.3/playwright_recaptcha.egg-info/SOURCES.txt` & `playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.1.3/setup.py` & `playwright-recaptcha-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from setuptools import find_packages, setup
-
-with open("README.md", encoding="utf-8") as file:
-    long_description = file.read()
-
-setup(
-    name="playwright-recaptcha",
-    version="0.1.3",
-    author="Xewdy444",
-    author_email="xewdy@xewdy.tech",
-    description="A library for solving reCAPTCHA v2 and v3 with Playwright",
-    license="MIT",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Xewdy444/Playwright-reCAPTCHA",
-    packages=find_packages(),
-    python_requires=">=3.8",
-    install_requires=[
-        "httpx==0.23.3",
-        "playwright==1.31.1",
-        "pydub==0.25.1",
-        "SpeechRecognition==3.10.0",
-    ],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Testing",
-        "Topic :: Internet :: WWW/HTTP :: Browsers",
-        "Framework :: AsyncIO",
-    ],
-)
+from setuptools import find_packages, setup
+
+with open("README.md", encoding="utf-8") as file:
+    long_description = file.read()
+
+setup(
+    name="playwright-recaptcha",
+    version="0.2.0",
+    author="Xewdy444",
+    author_email="xewdy@xewdy.tech",
+    description="A library for solving reCAPTCHA v2 and v3 with Playwright",
+    license="MIT",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Xewdy444/Playwright-reCAPTCHA",
+    packages=find_packages(),
+    python_requires=">=3.8",
+    install_requires=[
+        "playwright==1.32.1",
+        "pydub==0.25.1",
+        "SpeechRecognition==3.10.0",
+    ],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Testing",
+        "Topic :: Internet :: WWW/HTTP :: Browsers",
+        "Framework :: AsyncIO",
+    ],
+)
```

### Comparing `playwright-recaptcha-0.1.3/tests/test_async_recaptchav2.py` & `playwright-recaptcha-0.2.0/tests/test_async_recaptchav2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,72 @@
-import pytest
-from playwright.async_api import async_playwright
-
-from playwright_recaptcha import (
-    RecaptchaNotFoundError,
-    RecaptchaRateLimitError,
-    recaptchav2,
-)
-
-
-@pytest.mark.asyncio
-@pytest.mark.xfail(raises=RecaptchaRateLimitError)
-async def test_solver() -> None:
-    """Test the solver with a normal browser."""
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
-
-        async with recaptchav2.AsyncSolver(page) as solver:
-            await solver.solve_recaptcha()
-
-
-@pytest.mark.asyncio
-@pytest.mark.xfail(raises=RecaptchaRateLimitError)
-async def test_solver_with_slow_browser() -> None:
-    """Test the solver with a slow browser."""
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch(slow_mo=1000)
-        page = await browser.new_page()
-
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
-
-        async with recaptchav2.AsyncSolver(page) as solver:
-            await solver.solve_recaptcha()
-
-
-@pytest.mark.asyncio
-async def test_recaptcha_not_found() -> None:
-    """Test the solver with a page that does not have a reCAPTCHA."""
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-        await page.goto("https://www.google.com/")
-
-        with pytest.raises(RecaptchaNotFoundError):
-            async with recaptchav2.AsyncSolver(page) as solver:
-                await solver.solve_recaptcha()
+import pytest
+from playwright.async_api import async_playwright
+
+from playwright_recaptcha import (
+    RecaptchaNotFoundError,
+    RecaptchaRateLimitError,
+    recaptchav2,
+)
+
+
+@pytest.mark.asyncio
+@pytest.mark.xfail(raises=RecaptchaRateLimitError)
+async def test_solver_with_normal_recaptcha() -> None:
+    """Test the solver with a normal reCAPTCHA."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+
+        await page.goto(
+            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+        )
+
+        async with recaptchav2.AsyncSolver(page) as solver:
+            await solver.solve_recaptcha()
+
+
+@pytest.mark.asyncio
+@pytest.mark.xfail(raises=(RecaptchaNotFoundError, RecaptchaRateLimitError))
+async def test_solver_with_hidden_recaptcha() -> None:
+    """Test the solver with a hidden reCAPTCHA."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+
+        await page.goto(
+            "https://www.google.com/recaptcha/api2/demo?invisible=true",
+            wait_until="networkidle",
+        )
+
+        await page.get_by_role("button").click()
+
+        async with recaptchav2.AsyncSolver(page) as solver:
+            await solver.solve_recaptcha()
+
+
+@pytest.mark.asyncio
+@pytest.mark.xfail(raises=RecaptchaRateLimitError)
+async def test_solver_with_slow_browser() -> None:
+    """Test the solver with a slow browser."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch(slow_mo=1000)
+        page = await browser.new_page()
+
+        await page.goto(
+            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+        )
+
+        async with recaptchav2.AsyncSolver(page) as solver:
+            await solver.solve_recaptcha()
+
+
+@pytest.mark.asyncio
+async def test_recaptcha_not_found_error() -> None:
+    """Test the solver with a page that does not have a reCAPTCHA."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+        await page.goto("https://www.google.com/")
+
+        with pytest.raises(RecaptchaNotFoundError):
+            async with recaptchav2.AsyncSolver(page) as solver:
+                await solver.solve_recaptcha()
```

### Comparing `playwright-recaptcha-0.1.3/tests/test_async_recaptchav3.py` & `playwright-recaptcha-0.2.0/tests/test_async_recaptchav3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import pytest
-from playwright.async_api import async_playwright
-
-from playwright_recaptcha import (
-    RecaptchaTimeoutError,
-    recaptchav3,
-)
-
-
-@pytest.mark.asyncio
-async def test_solver() -> None:
-    """Test the solver with a normal browser."""
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-        await page.goto("https://antcpt.com/score_detector/")
-
-        async with recaptchav3.AsyncSolver(page) as solver:
-            await solver.solve_recaptcha()
-
-
-@pytest.mark.asyncio
-async def test_solver_with_slow_browser() -> None:
-    """Test the solver with a slow browser."""
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch(slow_mo=1000)
-        page = await browser.new_page()
-        await page.goto("https://antcpt.com/score_detector/")
-
-        async with recaptchav3.AsyncSolver(page) as solver:
-            await solver.solve_recaptcha()
-
-
-@pytest.mark.asyncio
-async def test_recaptcha_not_found() -> None:
-    """Test the solver with a page that does not have a reCAPTCHA."""
-    async with async_playwright() as playwright:
-        browser = await playwright.firefox.launch()
-        page = await browser.new_page()
-        await page.goto("https://www.google.com/")
-
-        with pytest.raises(RecaptchaTimeoutError):
-            async with recaptchav3.AsyncSolver(page, timeout=10) as solver:
-                await solver.solve_recaptcha()
+import pytest
+from playwright.async_api import async_playwright
+
+from playwright_recaptcha import (
+    RecaptchaTimeoutError,
+    recaptchav3,
+)
+
+
+@pytest.mark.asyncio
+async def test_solver_with_normal_browser() -> None:
+    """Test the solver with a normal browser."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+        await page.goto("https://antcpt.com/score_detector/")
+
+        async with recaptchav3.AsyncSolver(page) as solver:
+            await solver.solve_recaptcha()
+
+
+@pytest.mark.asyncio
+async def test_solver_with_slow_browser() -> None:
+    """Test the solver with a slow browser."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch(slow_mo=1000)
+        page = await browser.new_page()
+        await page.goto("https://antcpt.com/score_detector/")
+
+        async with recaptchav3.AsyncSolver(page) as solver:
+            await solver.solve_recaptcha()
+
+
+@pytest.mark.asyncio
+async def test_recaptcha_not_found_error() -> None:
+    """Test the solver with a page that does not have a reCAPTCHA."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+        await page.goto("https://www.google.com/")
+
+        with pytest.raises(RecaptchaTimeoutError):
+            async with recaptchav3.AsyncSolver(page, timeout=10) as solver:
+                await solver.solve_recaptcha()
```

### Comparing `playwright-recaptcha-0.1.3/tests/test_sync_recaptchav2.py` & `playwright-recaptcha-0.2.0/tests/test_sync_recaptchav2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,69 @@
-import pytest
-from playwright.sync_api import sync_playwright
-
-from playwright_recaptcha import (
-    RecaptchaNotFoundError,
-    RecaptchaRateLimitError,
-    recaptchav2,
-)
-
-
-@pytest.mark.xfail(raises=RecaptchaRateLimitError)
-def test_solver() -> None:
-    """Test the solver with a normal browser."""
-    with sync_playwright() as playwright:
-        browser = playwright.firefox.launch()
-        page = browser.new_page()
-
-        page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
-
-        with recaptchav2.SyncSolver(page) as solver:
-            solver.solve_recaptcha()
-
-
-@pytest.mark.xfail(raises=RecaptchaRateLimitError)
-def test_solver_with_slow_browser() -> None:
-    """Test the solver with a slow browser."""
-    with sync_playwright() as playwright:
-        browser = playwright.firefox.launch(slow_mo=1000)
-        page = browser.new_page()
-
-        page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
-
-        with recaptchav2.SyncSolver(page) as solver:
-            solver.solve_recaptcha()
-
-
-def test_recaptcha_not_found() -> None:
-    """Test the solver with a page that does not have a reCAPTCHA."""
-    with sync_playwright() as playwright:
-        browser = playwright.firefox.launch()
-        page = browser.new_page()
-        page.goto("https://www.google.com/")
-
-        with pytest.raises(RecaptchaNotFoundError), recaptchav2.SyncSolver(
-            page
-        ) as solver:
-            solver.solve_recaptcha()
+import pytest
+from playwright.sync_api import sync_playwright
+
+from playwright_recaptcha import (
+    RecaptchaNotFoundError,
+    RecaptchaRateLimitError,
+    recaptchav2,
+)
+
+
+@pytest.mark.xfail(raises=RecaptchaRateLimitError)
+def test_solver_with_normal_recaptcha() -> None:
+    """Test the solver with a normal reCAPTCHA."""
+    with sync_playwright() as playwright:
+        browser = playwright.firefox.launch()
+        page = browser.new_page()
+
+        page.goto(
+            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+        )
+
+        with recaptchav2.SyncSolver(page) as solver:
+            solver.solve_recaptcha()
+
+
+@pytest.mark.xfail(raises=(RecaptchaNotFoundError, RecaptchaRateLimitError))
+def test_solver_with_hidden_recaptcha() -> None:
+    """Test the solver with a hidden reCAPTCHA."""
+    with sync_playwright() as playwright:
+        browser = playwright.firefox.launch()
+        page = browser.new_page()
+
+        page.goto(
+            "https://www.google.com/recaptcha/api2/demo?invisible=true",
+            wait_until="networkidle",
+        )
+
+        page.get_by_role("button").click()
+
+        with recaptchav2.SyncSolver(page) as solver:
+            solver.solve_recaptcha()
+
+
+@pytest.mark.xfail(raises=RecaptchaRateLimitError)
+def test_solver_with_slow_browser() -> None:
+    """Test the solver with a slow browser."""
+    with sync_playwright() as playwright:
+        browser = playwright.firefox.launch(slow_mo=1000)
+        page = browser.new_page()
+
+        page.goto(
+            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
+        )
+
+        with recaptchav2.SyncSolver(page) as solver:
+            solver.solve_recaptcha()
+
+
+def test_recaptcha_not_found_error() -> None:
+    """Test the solver with a page that does not have a reCAPTCHA."""
+    with sync_playwright() as playwright:
+        browser = playwright.firefox.launch()
+        page = browser.new_page()
+        page.goto("https://www.google.com/")
+
+        with pytest.raises(RecaptchaNotFoundError), recaptchav2.SyncSolver(
+            page
+        ) as solver:
+            solver.solve_recaptcha()
```

