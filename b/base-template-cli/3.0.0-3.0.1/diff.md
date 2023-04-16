# Comparing `tmp/base_template_cli-3.0.0.tar.gz` & `tmp/base_template_cli-3.0.1.tar.gz`

## Comparing `base_template_cli-3.0.0.tar` & `base_template_cli-3.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.commitlintrc.yml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.czrc
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.editorconfig
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.gitignore_custom
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.lintstagedrc.yml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.markdownlint.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.markdownlintignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.node-version
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.prettierignore
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.python-version
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.releaserc.yml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.secretlintrc.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.tool-versions
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.vale.ini
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.yamllint.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/Makefile
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/Pipfile
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/Pipfile.lock
--rw-r--r--   0        0        0   479074 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/package-lock.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/package.json
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/ISSUE_TEMPLATE/general-issue-beta.yml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/ISSUE_TEMPLATE/general-issue.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/vale_styles/Vocab/Base/accept.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/vale_styles/Vocab/Base/reject.txt
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/workflows/dependabot.yml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/workflows/lint-pr-title.yml
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/workflows/reviewdog.yml
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.github/workflows/test.yml
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.husky/commit-msg
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.husky/pre-commit
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.vscode/extensions.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.vscode/settings.json
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/bin/build.sh
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/bin/publish.sh
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/docs/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/docs/SECURITY.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/docs/_config.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/src/base_template_cli/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/src/base_template_cli/applyer.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/src/base_template_cli/base_template_updater.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/src/base_template_cli/di_manager.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/src/base_template_cli/file_copy_util.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/src/base_template_cli/main.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/src/base_template_cli/version_getter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/tests/.keep
--rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/LICENSE
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/README.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/hatch.toml
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 base_template_cli-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.commitlintrc.yml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.czrc
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.editorconfig
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.gitignore_custom
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.lintstagedrc.yml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.markdownlint.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.markdownlintignore
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.node-version
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.prettierignore
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.python-version
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.releaserc.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.secretlintrc.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.tool-versions
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.vale.ini
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.yamllint.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/Makefile
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/Pipfile
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/Pipfile.lock
+-rw-r--r--   0        0        0   479092 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/package-lock.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/package.json
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/ISSUE_TEMPLATE/general-issue-beta.yml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/ISSUE_TEMPLATE/general-issue.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/vale_styles/Vocab/Base/accept.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/vale_styles/Vocab/Base/reject.txt
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/workflows/dependabot.yml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/workflows/lint-pr-title.yml
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/workflows/reviewdog.yml
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.husky/commit-msg
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.husky/pre-commit
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.vscode/settings.json
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/bin/build.sh
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/bin/publish.sh
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/docs/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/docs/SECURITY.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/docs/_config.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/src/base_template_cli/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/src/base_template_cli/applyer.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/src/base_template_cli/base_template_updater.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/src/base_template_cli/di_manager.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/src/base_template_cli/file_copy_util.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/src/base_template_cli/main.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/src/base_template_cli/version_getter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/tests/.keep
+-rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/LICENSE
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/README.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/hatch.toml
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 base_template_cli-3.0.1/PKG-INFO
```

### Comparing `base_template_cli-3.0.0/.releaserc.yml` & `base_template_cli-3.0.1/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/Makefile` & `base_template_cli-3.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/Pipfile.lock` & `base_template_cli-3.0.1/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'734dae06af031f75755132664c4040c30c3c837093d6b78ecaf034153d75a93c'}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "86921d46874b7a5a2a98fa0fd25be60b0f6ceb273f2961c0a8af773482b6b27a"
+            "sha256": "734dae06af031f75755132664c4040c30c3c837093d6b78ecaf034153d75a93c"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_full_version": "3.11.2",
             "python_version": "3.11"
         },
         "sources": [
```

### Comparing `base_template_cli-3.0.0/package-lock.json` & `base_template_cli-3.0.1/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999541161087624%*

 * *Differences: {"'packages'": "{'': {'version': '3.0.1', 'devDependencies': {'lint-staged': '^13.2.1', "*

 * *               "'npm-check-updates': '^16.10.7'}}, 'node_modules/lint-staged': {'version': "*

 * *               "'13.2.1', 'resolved': "*

 * *               "'https://registry.npmjs.org/lint-staged/-/lint-staged-13.2.1.tgz', 'integrity': "*

 * *               "'sha512-8gfzinVXoPfga5Dz/ZOn8I2GOhf81Wvs+KwbEXQn/oWZAvCVS2PivrXfVbFJc93zD16uC0neS47RXHIjXKYZQw=='}, "*

 * *               "'node_modules/npm-check-updates': {'version': '16.10.7',  […]*

```diff
@@ -10,29 +10,29 @@
                 "@secretlint/secretlint-rule-preset-recommend": "^6.2.3",
                 "@semantic-release/changelog": "^6.0.3",
                 "@semantic-release/exec": "^6.0.3",
                 "@semantic-release/git": "^10.0.1",
                 "commitizen": "^4.3.0",
                 "conventional-changelog-conventionalcommits": "^5.0.0",
                 "husky": "^8.0.3",
-                "lint-staged": "^13.2.0",
+                "lint-staged": "^13.2.1",
                 "markdownlint-cli": ">=0.33.0 <1.0.0",
-                "npm-check-updates": "^16.10.0",
+                "npm-check-updates": "^16.10.7",
                 "npm-run-all": "^4.1.5",
                 "prettier": "^2.8.7",
                 "secretlint": "^6.2.3",
                 "semantic-release": "^21.0.1"
             },
             "engines": {
                 "node": "^18.15.0",
                 "npm": "^9.6.3"
             },
             "license": "MIT",
             "name": "base-template-cli",
-            "version": "3.0.0"
+            "version": "3.0.1"
         },
         "node_modules/@azu/format-text": {
             "dev": true,
             "integrity": "sha512-Swi4N7Edy1Eqq82GxgEECXSSLyn6GOb5htRFPzBDdUkECGXtlf12ynO5oJSpWKPwCaUssOu7NfhDcCWpIC6Ywg==",
             "resolved": "https://registry.npmjs.org/@azu/format-text/-/format-text-1.0.2.tgz",
             "version": "1.0.2"
         },
@@ -5475,17 +5475,17 @@
             "dev": true,
             "engines": {
                 "node": "^14.13.1 || >=16.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/lint-staged"
             },
-            "integrity": "sha512-GbyK5iWinax5Dfw5obm2g2ccUiZXNGtAS4mCbJ0Lv4rq6iEtfBSjOYdcbOtAIFtM114t0vdpViDDetjVTSd8Vw==",
-            "resolved": "https://registry.npmjs.org/lint-staged/-/lint-staged-13.2.0.tgz",
-            "version": "13.2.0"
+            "integrity": "sha512-8gfzinVXoPfga5Dz/ZOn8I2GOhf81Wvs+KwbEXQn/oWZAvCVS2PivrXfVbFJc93zD16uC0neS47RXHIjXKYZQw==",
+            "resolved": "https://registry.npmjs.org/lint-staged/-/lint-staged-13.2.1.tgz",
+            "version": "13.2.1"
         },
         "node_modules/lint-staged/node_modules/chalk": {
             "dev": true,
             "engines": {
                 "node": "^12.17.0 || ^14.13 || >=16.0.0"
             },
             "funding": {
@@ -7085,42 +7085,42 @@
                 "fast-memoize": "^2.5.2",
                 "find-up": "5.0.0",
                 "fp-and-or": "^0.1.3",
                 "get-stdin": "^8.0.0",
                 "globby": "^11.0.4",
                 "hosted-git-info": "^5.1.0",
                 "ini": "^4.0.0",
+                "js-yaml": "^4.1.0",
                 "json-parse-helpfulerror": "^1.0.3",
                 "jsonlines": "^0.1.1",
                 "lodash": "^4.17.21",
-                "minimatch": "^7.4.3",
+                "minimatch": "^8.0.3",
                 "p-map": "^4.0.0",
                 "pacote": "15.1.1",
                 "parse-github-url": "^1.0.2",
                 "progress": "^2.0.3",
-                "prompts-ncu": "^2.5.1",
+                "prompts-ncu": "^3.0.0",
                 "rc-config-loader": "^4.1.2",
                 "remote-git-tags": "^3.0.0",
                 "rimraf": "^4.4.1",
                 "semver": "^7.3.8",
                 "semver-utils": "^1.1.4",
                 "source-map-support": "^0.5.21",
                 "spawn-please": "^2.0.1",
                 "strip-json-comments": "^5.0.0",
                 "untildify": "^4.0.0",
-                "update-notifier": "^6.0.2",
-                "yaml": "^2.2.1"
+                "update-notifier": "^6.0.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=14.14"
             },
-            "integrity": "sha512-xtTm38/94u9BhFbIuq1yxjKs+lmXQK+RnzxgfMVzRhz9vRXgcuC9ZsSw8hormmrmVtIZ8yG0At80d1R5vRf6rQ==",
-            "resolved": "https://registry.npmjs.org/npm-check-updates/-/npm-check-updates-16.10.0.tgz",
-            "version": "16.10.0"
+            "integrity": "sha512-hVJCULf8AoVob9FDvoC7hrkQGuWhWctE9k3sNmR+M6hxZJnlb+03Ph4G1w/pHmI5BGHoo+ZPJtVEXkJsA+JwPQ==",
+            "resolved": "https://registry.npmjs.org/npm-check-updates/-/npm-check-updates-16.10.7.tgz",
+            "version": "16.10.7"
         },
         "node_modules/npm-check-updates/node_modules/brace-expansion": {
             "dependencies": {
                 "balanced-match": "^1.0.0"
             },
             "dev": true,
             "integrity": "sha512-XnAIvQ8eM+kC6aULx6wuQiwVsnzsi9d3WxzV3FpWTGA19F621kwdbsAcFKXgKUHZWsy+mY6iL1sHTxWEFCytDA==",
@@ -7174,22 +7174,22 @@
         },
         "node_modules/npm-check-updates/node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^2.0.1"
             },
             "dev": true,
             "engines": {
-                "node": ">=10"
+                "node": ">=16 || 14 >=14.17"
             },
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
-            "integrity": "sha512-T+8B3kNrLP7jDb5eaC4rUIp6DKoeTSb6f9SwF2phcY2gxJUA0GEf1i29/FHxBMEfx0ppWlr434/D0P+6jb8bOQ==",
-            "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-7.4.4.tgz",
-            "version": "7.4.4"
+            "integrity": "sha512-W0Wvr9HyFXZRGIDgCicunpQ299OKXs9RgZfaukz4qAW/pJhcpUfupc9c+OObPOFueNy8VSrZgEmDtk6Kh4WzDA==",
+            "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-8.0.4.tgz",
+            "version": "8.0.4"
         },
         "node_modules/npm-check-updates/node_modules/strip-json-comments": {
             "dev": true,
             "engines": {
                 "node": ">=14.16"
             },
             "funding": {
@@ -10965,19 +10965,19 @@
         "node_modules/prompts-ncu": {
             "dependencies": {
                 "kleur": "^4.0.1",
                 "sisteransi": "^1.0.5"
             },
             "dev": true,
             "engines": {
-                "node": ">= 6"
+                "node": ">= 14"
             },
-            "integrity": "sha512-Hdd7GgV7b76Yh9FP9HL1D9xqtJCJdVPpiM2vDtuoc8W1KfweJe15gutFYmxkq83ViFaagFM8K0UcPCQ/tZq8bA==",
-            "resolved": "https://registry.npmjs.org/prompts-ncu/-/prompts-ncu-2.5.1.tgz",
-            "version": "2.5.1"
+            "integrity": "sha512-qyz9UxZ5MlPKWVhWrCmSZ1ahm2GVYdjLb8og2sg0IPth1KRuhcggHGuijz0e41dkx35p1t1q3GRISGH7QGALFA==",
+            "resolved": "https://registry.npmjs.org/prompts-ncu/-/prompts-ncu-3.0.0.tgz",
+            "version": "3.0.0"
         },
         "node_modules/proto-list": {
             "dev": true,
             "integrity": "sha512-vtK/94akxsTMhe0/cbfpR+syPuszcuwhqVjJq26CuNDgFGj682oRBXOP5MJpv2r7JtE8MsiepGIqvvOTBwn2vA==",
             "resolved": "https://registry.npmjs.org/proto-list/-/proto-list-1.2.4.tgz",
             "version": "1.2.4"
         },
@@ -13905,9 +13905,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "3.0.0"
+    "version": "3.0.1"
 }
```

### Comparing `base_template_cli-3.0.0/package.json` & `base_template_cli-3.0.1/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9592760180995475%*

 * *Differences: {"'devDependencies'": "{'lint-staged': '^13.2.1', 'npm-check-updates': '^16.10.7'}",*

 * * "'version'": "'3.0.1'"}*

```diff
@@ -14,17 +14,17 @@
         "@secretlint/secretlint-rule-preset-recommend": "^6.2.3",
         "@semantic-release/changelog": "^6.0.3",
         "@semantic-release/exec": "^6.0.3",
         "@semantic-release/git": "^10.0.1",
         "commitizen": "^4.3.0",
         "conventional-changelog-conventionalcommits": "^5.0.0",
         "husky": "^8.0.3",
-        "lint-staged": "^13.2.0",
+        "lint-staged": "^13.2.1",
         "markdownlint-cli": ">=0.33.0 <1.0.0",
-        "npm-check-updates": "^16.10.0",
+        "npm-check-updates": "^16.10.7",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.7",
         "secretlint": "^6.2.3",
         "semantic-release": "^21.0.1"
     },
     "engines": {
         "node": "^18.15.0",
@@ -52,9 +52,9 @@
         "lint": "run-s --continue-on-error lint:*",
         "lint:credentials": "[ \"$CI\" = 'true' ] || secretlint \"**/*\"",
         "lint:md": "markdownlint . \".?*/**/*.{md,markdown}\"",
         "lint:prettier": "prettier --check .",
         "prepare": "[ \"$CI\" = 'true' ] || husky install",
         "test": "echo \"Error: no test specified\" && exit 1"
     },
-    "version": "3.0.0"
+    "version": "3.0.1"
 }
```

### Comparing `base_template_cli-3.0.0/.github/ISSUE_TEMPLATE/general-issue-beta.yml` & `base_template_cli-3.0.1/.github/ISSUE_TEMPLATE/general-issue-beta.yml`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/.github/workflows/dependabot.yml` & `base_template_cli-3.0.1/.github/workflows/dependabot.yml`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/.github/workflows/release.yml` & `base_template_cli-3.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/.github/workflows/reviewdog.yml` & `base_template_cli-3.0.1/.github/workflows/reviewdog.yml`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/.github/workflows/test.yml` & `base_template_cli-3.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/docs/CHANGELOG.md` & `base_template_cli-3.0.1/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [3.0.1](https://github.com/haru52/base_template_cli/compare/v3.0.0...v3.0.1) (2023-04-16)
+
+
+### Bug Fixes
+
+* fix CLI to work correctly ([3c09951](https://github.com/haru52/base_template_cli/commit/3c099519b8f89412c7f307749a74238b18482621))
+
 ## [3.0.0](https://github.com/haru52/base_template_cli/compare/v2.2.0...v3.0.0) (2023-04-06)
 
 
 ### ⚠ BREAKING CHANGES
 
 * change to use subcommands
```

### Comparing `base_template_cli-3.0.0/docs/CODE_OF_CONDUCT.md` & `base_template_cli-3.0.1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/docs/CONTRIBUTING.md` & `base_template_cli-3.0.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/docs/SECURITY.md` & `base_template_cli-3.0.1/docs/SECURITY.md`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/src/base_template_cli/applyer.py` & `base_template_cli-3.0.1/src/base_template_cli/applyer.py`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/src/base_template_cli/base_template_updater.py` & `base_template_cli-3.0.1/src/base_template_cli/base_template_updater.py`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/src/base_template_cli/di_manager.py` & `base_template_cli-3.0.1/src/base_template_cli/di_manager.py`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/src/base_template_cli/file_copy_util.py` & `base_template_cli-3.0.1/src/base_template_cli/file_copy_util.py`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/src/base_template_cli/main.py` & `base_template_cli-3.0.1/src/base_template_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,9 +53,13 @@
         target_dirs,
         only_root,
         lang)
     applyer = di_manager.getInstance('Applyer')
     applyer.apply()
 
 
-if __name__ == '__main__':
+def main():
     cli()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `base_template_cli-3.0.0/.gitignore` & `base_template_cli-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/LICENSE` & `base_template_cli-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/README.md` & `base_template_cli-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/pyproject.toml` & `base_template_cli-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `base_template_cli-3.0.0/PKG-INFO` & `base_template_cli-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-template-cli
-Version: 3.0.0
+Version: 3.0.1
 Summary: CLI tool of Base Template Repository.
 Project-URL: Homepage, https://github.com/haru52/base_template_cli#readme
 Project-URL: Bug Tracker, https://github.com/haru52/base_template_cli/issues
 Project-URL: Repository, https://github.com/haru52/base_template_cli.git
 Author: haru
 License-Expression: MIT
 License-File: LICENSE
```

