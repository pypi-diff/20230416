# Comparing `tmp/katalytic-data-0.1.1.tar.gz` & `tmp/katalytic-data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.1.1.tar", last modified: Sun Apr 16 11:10:06 2023, max compression
+gzip compressed data, was "katalytic-data-0.2.0.tar", last modified: Sun Apr 16 12:22:55 2023, max compression
```

## Comparing `katalytic-data-0.1.1.tar` & `katalytic-data-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       87 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.gitignore
--rw-r--r--   0        0        0      841 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      542 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/.travis.yml
--rw-r--r--   0        0        0     1235 2023-04-16 11:10:02.179073 katalytic-data-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/README.md
--rw-r--r--   0        0        0     1516 2023-04-16 11:10:01.738853 katalytic-data-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/pytest.sh
--rw-r--r--   0        0        0     3107 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/scripts/venv.sh
--rw-r--r--   0        0        0      381 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/src/katalytic/checks.py
--rw-r--r--   0        0        0     2455 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/src/katalytic/data.py
--rw-r--r--   0        0        0      772 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/tests/test_checks.py
--rw-r--r--   0        0        0     5465 2023-04-16 11:09:24.460225 katalytic-data-0.1.1/tests/test_data.py
--rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 katalytic-data-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-13 15:48:09.439894 katalytic-data-0.2.0/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-data-0.2.0/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-05 11:25:28.742970 katalytic-data-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      542 2023-04-15 03:06:48.732796 katalytic-data-0.2.0/.travis.yml
+-rw-r--r--   0        0        0      884 2023-04-16 12:22:50.960034 katalytic-data-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-10 04:00:05.979612 katalytic-data-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2083 2023-04-15 15:52:39.144384 katalytic-data-0.2.0/README.md
+-rw-r--r--   0        0        0     1516 2023-04-16 12:22:50.560034 katalytic-data-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-13 11:10:42.206595 katalytic-data-0.2.0/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-13 05:19:55.379205 katalytic-data-0.2.0/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-10 04:05:02.825570 katalytic-data-0.2.0/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-10 04:00:05.995612 katalytic-data-0.2.0/scripts/pytest.sh
+-rw-r--r--   0        0        0     3267 2023-04-16 12:22:39.396035 katalytic-data-0.2.0/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-14 17:30:33.363765 katalytic-data-0.2.0/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-13 16:48:26.840531 katalytic-data-0.2.0/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-13 16:48:17.692461 katalytic-data-0.2.0/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-13 05:20:07.215328 katalytic-data-0.2.0/scripts/venv.sh
+-rw-r--r--   0        0        0      381 2023-04-16 05:11:03.853269 katalytic-data-0.2.0/src/katalytic/checks.py
+-rw-r--r--   0        0        0     2455 2023-04-16 05:01:47.932490 katalytic-data-0.2.0/src/katalytic/data.py
+-rw-r--r--   0        0        0      772 2023-04-16 05:10:05.493474 katalytic-data-0.2.0/tests/test_checks.py
+-rw-r--r--   0        0        0     5465 2023-04-16 05:05:41.482731 katalytic-data-0.2.0/tests/test_data.py
+-rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 katalytic-data-0.2.0/PKG-INFO
```

### Comparing `katalytic-data-0.1.1/.gitignore` & `katalytic-data-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/.gitlab-ci.yml` & `katalytic-data-0.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/.travis.yml` & `katalytic-data-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/CHANGELOG.md` & `katalytic-data-0.2.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-## 0.1.1 (2023-04-16)
-### Fix
-* Test the new token ([`7b08c42`](https://github.com/katalytic/katalytic-data/commit/7b08c428164a5c37c205b10687ce274622579a70))
-* Test the new token ([`4680b23`](https://github.com/katalytic/katalytic-data/commit/4680b2379099e206fef1ee4aef176547ef0c9f64))
-* Test the new token ([`9b71e3e`](https://github.com/katalytic/katalytic-data/commit/9b71e3e81fe35735673620732b1f54fc86f7e3d4))
+## 0.2.0 (2023-04-16)
+
 
 
+## 0.1.1 (2023-04-16)
+## Fix
+* nothing
+
 ## 0.1.0 (2023-04-16)
 ### Feature
 * Add is_collection() ([`bf29261`](https://github.com/katalytic/katalytic-data/commit/bf2926172f56d000d1f09318ab212c7b9747a8b0))
 * Add is_primitive() ([`ed950cc`](https://github.com/katalytic/katalytic-data/commit/ed950ccdd8e4cd4d4439cb0ab9c763d55135461d))
 * Add sort_dict_by_values() ([`6b3c985`](https://github.com/katalytic/katalytic-data/commit/6b3c9856c69e088467087345743a38e6294def7a))
 * Add sort_dict_by_keys() ([`5c05e48`](https://github.com/katalytic/katalytic-data/commit/5c05e48c4cc8afaf6a861103784690ebc153dcc8))
 * Add map_dict_values() ([`ba289c5`](https://github.com/katalytic/katalytic-data/commit/ba289c5f5cb21ff66d89bb833f30e2be678e15da))
```

### Comparing `katalytic-data-0.1.1/LICENSE.txt` & `katalytic-data-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/README.md` & `katalytic-data-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/pyproject.toml` & `katalytic-data-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.1.1"
+version = "0.2.0"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.1.1/scripts/conda.sh` & `katalytic-data-0.2.0/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/scripts/find_requirements.py` & `katalytic-data-0.2.0/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/scripts/release.sh` & `katalytic-data-0.2.0/scripts/release.sh`

 * *Files 12% similar despite different names*

```diff
@@ -91,50 +91,54 @@
 main(){
 	current_version=$(grep -P 'version = (.*)' pyproject.toml | grep -Po '[.0-9]+')
 	pkg=$(grep -P 'name = (.*)' pyproject.toml | head -n 1 | grep -Po 'katalytic[-.a-z]*' | sed 's/-/./' )
 	echo "Package: '$pkg'"
 	echo "Current: '$current_version'"
 	echo ""
 
-	rm -rf **/dist
-	rm -rf **/build
-	create_pypirc
-	create_env
-
-	# git config and pull
-	export GIT_MERGE_AUTOEDIT=no
-	git config credential.helper "!f() { printf '%s\n' 'username=vali19th' 'password=$GITLAB_TOKEN'; };f"
-	git config pull.rebase false
-	git pull --no-edit
+	# rm -rf **/dist
+	# rm -rf **/build
+	# create_pypirc
+	# create_env
+
+	# # git config and pull
+	# export GIT_MERGE_AUTOEDIT=no
+	# git config credential.helper "!f() { printf '%s\n' 'username=vali19th' 'password=$GITLAB_TOKEN'; };f"
+	# git config pull.rebase false
+	# git pull --no-edit
 
 	# bump version and update changelog
 	new_version="$(semantic-release print-version)"
 	if [[ "$new_version" != "" ]]; then
 		semantic-release version
 		update_changelog "$new_version"
 		command cat CHANGELOG.md
 	else
 		echo "No version bump. Exiting ..."
+		return
 		sleep 2
-		exit 0
+		# exit 0
 	fi
+	# return
 
 	# without this, flit won't build the sdist
 	git update-index --assume-unchanged pyproject.toml
 	git update-index --assume-unchanged CHANGELOG.md
+	git update-index --assume-unchanged scripts/release.sh
 
 	flit build --format sdist --setup-py
 	flit build --format wheel --setup-py
 	check_build "$pkg"
 
 	# release
 	flit publish --repository pypi
 
 	# push
 	git update-index --no-assume-unchanged pyproject.toml
 	git update-index --no-assume-unchanged CHANGELOG.md
-	git add CHANGELOG.md && git commit -m "doc: update CHANGELOG.md"
-	git push --tags
-	git push origin HEAD:main
+	git update-index --no-assume-unchanged scripts/release.sh
+	# git add CHANGELOG.md && git commit -m "doc: update CHANGELOG.md"
+	# git push --tags
+	# git push origin HEAD:main
 }
 
 main
```

### Comparing `katalytic-data-0.1.1/scripts/venv.sh` & `katalytic-data-0.2.0/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/src/katalytic/data.py` & `katalytic-data-0.2.0/src/katalytic/data.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/tests/test_checks.py` & `katalytic-data-0.2.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/tests/test_data.py` & `katalytic-data-0.2.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.1.1/PKG-INFO` & `katalytic-data-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.1.1
+Version: 0.2.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

