# Comparing `tmp/port_pulumi-0.9.0.tar.gz` & `tmp/port_pulumi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-0.9.0.tar", last modified: Sun Apr  2 11:03:25 2023, max compression
+gzip compressed data, was "port_pulumi-0.9.1.tar", last modified: Sun Apr 16 11:13:59 2023, max compression
```

## Comparing `port_pulumi-0.9.0.tar` & `port_pulumi-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:03:25.171950 port_pulumi-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-02 11:03:25.171950 port_pulumi-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:03:25.171950 port_pulumi-0.9.0/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24772 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    31426 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:03:25.171950 port_pulumi-0.9.0/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    22419 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/port_pulumi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:03:25.171950 port_pulumi-0.9.0/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-02 11:03:25.000000 port_pulumi-0.9.0/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-02 11:03:25.000000 port_pulumi-0.9.0/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 11:03:25.000000 port_pulumi-0.9.0/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 11:03:25.000000 port_pulumi-0.9.0/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-02 11:03:25.000000 port_pulumi-0.9.0/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-02 11:03:25.000000 port_pulumi-0.9.0/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 11:03:25.171950 port_pulumi-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-02 11:03:24.000000 port_pulumi-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22419 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:13:59.378078 port_pulumi-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-16 11:13:59.000000 port_pulumi-0.9.1/setup.py
```

### Comparing `port_pulumi-0.9.0/PKG-INFO` & `port_pulumi-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Port Resource Provider
 
 ![Port](./img/port.svg)
 
 The Port Resource Provider lets you manage [Port](https://www.getport.io) resources.
```

### Comparing `port_pulumi-0.9.0/README.md` & `port_pulumi-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/port_pulumi/__init__.py` & `port_pulumi-0.9.1/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/port_pulumi/_inputs.py` & `port_pulumi-0.9.1/port_pulumi/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,14 +477,15 @@
                  default: Optional[pulumi.Input[str]] = None,
                  default_items: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enum_colors: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  enums: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  format: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
+                 items: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  required: Optional[pulumi.Input[bool]] = None,
                  spec: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "identifier", identifier)
         pulumi.set(__self__, "title", title)
         pulumi.set(__self__, "type", type)
         if default is not None:
             pulumi.set(__self__, "default", default)
@@ -496,14 +497,16 @@
             pulumi.set(__self__, "enum_colors", enum_colors)
         if enums is not None:
             pulumi.set(__self__, "enums", enums)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
+        if items is not None:
+            pulumi.set(__self__, "items", items)
         if required is not None:
             pulumi.set(__self__, "required", required)
         if spec is not None:
             pulumi.set(__self__, "spec", spec)
 
     @property
     @pulumi.getter
@@ -593,14 +596,23 @@
 
     @icon.setter
     def icon(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "icon", value)
 
     @property
     @pulumi.getter
+    def items(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+        return pulumi.get(self, "items")
+
+    @items.setter
+    def items(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+        pulumi.set(self, "items", value)
+
+    @property
+    @pulumi.getter
     def required(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "required")
 
     @required.setter
     def required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "required", value)
```

### Comparing `port_pulumi-0.9.0/port_pulumi/_utilities.py` & `port_pulumi-0.9.1/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/port_pulumi/action.py` & `port_pulumi-0.9.1/port_pulumi/action.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/port_pulumi/blueprint.py` & `port_pulumi-0.9.1/port_pulumi/blueprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                  mirror_properties: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]]] = None,
                  relations: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]] = None):
         """
         The set of arguments for constructing a Blueprint resource.
         :param pulumi.Input[str] identifier: The identifier of the blueprint
         :param pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]] properties: The metadata of the entity
         :param pulumi.Input[str] title: The display name of the blueprint
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]] calculation_properties: A set of properties that are calculated upon Entitys regular properties.
+        :param pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
         :param pulumi.Input['BlueprintChangelogDestinationArgs'] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
         :param pulumi.Input[str] data_source: The data source for entities of this blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
         :param pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
                Blueprint.
         :param pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]] relations: The blueprints that are connected to this blueprint
@@ -97,15 +97,15 @@
     def title(self, value: pulumi.Input[str]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter(name="calculationProperties")
     def calculation_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]:
         """
-        A set of properties that are calculated upon Entitys regular properties.
+        A set of properties that are calculated upon entity's regular properties.
         """
         return pulumi.get(self, "calculation_properties")
 
     @calculation_properties.setter
     def calculation_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]):
         pulumi.set(self, "calculation_properties", value)
 
@@ -198,15 +198,15 @@
                  properties: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintPropertyArgs']]]] = None,
                  relations: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintRelationArgs']]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  updated_at: Optional[pulumi.Input[str]] = None,
                  updated_by: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Blueprint resources.
-        :param pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]] calculation_properties: A set of properties that are calculated upon Entitys regular properties.
+        :param pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
         :param pulumi.Input['BlueprintChangelogDestinationArgs'] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
         :param pulumi.Input[str] data_source: The data source for entities of this blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
         :param pulumi.Input[str] identifier: The identifier of the blueprint
         :param pulumi.Input[Sequence[pulumi.Input['BlueprintMirrorPropertyArgs']]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
                Blueprint.
@@ -246,15 +246,15 @@
         if updated_by is not None:
             pulumi.set(__self__, "updated_by", updated_by)
 
     @property
     @pulumi.getter(name="calculationProperties")
     def calculation_properties(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]:
         """
-        A set of properties that are calculated upon Entitys regular properties.
+        A set of properties that are calculated upon entity's regular properties.
         """
         return pulumi.get(self, "calculation_properties")
 
     @calculation_properties.setter
     def calculation_properties(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BlueprintCalculationPropertyArgs']]]]):
         pulumi.set(self, "calculation_properties", value)
 
@@ -420,15 +420,15 @@
                  relations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintRelationArgs']]]]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Blueprint resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]] calculation_properties: A set of properties that are calculated upon Entitys regular properties.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
         :param pulumi.Input[pulumi.InputType['BlueprintChangelogDestinationArgs']] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
         :param pulumi.Input[str] data_source: The data source for entities of this blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
         :param pulumi.Input[str] identifier: The identifier of the blueprint
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintMirrorPropertyArgs']]]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
                Blueprint.
@@ -528,15 +528,15 @@
         """
         Get an existing Blueprint resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]] calculation_properties: A set of properties that are calculated upon Entitys regular properties.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintCalculationPropertyArgs']]]] calculation_properties: A set of properties that are calculated upon entity's regular properties.
         :param pulumi.Input[pulumi.InputType['BlueprintChangelogDestinationArgs']] changelog_destination: Blueprints changelog destination, Supports WEBHOOK and KAFKA
         :param pulumi.Input[str] data_source: The data source for entities of this blueprint
         :param pulumi.Input[str] description: The description of the blueprint
         :param pulumi.Input[str] icon: The icon of the blueprint
         :param pulumi.Input[str] identifier: The identifier of the blueprint
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BlueprintMirrorPropertyArgs']]]] mirror_properties: When two Blueprints are connected via a Relation, a new set of properties becomes available to Entities in the source
                Blueprint.
@@ -564,15 +564,15 @@
         __props__.__dict__["updated_by"] = updated_by
         return Blueprint(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="calculationProperties")
     def calculation_properties(self) -> pulumi.Output[Optional[Sequence['outputs.BlueprintCalculationProperty']]]:
         """
-        A set of properties that are calculated upon Entitys regular properties.
+        A set of properties that are calculated upon entity's regular properties.
         """
         return pulumi.get(self, "calculation_properties")
 
     @property
     @pulumi.getter(name="changelogDestination")
     def changelog_destination(self) -> pulumi.Output[Optional['outputs.BlueprintChangelogDestination']]:
         """
```

### Comparing `port_pulumi-0.9.0/port_pulumi/config/vars.py` & `port_pulumi-0.9.1/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/port_pulumi/entity.py` & `port_pulumi-0.9.1/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/port_pulumi/outputs.py` & `port_pulumi-0.9.1/port_pulumi/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,15 @@
                  default: Optional[str] = None,
                  default_items: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
                  enum_colors: Optional[Mapping[str, str]] = None,
                  enums: Optional[Sequence[str]] = None,
                  format: Optional[str] = None,
                  icon: Optional[str] = None,
+                 items: Optional[Mapping[str, Any]] = None,
                  required: Optional[bool] = None,
                  spec: Optional[str] = None):
         pulumi.set(__self__, "identifier", identifier)
         pulumi.set(__self__, "title", title)
         pulumi.set(__self__, "type", type)
         if default is not None:
             pulumi.set(__self__, "default", default)
@@ -411,14 +412,16 @@
             pulumi.set(__self__, "enum_colors", enum_colors)
         if enums is not None:
             pulumi.set(__self__, "enums", enums)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
+        if items is not None:
+            pulumi.set(__self__, "items", items)
         if required is not None:
             pulumi.set(__self__, "required", required)
         if spec is not None:
             pulumi.set(__self__, "spec", spec)
 
     @property
     @pulumi.getter
@@ -468,14 +471,19 @@
     @property
     @pulumi.getter
     def icon(self) -> Optional[str]:
         return pulumi.get(self, "icon")
 
     @property
     @pulumi.getter
+    def items(self) -> Optional[Mapping[str, Any]]:
+        return pulumi.get(self, "items")
+
+    @property
+    @pulumi.getter
     def required(self) -> Optional[bool]:
         return pulumi.get(self, "required")
 
     @property
     @pulumi.getter
     def spec(self) -> Optional[str]:
         return pulumi.get(self, "spec")
```

### Comparing `port_pulumi-0.9.0/port_pulumi/provider.py` & `port_pulumi-0.9.1/port_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-0.9.1/port_pulumi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Port Resource Provider
 
 ![Port](./img/port.svg)
 
 The Port Resource Provider lets you manage [Port](https://www.getport.io) resources.
```

### Comparing `port_pulumi-0.9.0/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-0.9.1/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-0.9.0/setup.py` & `port_pulumi-0.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.0"
-PLUGIN_VERSION = "0.9.0"
+VERSION = "0.9.1"
+PLUGIN_VERSION = "0.9.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'port', PLUGIN_VERSION, '--server', 'github://api.github.com/port-labs/pulumi'])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "port Pulumi Package - Development Version"
 
 
 setup(name='port_pulumi',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing Port resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

