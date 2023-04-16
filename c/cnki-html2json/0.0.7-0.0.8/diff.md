# Comparing `tmp/cnki_html2json-0.0.7.tar.gz` & `tmp/cnki_html2json-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.0.7.tar", last modified: Sun Apr  9 14:24:59 2023, max compression
+gzip compressed data, was "cnki_html2json-0.0.8.tar", last modified: Sun Apr 16 17:02:06 2023, max compression
```

## Comparing `cnki_html2json-0.0.7.tar` & `cnki_html2json-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 14:24:59.000000 cnki_html2json-0.0.7/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:59.470739 cnki_html2json-0.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/test/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 14:24:44.000000 cnki_html2json-0.0.7/test/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.493581 cnki_html2json-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-16 17:02:06.493581 cnki_html2json-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.489581 cnki_html2json-0.0.8/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.489581 cnki_html2json-0.0.8/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 17:02:06.000000 cnki_html2json-0.0.8/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 17:02:06.493581 cnki_html2json-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:02:06.489581 cnki_html2json-0.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/test/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-16 17:01:55.000000 cnki_html2json-0.0.8/test/test_metadata.py
```

### Comparing `cnki_html2json-0.0.7/PKG-INFO` & `cnki_html2json-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
@@ -55,18 +55,18 @@
 ```
 
 ## 使用方法
 
 1、调用 `html2json` 函数
 
 ```python
-from cnki_html2json.core import html2json
+from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
-    html = f.read()
-print(html2dict(html, mode='structure'))
+	html = f.read()
+print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
@@ -93,26 +93,26 @@
 
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
 | s | `start_paper_index` | 论文提取的起始索引，默认为1 |
 | e | `end_paper_index` | 论文提取的终止索引，默认为None，爬取到最后 |
 | m | `mode` | 模式，可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
+| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
 | save | `save_path` | 下载文件的保存路径，默认为当前目录的data文件夹 |
 | wait | `wait_time` | 为检索预留的等待时间，默认120秒 |
-| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
 
 注：爬虫将自动保存日志到 `save_path` 的log文件夹中，如果不想保存日志，请传入参数 `--debug`
 > 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫
-from cnki_html2json.core import start_crawl:
-start_crawl() # 默认参数
+from cnki_html2json.crawl import start_crawl:
+	start_crawl() # 默认参数
 ```
 
 ## json文件字段说明
 
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
```

### Comparing `cnki_html2json-0.0.7/README.md` & `cnki_html2json-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 ```
 
 ## 使用方法
 
 1、调用 `html2json` 函数
 
 ```python
-from cnki_html2json.core import html2json
+from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
-    html = f.read()
-print(html2dict(html, mode='structure'))
+	html = f.read()
+print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
@@ -71,26 +71,26 @@
 
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
 | s | `start_paper_index` | 论文提取的起始索引，默认为1 |
 | e | `end_paper_index` | 论文提取的终止索引，默认为None，爬取到最后 |
 | m | `mode` | 模式，可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
+| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
 | save | `save_path` | 下载文件的保存路径，默认为当前目录的data文件夹 |
 | wait | `wait_time` | 为检索预留的等待时间，默认120秒 |
-| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
 
 注：爬虫将自动保存日志到 `save_path` 的log文件夹中，如果不想保存日志，请传入参数 `--debug`
 > 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫
-from cnki_html2json.core import start_crawl:
-start_crawl() # 默认参数
+from cnki_html2json.crawl import start_crawl:
+	start_crawl() # 默认参数
 ```
 
 ## json文件字段说明
 
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
```

### Comparing `cnki_html2json-0.0.7/cnki_html2json/_html2json.py` & `cnki_html2json-0.0.8/cnki_html2json/html2json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
-# from lxml import etree
 from lxml import html
 import re
+import json
 
 def extract_nodes(long_nodes_list:list,short_nodes_list:list):
 	"""提取两个节点列表的差集"""
 	if short_nodes_list:
 		result = []
 		for node in long_nodes_list:
 			if node not in short_nodes_list:
@@ -193,15 +193,15 @@
 			total_text = concat_nodes_value(total_nodes_list,'text')
 			
 			if self.prefix:
 				return self.text['0']['text']+' '+total_text # type:ignore
 			else:
 				return total_text
 
-	def extract(self,task:str)->None:
+	def __extract(self,task:str)->None:
 		
 		if self.error:
 			self.text = None
 			return None
 		
 		offset = 1
 		if not self.annotation and "注释" in self.level_1_chapter:
@@ -260,21 +260,21 @@
 				self.text[current_level_1_chapter][task] = concat_nodes_value(current_node_,task) # type: ignore
 		
 			idx += 1
 
 	def extract_citation_index(self):
 		"""提取章节引用的文献索引"""
 
-		self.extract(task='citation')
+		self.__extract(task='citation')
 		return self.text
 	
 	def extract_text(self):
 		"""提取正文"""
 		
-		self.extract(task='text')
+		self.__extract(task='text')
 		return self.text
 
 	def extract_citation(self):
 		"""提取参考文献"""
 		citation = [doc.strip() for doc in self.html_general.xpath('//div[@id="a_bibliography"]/p/a/text()') if doc.strip()!='']
 		citation_with_index = [f'[{idx}] '+re.sub(r'^[\.]+','',doc).strip() for idx,doc in enumerate(citation,1)]
 		return citation_with_index
@@ -293,13 +293,28 @@
 		
 		elif self.mode == 'plain':
 			result = {'body_text':self.extract_plain_text()}
 		
 		# result |= {'参考文献':citing_docs}
 		return {**result,**{'参考文献':citing_docs}}
 	
-if __name__ == '__main__':
-	with open('test/fulltext.html','r',encoding='utf-8') as f:
-		content = f.read()
-	import json
-	with open('examples/raw_text.json','w',encoding='utf-8') as f:
-		json.dump(ExtractContent(content,'raw').extract_all(),f,ensure_ascii=False,indent=4)
+# 设置公开的接口
+def export_json(text,json_path):
+    """导出json文件"""
+    with open(json_path,'w',encoding='utf-8') as f:
+        json.dump(text,f,ensure_ascii=False,indent=4)
+
+def extract(paper_html:str,mode:str='structure',export=False,export_path=None):
+    """将论文的html字符串转换为字典
+    paper_html: 论文的html字符串
+    mode: 模式，structure|plain|raw，默认为structure
+    export: 是否导出json文件，默认为False
+    export_path: 导出json文件的路径，默认为None，如果导出json文件，该参数必须指定
+    """
+    result = ExtractContent(paper_html,mode).extract_all()
+    if not export:
+        return result
+    else:
+        if export_path is None:
+            raise ValueError('请设置导出参数')
+        else:
+            export_json(result,export_path)
```

### Comparing `cnki_html2json-0.0.7/cnki_html2json/cli.py` & `cnki_html2json-0.0.8/cnki_html2json/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from cnki_html2json.core import start_crawl
+from cnki_html2json.crawl import start_crawl
 
 def main():
     parser = argparse.ArgumentParser(description='CNKI crawler. Convert the html format of papers to json format.')
     parser.add_argument('-s','--start_paper_index',type=int,default=1,help='开始下载索引, 默认为1')
     parser.add_argument('-e','--end_paper_index',type=int,default=None,help='结束下载索引, 默认为None, 即下载到最后')
     parser.add_argument('-m','--mode',type=str,default='structure',help='模式: structure|plain|raw, 默认为structure')
     parser.add_argument('-b','--browser_type',type=str,default='Chrome',help='浏览器类型: Chrome(default)|Firefox|Edge')
```

### Comparing `cnki_html2json-0.0.7/cnki_html2json/crawl.py` & `cnki_html2json-0.0.8/cnki_html2json/crawl.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 import random
 import sys
 import math
 from loguru import logger
 from datetime import datetime
 
-from cnki_html2json import _html2json
+from cnki_html2json import html2json
 from cnki_html2json import parse_metadata
 from cnki_html2json import recognize_slider_coordinate
 
 
 def obtain_page_papers_url(driver) -> list:
     url_list = [i.get_attribute('href') for i in driver.find_elements(By.XPATH,'//*[@id="gridTable"]/table/tbody/tr/td[2]/a')]
     return url_list
@@ -66,15 +66,15 @@
         # 调用判断验证码函数
         recogize_count = process_slider(driver)
         
         if recogize_count > 0:
             logger.info(f'验证码识别{recogize_count}次后通过')
 
         paper_raw_html = driver.page_source
-        paper_dict = _html2json.ExtractContent(paper_raw_html,mode).extract_all()
+        paper_dict = html2json.ExtractContent(paper_raw_html,mode).extract_all()
         driver.close()
         if not paper_dict:
             logger.error('无法解析html页面')
         return concat_content(metadata,paper_dict)
       
     finally:
         driver.switch_to.window(handles[0]) 
@@ -106,20 +106,22 @@
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{visible_page_index[-1]}"]').click()
             time.sleep(3)
             current_page = visible_page_index[-1]
 
         
 def start_crawl(start_paper_index=1,end_paper_index=None,mode='structure',save_path='data',log=True,wait_time=120,browser_type='Chrome'):
-    """
-    start_paper_index:开始下载论文的索引
-    end_paper_index:结束下载论文的索引
-    mode:解析html页面的模式, 可选值为structure、plain和raw
-    save_path:文件保存路径
-    log:是否记录日志
+    """爬取cnki网站的论文
+    start_paper_index: 开始爬取的论文索引，默认为1
+    end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后
+    mode: 模式，structure|plain|raw，默认为structure
+    save_path: 下载文件的保存路径，默认为当前目录的data文件夹
+    log: 是否保存日志，默认为True
+    wait_time: 为检索预留的等待时间，单位为秒
+    browser_type: Chrome(默认)|Firefox|Edge|Safari
     """
     if log:
         if not os.path.exists(f'{save_path}/log'):
             os.mkdir(f'{save_path}/log')
             logger.info(f'已在{save_path}文件夹下创建log文件夹')
 
         current_time = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
```

### Comparing `cnki_html2json-0.0.7/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.0.8/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.7/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.0.8/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.0.7/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.0.8/cnki_html2json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Programming Language :: Python :: 3
@@ -55,18 +55,18 @@
 ```
 
 ## 使用方法
 
 1、调用 `html2json` 函数
 
 ```python
-from cnki_html2json.core import html2json
+from cnki_html2json import html2json
 with open('paper.html', 'r', encoding='utf-8') as f:
-    html = f.read()
-print(html2dict(html, mode='structure'))
+	html = f.read()
+print(html2json.extract(html, mode='structure'))
 ```
 `html2json` 参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
 | `paper_html` | 一篇期刊论文的html字符串 |
 | `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
@@ -93,26 +93,26 @@
 
 参数说明：
 | 简写参数 | 参数 | 说明 |
 | --- | --- | --- |
 | s | `start_paper_index` | 论文提取的起始索引，默认为1 |
 | e | `end_paper_index` | 论文提取的终止索引，默认为None，爬取到最后 |
 | m | `mode` | 模式，可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
+| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
 | save | `save_path` | 下载文件的保存路径，默认为当前目录的data文件夹 |
 | wait | `wait_time` | 为检索预留的等待时间，默认120秒 |
-| b | `browser` | 浏览器类型，Chrome(默认),可选 Edge, Firefox, 不支持Safari|
 
 注：爬虫将自动保存日志到 `save_path` 的log文件夹中，如果不想保存日志，请传入参数 `--debug`
 > 提取结果可以参考examples文件夹中给出的样例。如果未指定保存路径，将下载结果默认保存在当前目录下的data文件夹下  
 > 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫
-from cnki_html2json.core import start_crawl:
-start_crawl() # 默认参数
+from cnki_html2json.crawl import start_crawl:
+	start_crawl() # 默认参数
 ```
 
 ## json文件字段说明
 
 | 一级字段 | 二级字段 |三级字段| 说明 |
 | --- | --- | --- | --- |
 | metadata | title |  |论文标题|
```

### Comparing `cnki_html2json-0.0.7/setup.py` & `cnki_html2json-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.0.7",
+    version="0.0.8",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=find_packages(),
```

### Comparing `cnki_html2json-0.0.7/test/test_html2json.py` & `cnki_html2json-0.0.8/test/test_html2json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from cnki_html2json import _html2json
+from cnki_html2json import html2json
 
 def test_html2json():
     with open('test/fulltext.html','r') as f:
         content = f.read()
 
-    text_structure = _html2json.ExtractContent(content,'structure').extract_all()
+    text_structure = html2json.ExtractContent(content,'structure').extract_all()
     assert text_structure['body_text']['1 引言']['text'][:3] == "近年来"
 
-    text_plain = _html2json.ExtractContent(content,'plain').extract_all()
+    text_plain = html2json.ExtractContent(content,'plain').extract_all()
     assert text_plain['body_text'][:3] == "近年来"
 
-    text_raw = _html2json.ExtractContent(content,'raw').extract_all()
+    text_raw = html2json.ExtractContent(content,'raw').extract_all()
     assert '[1]' in text_raw['body_text']['1 引言']['text']
```

