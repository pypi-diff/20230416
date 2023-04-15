# Comparing `tmp/sigmatools-0.8-py3-none-any.whl.zip` & `tmp/sigmatools-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,54 +1,56 @@
-Zip file size: 77770 bytes, number of entries: 52
--rw-r--r--  2.0 unx        0 b- defN 18-Nov-07 07:06 sigma/__init__.py
--rw-r--r--  2.0 unx    10434 b- defN 19-Feb-28 07:59 sigma/configuration.py
--rw-r--r--  2.0 unx     4768 b- defN 18-Nov-07 07:06 sigma/filter.py
--rw-r--r--  2.0 unx     6686 b- defN 18-Nov-07 07:06 sigma/backends/arcsight.py
--rw-r--r--  2.0 unx    10501 b- defN 19-Feb-28 07:59 sigma/backends/base.py
--rw-r--r--  2.0 unx     1685 b- defN 18-Nov-07 07:06 sigma/backends/discovery.py
--rw-r--r--  2.0 unx    34250 b- defN 19-Feb-28 07:21 sigma/backends/elasticsearch.py
--rw-r--r--  2.0 unx     1164 b- defN 18-Nov-07 07:06 sigma/backends/exceptions.py
--rw-r--r--  2.0 unx     1388 b- defN 19-Feb-28 07:21 sigma/backends/graylog.py
--rw-r--r--  2.0 unx     2036 b- defN 19-Feb-28 07:21 sigma/backends/logpoint.py
--rw-r--r--  2.0 unx     2093 b- defN 19-Feb-28 07:21 sigma/backends/misc.py
--rw-r--r--  2.0 unx     2895 b- defN 18-Nov-07 07:06 sigma/backends/mixins.py
--rw-r--r--  2.0 unx     4439 b- defN 18-Dec-05 08:03 sigma/backends/netwitness.py
--rw-r--r--  2.0 unx     8381 b- defN 19-Feb-28 07:21 sigma/backends/powershell.py
--rw-r--r--  2.0 unx     8613 b- defN 19-Feb-19 13:46 sigma/backends/qradar.py
--rw-r--r--  2.0 unx     4138 b- defN 18-Nov-07 07:06 sigma/backends/qualys.py
--rw-r--r--  2.0 unx     7573 b- defN 19-Feb-28 07:21 sigma/backends/splunk.py
--rw-r--r--  2.0 unx    11392 b- defN 19-Feb-28 07:21 sigma/backends/sumologic.py
--rw-r--r--  2.0 unx     2806 b- defN 18-Nov-07 07:06 sigma/backends/tools.py
--rw-r--r--  2.0 unx    10122 b- defN 19-Feb-28 07:59 sigma/backends/wdatp.py
--rw-r--r--  2.0 unx      827 b- defN 19-Feb-28 07:59 sigma/config/exceptions.py
--rw-r--r--  2.0 unx     5629 b- defN 19-Feb-28 07:59 sigma/config/mapping.py
--rw-r--r--  2.0 unx     3284 b- defN 19-Feb-28 07:59 sigma/parser/base.py
--rw-r--r--  2.0 unx     3471 b- defN 18-Nov-07 07:06 sigma/parser/collection.py
--rw-r--r--  2.0 unx    26573 b- defN 19-Feb-28 07:59 sigma/parser/condition.py
--rw-r--r--  2.0 unx      817 b- defN 18-Nov-07 07:06 sigma/parser/exceptions.py
--rw-r--r--  2.0 unx     5485 b- defN 19-Feb-28 07:59 sigma/parser/rule.py
--rw-r--r--  2.0 unx     2227 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/arcsight.yml
--rw-r--r--  2.0 unx       31 b- defN 18-Nov-07 07:06 sigmatools-0.8.data/data/etc/sigma/elk-defaultindex-filebeat.yml
--rw-r--r--  2.0 unx       31 b- defN 18-Nov-07 07:06 sigmatools-0.8.data/data/etc/sigma/elk-defaultindex-logstash.yml
--rw-r--r--  2.0 unx       48 b- defN 18-Nov-07 07:06 sigmatools-0.8.data/data/etc/sigma/elk-defaultindex.yml
--rw-r--r--  2.0 unx      345 b- defN 18-Nov-07 07:06 sigmatools-0.8.data/data/etc/sigma/elk-linux.yml
--rw-r--r--  2.0 unx      841 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/elk-windows.yml
--rw-r--r--  2.0 unx     3646 b- defN 19-Feb-28 07:59 sigmatools-0.8.data/data/etc/sigma/elk-winlogbeat.yml
--rw-r--r--  2.0 unx     4601 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/helk.yml
--rw-r--r--  2.0 unx     3346 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/logpoint-windows-all.yml
--rw-r--r--  2.0 unx     1641 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/netwitness.yml
--rw-r--r--  2.0 unx     1715 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/powershell-windows-all.yml
--rw-r--r--  2.0 unx      659 b- defN 19-Feb-19 13:46 sigmatools-0.8.data/data/etc/sigma/qradar.yml
--rw-r--r--  2.0 unx      395 b- defN 18-Nov-07 07:06 sigmatools-0.8.data/data/etc/sigma/qualys.yml
--rw-r--r--  2.0 unx     1510 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/spark.yml
--rw-r--r--  2.0 unx     1820 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/splunk-windows-all.yml
--rw-r--r--  2.0 unx     1371 b- defN 19-Feb-28 07:21 sigmatools-0.8.data/data/etc/sigma/sumologic.yml
--rwxr-xr-x  2.0 unx     1313 b- defN 19-Feb-28 08:09 sigmatools-0.8.data/scripts/merge_sigma
--rwxr-xr-x  2.0 unx     2286 b- defN 19-Feb-28 08:09 sigmatools-0.8.data/scripts/sigma2misp
--rwxr-xr-x  2.0 unx     9011 b- defN 19-Feb-28 08:09 sigmatools-0.8.data/scripts/sigmac
--rw-r--r--  2.0 unx     4489 b- defN 19-Feb-28 08:11 sigmatools-0.8.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx     1174 b- defN 19-Feb-28 08:11 sigmatools-0.8.dist-info/metadata.json
--rw-r--r--  2.0 unx        6 b- defN 19-Feb-28 08:11 sigmatools-0.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 19-Feb-28 08:11 sigmatools-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx     5560 b- defN 19-Feb-28 08:11 sigmatools-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx     4753 b- defN 19-Feb-28 08:11 sigmatools-0.8.dist-info/RECORD
-52 files, 234361 bytes uncompressed, 70186 bytes compressed:  70.1%
+Zip file size: 80537 bytes, number of entries: 54
+-rw-r--r--  2.0 unx        0 b- defN 18-Jan-26 22:14 sigma/__init__.py
+-rw-r--r--  2.0 unx    12960 b- defN 19-Mar-01 23:20 sigma/configuration.py
+-rw-r--r--  2.0 unx     4768 b- defN 19-Jan-14 21:19 sigma/filter.py
+-rw-r--r--  2.0 unx     6686 b- defN 18-Aug-02 20:44 sigma/backends/arcsight.py
+-rw-r--r--  2.0 unx    10546 b- defN 19-Mar-01 23:20 sigma/backends/base.py
+-rw-r--r--  2.0 unx     1685 b- defN 18-Jul-26 22:02 sigma/backends/discovery.py
+-rw-r--r--  2.0 unx    34250 b- defN 19-Feb-25 22:16 sigma/backends/elasticsearch.py
+-rw-r--r--  2.0 unx     1164 b- defN 18-Jul-26 22:02 sigma/backends/exceptions.py
+-rw-r--r--  2.0 unx     1388 b- defN 19-Feb-25 22:16 sigma/backends/graylog.py
+-rw-r--r--  2.0 unx     2036 b- defN 19-Feb-25 22:16 sigma/backends/logpoint.py
+-rw-r--r--  2.0 unx     2093 b- defN 19-Feb-25 22:16 sigma/backends/misc.py
+-rw-r--r--  2.0 unx     2895 b- defN 18-Jul-26 22:02 sigma/backends/mixins.py
+-rw-r--r--  2.0 unx     4439 b- defN 19-Jan-14 21:19 sigma/backends/netwitness.py
+-rw-r--r--  2.0 unx     8381 b- defN 19-Feb-25 22:16 sigma/backends/powershell.py
+-rw-r--r--  2.0 unx     8613 b- defN 19-Jan-14 21:19 sigma/backends/qradar.py
+-rw-r--r--  2.0 unx     4138 b- defN 18-Aug-02 20:44 sigma/backends/qualys.py
+-rw-r--r--  2.0 unx     7573 b- defN 19-Feb-25 22:16 sigma/backends/splunk.py
+-rw-r--r--  2.0 unx    11392 b- defN 19-Feb-25 22:16 sigma/backends/sumologic.py
+-rw-r--r--  2.0 unx     2806 b- defN 18-Aug-02 20:44 sigma/backends/tools.py
+-rw-r--r--  2.0 unx    10429 b- defN 19-Mar-01 23:20 sigma/backends/wdatp.py
+-rw-r--r--  2.0 unx      885 b- defN 19-Mar-01 23:20 sigma/config/exceptions.py
+-rw-r--r--  2.0 unx    10061 b- defN 19-Mar-01 23:20 sigma/config/mapping.py
+-rw-r--r--  2.0 unx     3304 b- defN 19-Mar-01 23:20 sigma/parser/base.py
+-rw-r--r--  2.0 unx     3471 b- defN 18-Aug-14 19:36 sigma/parser/collection.py
+-rw-r--r--  2.0 unx    26326 b- defN 19-Mar-01 23:20 sigma/parser/condition.py
+-rw-r--r--  2.0 unx      817 b- defN 18-Jul-26 22:02 sigma/parser/exceptions.py
+-rw-r--r--  2.0 unx     7148 b- defN 19-Mar-01 23:20 sigma/parser/rule.py
+-rw-r--r--  2.0 unx     2227 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/arcsight.yml
+-rw-r--r--  2.0 unx       31 b- defN 17-Nov-14 19:58 sigmatools-0.9.data/data/etc/sigma/elk-defaultindex-filebeat.yml
+-rw-r--r--  2.0 unx       31 b- defN 17-Nov-14 19:58 sigmatools-0.9.data/data/etc/sigma/elk-defaultindex-logstash.yml
+-rw-r--r--  2.0 unx       48 b- defN 17-Oct-22 22:46 sigmatools-0.9.data/data/etc/sigma/elk-defaultindex.yml
+-rw-r--r--  2.0 unx      345 b- defN 17-Oct-22 22:46 sigmatools-0.9.data/data/etc/sigma/elk-linux.yml
+-rw-r--r--  2.0 unx      841 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/elk-windows.yml
+-rw-r--r--  2.0 unx     3752 b- defN 19-Mar-01 23:20 sigmatools-0.9.data/data/etc/sigma/elk-winlogbeat.yml
+-rw-r--r--  2.0 unx     4601 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/helk.yml
+-rw-r--r--  2.0 unx     3346 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/logpoint-windows-all.yml
+-rw-r--r--  2.0 unx     1641 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/netwitness.yml
+-rw-r--r--  2.0 unx     1715 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/powershell-windows-all.yml
+-rw-r--r--  2.0 unx      659 b- defN 19-Jan-14 21:19 sigmatools-0.9.data/data/etc/sigma/qradar.yml
+-rw-r--r--  2.0 unx      395 b- defN 18-Jun-26 21:30 sigmatools-0.9.data/data/etc/sigma/qualys.yml
+-rw-r--r--  2.0 unx     1510 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/spark.yml
+-rw-r--r--  2.0 unx     1820 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/splunk-windows-all.yml
+-rw-r--r--  2.0 unx     1371 b- defN 19-Feb-25 22:16 sigmatools-0.9.data/data/etc/sigma/sumologic.yml
+-rw-r--r--  2.0 unx      211 b- defN 19-Mar-01 23:20 sigmatools-0.9.data/data/etc/sigma/generic/sysmon.yml
+-rw-r--r--  2.0 unx      328 b- defN 19-Mar-01 23:20 sigmatools-0.9.data/data/etc/sigma/generic/windows-audit.yml
+-rwxr-xr-x  2.0 unx     1313 b- defN 19-Mar-01 23:40 sigmatools-0.9.data/scripts/merge_sigma
+-rwxr-xr-x  2.0 unx     2286 b- defN 19-Mar-01 23:40 sigmatools-0.9.data/scripts/sigma2misp
+-rwxr-xr-x  2.0 unx     9294 b- defN 19-Mar-01 23:40 sigmatools-0.9.data/scripts/sigmac
+-rw-r--r--  2.0 unx     4489 b- defN 19-Mar-01 23:43 sigmatools-0.9.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     1174 b- defN 19-Mar-01 23:43 sigmatools-0.9.dist-info/metadata.json
+-rw-r--r--  2.0 unx        6 b- defN 19-Mar-01 23:43 sigmatools-0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 19-Mar-01 23:43 sigmatools-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx     5560 b- defN 19-Mar-01 23:43 sigmatools-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx     4981 b- defN 19-Mar-01 23:43 sigmatools-0.9.dist-info/RECORD
+54 files, 244321 bytes uncompressed, 72575 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -75,83 +75,89 @@
 
 Filename: sigma/parser/exceptions.py
 Comment: 
 
 Filename: sigma/parser/rule.py
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/arcsight.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/arcsight.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/elk-defaultindex-filebeat.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/elk-defaultindex-filebeat.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/elk-defaultindex-logstash.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/elk-defaultindex-logstash.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/elk-defaultindex.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/elk-defaultindex.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/elk-linux.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/elk-linux.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/elk-windows.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/elk-windows.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/elk-winlogbeat.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/elk-winlogbeat.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/helk.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/helk.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/logpoint-windows-all.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/logpoint-windows-all.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/netwitness.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/netwitness.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/powershell-windows-all.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/powershell-windows-all.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/qradar.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/qradar.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/qualys.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/qualys.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/spark.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/spark.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/splunk-windows-all.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/splunk-windows-all.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/data/etc/sigma/sumologic.yml
+Filename: sigmatools-0.9.data/data/etc/sigma/sumologic.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/scripts/merge_sigma
+Filename: sigmatools-0.9.data/data/etc/sigma/generic/sysmon.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/scripts/sigma2misp
+Filename: sigmatools-0.9.data/data/etc/sigma/generic/windows-audit.yml
 Comment: 
 
-Filename: sigmatools-0.8.data/scripts/sigmac
+Filename: sigmatools-0.9.data/scripts/merge_sigma
 Comment: 
 
-Filename: sigmatools-0.8.dist-info/DESCRIPTION.rst
+Filename: sigmatools-0.9.data/scripts/sigma2misp
 Comment: 
 
-Filename: sigmatools-0.8.dist-info/metadata.json
+Filename: sigmatools-0.9.data/scripts/sigmac
 Comment: 
 
-Filename: sigmatools-0.8.dist-info/top_level.txt
+Filename: sigmatools-0.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: sigmatools-0.8.dist-info/WHEEL
+Filename: sigmatools-0.9.dist-info/metadata.json
 Comment: 
 
-Filename: sigmatools-0.8.dist-info/METADATA
+Filename: sigmatools-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sigmatools-0.8.dist-info/RECORD
+Filename: sigmatools-0.9.dist-info/WHEEL
+Comment: 
+
+Filename: sigmatools-0.9.dist-info/METADATA
+Comment: 
+
+Filename: sigmatools-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sigma/configuration.py

```diff
@@ -13,25 +13,84 @@
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import yaml
 from sigma.parser.condition import ConditionAND, ConditionOR
 from sigma.config.exceptions import SigmaConfigParseError
-from sigma.config.mapping import FieldMapping
+from sigma.config.mapping import FieldMapping, FieldMappingChain
+
+# Chain of multiple configurations
+class SigmaConfigurationChain(list):
+    """
+    Chain of SigmaConfiguration objects. Behaves like a list of Sigma configuration objects on the one side and
+    like a SigmaConfiguration object on the other. All methods are applied to the given parameters in the order
+    of addition of the configurations.
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.backend = None
+        self.defaultindex = None
+        self.config = dict()
+        self.fieldmappings = dict()
+        self.logsources = dict()
+
+        for config in self:
+            self.postprocess_config(config)
+
+    def append(self, config):
+        super().append(config)
+        self.postprocess_config(config)
+
+    def postprocess_config(self, config):
+        self.defaultindex = config.defaultindex
+        self.config.update(config.config)
+        self.fieldmappings.update(config.fieldmappings)
+        self.logsources.update(config.logsources)
+
+    def get_fieldmapping(self, fieldname):
+        """Return mapped fieldname by iterative application of each config stored in configuration chain."""
+        if self:
+            fieldmappings = FieldMappingChain(fieldname)
+            for config in self:
+                fieldmappings.append(config)
+            return fieldmappings
+        else:
+            return FieldMapping(fieldname)
+
+    def get_logsource(self, category, product, service):
+        """Return merged log source definition of all logosurces that match criteria across all Sigma conversion configurations in chain."""
+        matching = list()
+        for config in self:
+            for logsource in config.logsources:
+                if logsource.matches(category, product, service):
+                    matching.append(logsource)
+                    if logsource.rewrite is not None:
+                        category, product, service = logsource.rewrite
+        return SigmaLogsourceConfiguration(matching, self.defaultindex)
+
+    def set_backend(self, backend):
+        """Set backend for all sigma conversion configurations in chain."""
+        self.backend = backend
+        for config in self:
+            config.set_backend(backend)
+
+    def get_indexfield(self):
+        """Get index condition if index field name is configured"""
+        if self.backend is not None:
+            return self.backend.index_field
 
 # Configuration
 class SigmaConfiguration:
     """Sigma converter configuration. Contains field mappings and logsource descriptions"""
     def __init__(self, configyaml=None):
         if configyaml == None:
             self.config = None
             self.fieldmappings = dict()
             self.logsources = dict()
-            self.logsourcemerging = SigmaLogsourceConfiguration.MM_AND
             self.defaultindex = None
             self.backend = None
         else:
             config = yaml.safe_load(configyaml)
             self.config = config
 
             self.fieldmappings = dict()
@@ -40,19 +99,14 @@
                     self.fieldmappings[source] = FieldMapping(source, target)
             except KeyError:
                 pass
             if type(self.fieldmappings) != dict:
                 raise SigmaConfigParseError("Fieldmappings must be a map")
 
             try:
-                self.logsourcemerging = config['logsourcemerging']
-            except KeyError:
-                self.logsourcemerging = SigmaLogsourceConfiguration.MM_AND
-
-            try:
                 self.defaultindex = config['defaultindex']
             except KeyError:
                 self.defaultindex = None
 
             self.logsources = list()
             self.backend = None
 
@@ -73,40 +127,48 @@
         self.backend = backend
         if self.config != None:
             if 'logsources' in self.config:
                 logsources = self.config['logsources']
                 if type(logsources) != dict:
                     raise SigmaConfigParseError("Logsources must be a map")
                 for name, logsource in logsources.items():
-                    self.logsources.append(SigmaLogsourceConfiguration(logsource, self.defaultindex, name, self.logsourcemerging, self.get_indexfield()))
+                    self.logsources.append(SigmaLogsourceConfiguration(logsource, self.defaultindex))
 
     def get_indexfield(self):
         """Get index condition if index field name is configured"""
-        if self.backend != None:
+        if self.backend is not None:
             return self.backend.index_field
 
 class SigmaLogsourceConfiguration:
     """Contains the definition of a log source"""
-    MM_AND = "and"  # Merge all conditions with AND
-    MM_OR  = "or"   # Merge all conditions with OR
-
-    def __init__(self, logsource=None, defaultindex=None, name=None, mergemethod=MM_AND, indexfield=None):
-        self.name = name
-        self.indexfield = indexfield
+    def __init__(self, logsource=None, defaultindex=None):
         if logsource == None:               # create empty object
+            self.merged = False
             self.category = None
             self.product = None
             self.service = None
             self.index = list()
-            self.conditions = None
-        elif type(logsource) == list and all([isinstance(o, SigmaLogsourceConfiguration) for o in logsource]):      # list of SigmaLogsourceConfigurations: merge according to mergemethod
+            self.conditions = list()    # a list of (field, value) tuples which are OR-linked in the generated query. May also contain such a list as list element (in case of merged log sources)
+            self.rewrite = None
+        elif type(logsource) == list and all([isinstance(o, SigmaLogsourceConfiguration) for o in logsource]):      # list of SigmaLogsourceConfigurations: merge
+            self.merged = True
+            if any([ ls.merged for ls in logsource ]):      # Ensure that already merged objects are not merged again
+                raise TypeError("Nested merging of SigmaLogsourceConfiguration objects is not allowed")
+            rewrites = { ls.rewrite for ls in logsource if ls.rewrite is not None }
+            if len(rewrites) > 1:
+                raise ValueError("More than one matching log source contains a rewrite part")
+            elif len(rewrites) == 1:
+                self.rewrite = rewrites.pop()
+            else:
+                self.rewrite = None
+
             # Merge category, product and service
-            categories = set([ ls.category for ls in logsource if ls.category != None ])
-            products = set([ ls.product for ls in logsource if ls.product != None ])
-            services = set([ ls.service for ls in logsource if ls.service != None])
+            categories = { ls.category for ls in logsource if ls.category is not None }
+            products = { ls.product for ls in logsource if ls.product is not None }
+            services = { ls.service for ls in logsource if ls.service is not None }
             if len(categories) > 1 or len(products) > 1 or len(services) > 1:
                 raise ValueError("Merged SigmaLogsourceConfigurations must have disjunct categories (%s), products (%s) and services (%s)" % (str(categories), str(products), str(services)))
 
             try:
                 self.category = categories.pop()
             except KeyError:
                 self.category = None
@@ -125,36 +187,17 @@
                 if type(defaultindex) == str:
                     self.index = [defaultindex]
                 elif type(defaultindex) == list and all([type(i) == str for i in defaultindex]):
                     self.index = defaultindex
                 else:
                     raise TypeError("Default index must be string or list of strings")
 
-            # "merge" index field (should never differ between instances because it is provided by backend class
-            indexfields = [ ls.indexfield for ls in logsource if ls.indexfield != None ]
-            try:
-                self.indexfield = indexfields[0]
-            except IndexError:
-                self.indexfield = None
-
-            # Merge conditions according to mergemethod
-            if mergemethod == self.MM_AND:
-                cond = ConditionAND()
-            elif mergemethod == self.MM_OR:
-                cond = ConditionOR()
-            else:
-                raise ValueError("Mergemethod must be '%s' or '%s'" % (self.MM_AND, self.MM_OR))
-            for ls in logsource:
-                if ls.conditions != None:
-                    cond.add(ls.conditions)
-            if len(cond) > 0:
-                self.conditions = cond
-            else:
-                self.conditions = None
+            self.conditions = [ ls.conditions for ls in logsource if ls.conditions ]        # build list of list of (field, value) tuples as base for merged query condition.
         elif type(logsource) == dict:       # create logsource configuration from parsed yaml
+            self.merged = False
             if 'category' in logsource and type(logsource['category']) != str \
                     or 'product' in logsource and type(logsource['product']) != str \
                     or 'service' in logsource and type(logsource['service']) != str:
                 raise SigmaConfigParseError("Logsource category, product or service must be a string")
             try:
                 self.category = logsource['category']
             except KeyError:
@@ -166,14 +209,26 @@
             try:
                 self.service = logsource['service']
             except KeyError:
                 self.service = None
             if self.category == None and self.product == None and self.service == None:
                 raise SigmaConfigParseError("Log source definition will not match")
 
+            try:
+                if type(logsource['rewrite']) is not dict:
+                    raise SigmaConfigParseError("Rewrite rule must be a map")
+                rewrite = logsource['rewrite']
+                if not { 'category', 'product', 'service' }.issuperset(rewrite.keys()):
+                    raise SigmaConfigParseError("Rewrite rule in log source configuration may only contain the keys 'category', 'product' and 'service'")
+                if { str } != { type(value) for value in rewrite.values() }:
+                    raise SigmaConfigParseError("Rewrite rule values may only contain strings")
+                self.rewrite = tuple((rewrite.get(key) for key in ( 'category', 'product', 'service' )))    # build a (category, product, service) tuple from dict
+            except KeyError:
+                self.rewrite = None
+
             if 'index' in logsource:
                 index = logsource['index']
                 if type(index) not in (str, list):
                     raise SigmaConfigParseError("Logsource index must be string or list of strings")
                 if type(index) == list and not all([type(index) == str for index in logsource['index']]):
                     raise SigmaConfigParseError("Logsource index patterns must be strings")
                 if type(index) == list:
@@ -182,23 +237,20 @@
                     self.index = [ index ]
             else:
                 # no default index handling here - this branch is executed if log source definitions are parsed from
                 # config and these must not necessarily contain an index definition. A valid index may later be result
                 # from a merge, where default index handling applies.
                 self.index = []
 
-            if 'conditions' in logsource:
+            try:
                 if type(logsource['conditions']) != dict:
                     raise SigmaConfigParseError("Logsource conditions must be a map")
-                cond = ConditionAND()
-                for key, value in logsource['conditions'].items():
-                    cond.add((key, value))
-                self.conditions = cond
-            else:
-                self.conditions = None
+                self.conditions = [ (field, value) for field, value in logsource['conditions'].items() ]    # build list of (field, value) tuples as base for query condition
+            except KeyError:
+                self.conditions = list()
         else:
             raise SigmaConfigParseError("Logsource definitions must be maps")
 
     def matches(self, category, product, service):
         """Match log source definition against given criteria, None = ignore"""
         searched = 0
         for searchval, selfval in zip((category, product, service), (self.category, self.product, self.service)):
@@ -207,19 +259,9 @@
             if selfval != None:
                 searched += 1
                 if searchval != selfval:
                     return False
         if searched:
             return True
 
-    def get_indexcond(self):
-        """Get index condition if index field name is configured"""
-        cond = ConditionOR()
-        if self.indexfield:
-            for index in self.index:
-                cond.add((self.indexfield, index))
-            return cond
-        else:
-            return None
-
-    def __str__(self):
+    def __str__(self):  # pragma: no cover
         return "[ LogSourceConfiguration: %s %s %s indices: %s ]" % (self.category, self.product, self.service, str(self.index))
```

## sigma/backends/base.py

```diff
@@ -47,15 +47,15 @@
 
     def __init__(self, sigmaconfig, backend_options=None):
         """
         Initialize backend. This gets a sigmaconfig object, which is notified about the used backend class by
         passing the object instance to it.
         """
         super().__init__()
-        if not isinstance(sigmaconfig, (sigma.configuration.SigmaConfiguration, None)):
+        if not isinstance(sigmaconfig, (sigma.configuration.SigmaConfiguration, sigma.configuration.SigmaConfigurationChain, None)):
             raise TypeError("SigmaConfiguration object expected")
         self.backend_options = backend_options
         self.sigmaconfig = sigmaconfig
         self.sigmaconfig.set_backend(self)
 
         # Parse options
         for option, default_value, _, target in self.options:
```

## sigma/backends/wdatp.py

```diff
@@ -122,20 +122,25 @@
             return (("InitiatingProcessAccountDomain", domain), ("InititatingProcessAccountName", user))
         else:   # assume only user name is given if backslash is missing
             return (("InititatingProcessAccountName", src_value),)
 
     def generate(self, sigmaparser):
         self.table = None
         try:
-            self.product = sigmaparser.parsedyaml['logsource']['product']
-            self.service = sigmaparser.parsedyaml['logsource']['service']
+            self.category = sigmaparser.parsedyaml['logsource'].setdefault('category', None)
+            self.product = sigmaparser.parsedyaml['logsource'].setdefault('product', None)
+            self.service = sigmaparser.parsedyaml['logsource'].setdefault('service', None)
         except KeyError:
+            self.category = None
             self.product = None
             self.service = None
 
+        if (self.category, self.product, self.service) == ("process_creation", "windows", None):
+            self.table = "ProcessCreationEvents"
+
         return super().generate(sigmaparser)
 
     def generateBefore(self, parsed):
         if self.table is None:
             raise NotSupportedError("No WDATP table could be determined from Sigma rule")
         return "%s | where " % self.table
```

## sigma/config/exceptions.py

```diff
@@ -13,9 +13,12 @@
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 class SigmaConfigParseError(Exception):
     pass
 
+class FieldMappingError(SigmaConfigParseError):
+    pass
+
 class SigmaRuleFilterParseException(Exception):
     pass
```

## sigma/config/mapping.py

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from sigma.parser.condition import ConditionOR
-from .exceptions import SigmaConfigParseError
+from sigma.parser.condition import ConditionOR, NodeSubexpression
+from .exceptions import SigmaConfigParseError, FieldMappingError
 
 # Field Mapping Definitions
 def FieldMapping(source, target=None):
     """Determines target type and instantiate appropriate mapping type"""
     if target == None:
         return SimpleFieldMapping(source, source)
     elif type(target) == str:
@@ -43,27 +43,30 @@
     def resolve(self, key, value, sigmaparser):
         """Return mapped field name"""
         return (self.target, value)
 
     def resolve_fieldname(self, fieldname):
         return self.target
 
+    def __str__(self):  # pragma: no cover
+        return "SimpleFieldMapping: {} -> {}".format(self.source, self.target)
+
 class MultiFieldMapping(SimpleFieldMapping):
     """1:n field mapping that expands target field names into OR conditions"""
     target_type = list
 
     def resolve(self, key, value, sigmaparser):
         """Returns multiple target field names as OR condition"""
         cond = ConditionOR()
         for fieldname in self.target:
             cond.add((fieldname, value))
-        return cond
+        return NodeSubexpression(cond)
 
-    def resolve_fieldname(self, fieldname):
-        return self.target
+    def __str__(self):  # pragma: no cover
+        return "MultiFieldMapping: {} -> [{}]".format(self.source, ", ".join(self.target))
 
 class ConditionalFieldMapping(SimpleFieldMapping):
     """
     Conditional field mapping:
     * key contains field=value condition, value target mapping
     * key "default" maps when no condition matches
     * if no condition matches and there is no default, don't perform mapping
@@ -118,16 +121,100 @@
 
         if len(targets) == 1:     # result set contains only one target, return mapped item (like SimpleFieldMapping)
             return (targets.pop(), value)
         elif len(targets) > 1:        # result set contains multiple targets, return all linked as OR condition (like MultiFieldMapping)
             cond = ConditionOR()
             for target in targets:
                 cond.add((target, value))
-            return cond
+            return NodeSubexpression(cond)
         else:                       # no mapping found
             return (key, value)
 
     def resolve_fieldname(self, fieldname):
         if self.default != None:
             return self.default
         else:
             return fieldname
+
+    def __str__(self):  # pragma: no cover
+        return "ConditionalFieldMapping: {} -> {}".format(self.source, self.target)
+
+# Field mappimg chain
+class FieldMappingChain(object):
+    """
+    Chain of field mappings and fields used for calculation of a field mapping in chained conversion
+    configurations.
+
+    A chain of field mappings may fan out, as one field can map into multiple target fields and these
+    must be propagated further. As the whole chain must be completed at configuration parse time, a
+    restriction applies to conditional field mappings. These are calculated at rule conversion time and
+    therefore it is not possible to decide further mappings after conditionals and these may only appear
+    in the last configuration. This case could be solved by calculation of field mappings at rule conversion
+    time, but it is not considered as important enough to be implemented at this time.
+    """
+    def __init__(self, fieldname):
+        """Initialize field mapping chain with given field name."""
+        self.fieldmappings = set([fieldname])
+
+    def append(self, config):
+        """Propagate current possible field mappings with field mapping from configuration"""
+        if ConditionalFieldMapping in { type(fieldmapping) for fieldmapping in self.fieldmappings }:   # conditional field mapping appeared before, abort.
+            raise FieldMappingError("Conditional field mappings are only allowed in last configuration if configurations are chained.")
+
+        fieldmappings = set()
+        if type(self.fieldmappings) == str:
+            current_fieldmappings = {self.fieldmappings}
+        else:
+            current_fieldmappings = self.fieldmappings
+
+        for fieldname in current_fieldmappings:
+            mapping = config.get_fieldmapping(fieldname)
+            if type(mapping) in (SimpleFieldMapping,  MultiFieldMapping):
+                resolved_mapping = mapping.resolve_fieldname(fieldname)
+                if type(resolved_mapping) is list:
+                    fieldmappings.update(resolved_mapping)
+                else:
+                    fieldmappings.add(resolved_mapping)
+            elif type(mapping) == ConditionalFieldMapping:
+                fieldmappings.add(mapping)
+            else:
+                raise TypeError("Type '{}' is not supported by FieldMappingChain".format(str(type(mapping))))
+
+        if len(fieldmappings) == 1:
+            self.fieldmappings = fieldmappings.pop()
+        else:
+            self.fieldmappings = fieldmappings
+
+    def resolve(self, key, value, sigmaparser):
+        if type(self.fieldmappings) == str:     # one field mapping
+            return (self.fieldmappings, value)
+        elif isinstance(self.fieldmappings, SimpleFieldMapping):
+            return self.fieldmappings.resolve(key, value, sigmaparser)
+        elif type(self.fieldmappings) == set:
+            cond = ConditionOR()
+            for mapping in self.fieldmappings:
+                if type(mapping) == str:
+                    cond.add((mapping, value))
+                elif isinstance(mapping, SimpleFieldMapping):
+                    cond.add(mapping.resolve(key, value, sigmaparser))
+            return NodeSubexpression(cond)
+
+    def resolve_fieldname(self, fieldname):
+        if type(self.fieldmappings) == str:     # one field mapping
+            return self.fieldmappings
+        elif isinstance(self.fieldmappings, SimpleFieldMapping):
+            return self.fieldmappings.resolve_fieldname(fieldname)
+        elif type(self.fieldmappings) == set:
+            mappings = set()
+            for mapping in self.fieldmappings:
+                if type(mapping) == str:
+                    mappings.add(mapping)
+                elif isinstance(mapping, SimpleFieldMapping):
+                    resolved_mapping = mapping.resolve_fieldname(fieldname)
+                    if type(resolved_mapping) is list:
+                        mappings.update(resolved_mapping)
+                    else:
+                        mappings.add(resolved_mapping)
+            return list(mappings)
+
+    def __str__(self):  # pragma: no cover
+        return "FieldMappingChain: {}".format(self.fieldmappings)
```

## sigma/parser/base.py

```diff
@@ -59,9 +59,9 @@
                 setattr(self, rule[0], trans_value)
                 setattr(self, rule[0] + "_notrans", value)
             if rule[2] != None:
                 self.state = rule[2]
         if self.state not in self.finalstates:
             raise SigmaParseError("Unexpected end of aggregation expression, state=%d" % (self.state))
 
-    def __str__(self):
+    def __str__(self):  # pragma: no cover
         return "[ Parsed: %s ]" % (" ".join(["%s=%s" % (key, val) for key, val in self.__dict__.items() ]))
```

## sigma/parser/condition.py

```diff
@@ -93,15 +93,15 @@
         if type(other) == int:      # match against type
             return self.type == other
         if type(other) == str:      # match against content
             return self.matched == other
         else:
             raise NotImplementedError("SigmaConditionToken can only be compared against token type constants")
 
-    def __str__(self):
+    def __str__(self):  # pragma: no cover
         return "[ Token: %s: '%s' ]" % (self.tokenstr[self.type], self.matched)
 
 class SigmaConditionTokenizer:
     """Tokenize condition string into token sequence"""
     tokendefs = [      # list of tokens, preferred recognition in given order, (token identifier, matching regular expression). Ignored if token id == None
             (SigmaConditionToken.TOKEN_ONE,    re.compile("1 of", re.IGNORECASE)),
             (SigmaConditionToken.TOKEN_ALL,    re.compile("all of", re.IGNORECASE)),
@@ -140,15 +140,15 @@
                 else:   # no valid token identified
                     raise SigmaParseError("Unexpected token in condition at position %s" % condition)
         elif type(condition) == list:       # List of tokens to be converted into SigmaConditionTokenizer class
             self.tokens = condition
         else:
             raise TypeError("SigmaConditionTokenizer constructor expects string or list, got %s" % (type(condition)))
 
-    def __str__(self):
+    def __str__(self):  # pragma: no cover
         return " ".join([str(token) for token in self.tokens])
 
     def __iter__(self):
         return iter(self.tokens)
 
     def __len__(self):
         return len(self.tokens)
@@ -174,15 +174,15 @@
 
 ### Parse Tree Node Classes ###
 class ParseTreeNode:
     """Parse Tree Node Base Class"""
     def __init__(self):
         raise NotImplementedError("ConditionBase is no usable class")
 
-    def __str__(self):
+    def __str__(self):  # pragma: no cover
         return "[ %s: %s ]" % (self.__doc__, str([str(item) for item in self.items]))
 
 class ConditionBase(ParseTreeNode):
     """Base class for conditional operations"""
     op = COND_NONE
     items = None
 
@@ -525,39 +525,30 @@
                     tok_val1 = tokens[pos_val1]
                     tok_val2 = tokens[pos_val2]
                     treenode = operator[2](self.sigmaParser, tok_op, tok_val1, tok_val2)
                     tokens = tokens[:pos_val1] + treenode + tokens[pos_val2 + 1:]
 
         if len(tokens) != 1:     # parse tree must begin with exactly one node
             raise ValueError("Parse tree must have exactly one start node!")
-        querycond = tokens[0]
+        query_cond = tokens[0]
 
-        logsource = self.sigmaParser.get_logsource()
-        if logsource != None:
-            # 4. Integrate conditions from configuration
-            if logsource.conditions != None:
-                cond = ConditionAND()
-                cond.add(logsource.conditions)
-                cond.add(querycond)
-                querycond = cond
-
-            # 5. Integrate index conditions if applicable for backend
-            indexcond = logsource.get_indexcond()
-            if indexcond != None:
-                cond = ConditionAND()
-                cond.add(indexcond)
-                cond.add(querycond)
-                querycond = cond
+        # 4. Integrate conditions from logsources in configurations
+        ls_cond = self.sigmaParser.get_logsource_condition()
+        if ls_cond is not None:
+            cond = ConditionAND()
+            cond.add(ls_cond)
+            cond.add(query_cond)
+            query_cond = cond
 
-        return self._optimizer.optimizeTree(querycond)
+        return self._optimizer.optimizeTree(query_cond)
 
-    def __str__(self):
+    def __str__(self):  # pragma: no cover
         return str(self.parsedSearch)
 
-    def __len__(self):
+    def __len__(self):  # pragma: no cover
         return len(self.parsedSearch)
  
 # Aggregation parser
 class SigmaAggregationParser(SimpleParser):
     """Parse Sigma aggregation expression and provide parsed data"""
     parsingrules = [
             {   # State 0
```

## sigma/parser/rule.py

```diff
@@ -125,7 +125,42 @@
             product = None
         try:
             service = ls_rule['service']
         except KeyError:
             service = None
 
         return self.config.get_logsource(category, product, service)
+
+    def get_logsource_condition(self):
+        logsource = self.get_logsource()
+        if logsource is None:
+            return None
+        else:
+            if logsource.merged:    # Merged log source, flatten nested list of condition items
+                kvconds = [ item for sublscond in logsource.conditions for item in sublscond ]
+            else:                   # Simple log sources already contain flat list of conditions items
+                kvconds = logsource.conditions
+
+            # Apply field mappings
+            mapped_kvconds = list()
+            for field, value in kvconds:
+                mapping = self.config.get_fieldmapping(field)
+                mapped_kvconds.append(mapping.resolve(field, value, self))
+
+            # AND-link condition items
+            cond = ConditionAND()
+            for kvcond in mapped_kvconds:
+                cond.add(kvcond)
+
+            # Add index condition if supported by backend and defined in log source
+            index_field = self.config.get_indexfield()
+            indices = logsource.index
+            if len(indices) > 0 and index_field is not None:        # at least one index given and backend knows about indices in conditions
+                if len(indices) > 1:      # More than one index, search in all by ORing them together
+                    index_cond = ConditionOR()
+                    for index in indices:
+                        index_cond.add((index_field, index))
+                    cond.add(index_cond)
+                else:           # only one index, add directly to AND from above
+                    cond.add((index_field, indices[0]))
+
+            return cond
```

## Comparing `sigmatools-0.8.data/data/etc/sigma/arcsight.yml` & `sigmatools-0.9.data/data/etc/sigma/arcsight.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/elk-windows.yml` & `sigmatools-0.9.data/data/etc/sigma/elk-windows.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/elk-winlogbeat.yml` & `sigmatools-0.9.data/data/etc/sigma/elk-winlogbeat.yml`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,19 @@
     LogonType: event_data.LogonType
     NewProcessName: event_data.NewProcessName
     ObjectClass: event_data.ObjectClass
     ObjectName: event_data.ObjectName
     ObjectType: event_data.ObjectType
     ObjectValueName: event_data.ObjectValueName
     ParentCommandLine: event_data.ParentCommandLine
+    ParentProcessName: event_data.ParentProcessName
     ParentImage: event_data.ParentImage
     Path: event_data.Path
     PipeName: event_data.PipeName
+    ProcessCommandLine: event_data.ProcessCommandLine
     ProcessName: event_data.ProcessName
     Properties: event_data.Properties
     ServiceFileName: event_data.ServiceFileName
     ServiceName: event_data.ServiceName
     ShareName: event_data.ShareName
     Signature: event_data.Signature
     Source: event_data.Source
```

## Comparing `sigmatools-0.8.data/data/etc/sigma/helk.yml` & `sigmatools-0.9.data/data/etc/sigma/helk.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/logpoint-windows-all.yml` & `sigmatools-0.9.data/data/etc/sigma/logpoint-windows-all.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/netwitness.yml` & `sigmatools-0.9.data/data/etc/sigma/netwitness.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/powershell-windows-all.yml` & `sigmatools-0.9.data/data/etc/sigma/powershell-windows-all.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/qradar.yml` & `sigmatools-0.9.data/data/etc/sigma/qradar.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/spark.yml` & `sigmatools-0.9.data/data/etc/sigma/spark.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/splunk-windows-all.yml` & `sigmatools-0.9.data/data/etc/sigma/splunk-windows-all.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/data/etc/sigma/sumologic.yml` & `sigmatools-0.9.data/data/etc/sigma/sumologic.yml`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/scripts/merge_sigma` & `sigmatools-0.9.data/scripts/merge_sigma`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/scripts/sigma2misp` & `sigmatools-0.9.data/scripts/sigma2misp`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.data/scripts/sigmac` & `sigmatools-0.9.data/scripts/sigmac`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import yaml
 import json
 import pathlib
 import itertools
 import logging
 from sigma.parser.collection import SigmaCollectionParser
 from sigma.parser.exceptions import SigmaCollectionParseError, SigmaParseError
-from sigma.configuration import SigmaConfiguration
+from sigma.configuration import SigmaConfiguration, SigmaConfigurationChain
 from sigma.config.exceptions import SigmaConfigParseError, SigmaRuleFilterParseException
 from sigma.filter import SigmaRuleFilter
 import sigma.backends.discovery as backends
 from sigma.backends.base import BackendOptions
 from sigma.backends.exceptions import BackendError, NotSupportedError, PartialMatchError, FullMatchError
 import codecs
 
@@ -36,15 +36,15 @@
 
 logger = logging.getLogger(__name__)
 
 def print_verbose(*args, **kwargs):
     if cmdargs.verbose or cmdargs.debug:
         print(*args, **kwargs)
 
-def print_debug(*args, **kwargs):
+def print_debug(*args, **kwargs):   # pragme: no cover
     if cmdargs.debug:
         print(*args, **kwargs)
 
 def alliter(path):
     for sub in path.iterdir():
         if sub.name.startswith("."):
             continue
@@ -83,25 +83,25 @@
 y is one of: experimental, testing, stable.
 z is a word appearing in an arbitrary log source attribute.
 t is a tag that must appear in the rules tag list, case-insensitive matching.
 Multiple log source specifications are AND linked.
         """)
 argparser.add_argument("--target", "-t", default="es-qs", choices=backends.getBackendDict().keys(), help="Output target format")
 argparser.add_argument("--target-list", "-l", action="store_true", help="List available output target formats")
-argparser.add_argument("--config", "-c", help="Configuration with field name and index mapping for target environment")
+argparser.add_argument("--config", "-c", action="append", help="Configurations with field name and index mapping for target environment. Multiple configurations are merged into one. Last config is authorative in case of conflicts.")
 argparser.add_argument("--output", "-o", default=None, help="Output file or filename prefix if multiple files are generated")
 argparser.add_argument("--backend-option", "-O", action="append", help="Options and switches that are passed to the backend")
 argparser.add_argument("--defer-abort", "-d", action="store_true", help="Don't abort on parse or conversion errors, proceed with next rule. The exit code from the last error is returned")
 argparser.add_argument("--ignore-backend-errors", "-I", action="store_true", help="Only return error codes for parse errors and ignore errors for rules that cause backend errors. Useful, when you want to get as much queries as possible.")
 argparser.add_argument("--verbose", "-v", action="store_true", help="Be verbose")
 argparser.add_argument("--debug", "-D", action="store_true", help="Debugging output")
 argparser.add_argument("inputs", nargs="*", help="Sigma input files ('-' for stdin)")
 cmdargs = argparser.parse_args()
 
-if cmdargs.debug:
+if cmdargs.debug:   # pragma: no cover
     logger.setLevel(logging.DEBUG)
 
 if cmdargs.target_list:
     for backend in backends.getBackendList():
         print("%10s: %s" % (backend.identifier, backend.__doc__))
     sys.exit(0)
 elif len(cmdargs.inputs) == 0:
@@ -113,32 +113,33 @@
 if cmdargs.filter:
     try:
         rulefilter = SigmaRuleFilter(cmdargs.filter)
     except SigmaRuleFilterParseException as e:
         print("Parse error in Sigma rule filter expression: %s" % str(e), file=sys.stderr)
         sys.exit(9)
 
-sigmaconfig = SigmaConfiguration()
+sigmaconfigs = SigmaConfigurationChain()
 if cmdargs.config:
-    try:
-        conffile = cmdargs.config
-        f = open(conffile)
-        sigmaconfig = SigmaConfiguration(f)
-    except OSError as e:
-        print("Failed to open Sigma configuration file %s: %s" % (conffile, str(e)), file=sys.stderr)
-        exit(5)
-    except (yaml.parser.ParserError, yaml.scanner.ScannerError) as e:
-        print("Sigma configuration file %s is no valid YAML: %s" % (conffile, str(e)), file=sys.stderr)
-        exit(6)
-    except SigmaConfigParseError as e:
-        print("Sigma configuration parse error in %s: %s" % (conffile, str(e)), file=sys.stderr)
-        exit(7)
+    for conffile in cmdargs.config:
+        try:
+            f = open(conffile)
+            sigmaconfig = SigmaConfiguration(f)
+            sigmaconfigs.append(sigmaconfig)
+        except OSError as e:
+            print("Failed to open Sigma configuration file %s: %s" % (conffile, str(e)), file=sys.stderr)
+            exit(5)
+        except (yaml.parser.ParserError, yaml.scanner.ScannerError) as e:
+            print("Sigma configuration file %s is no valid YAML: %s" % (conffile, str(e)), file=sys.stderr)
+            exit(6)
+        except SigmaConfigParseError as e:
+            print("Sigma configuration parse error in %s: %s" % (conffile, str(e)), file=sys.stderr)
+            exit(7)
 
 backend_options = BackendOptions(cmdargs.backend_option)
-backend = backends.getBackend(cmdargs.target)(sigmaconfig, backend_options)
+backend = backends.getBackend(cmdargs.target)(sigmaconfigs, backend_options)
 filename = cmdargs.output
 if filename:
     try:
         out = open(filename, "w", encoding='utf-8')
     except (IOError, OSError) as e:
         print("Failed to open output file '%s': %s" % (filename, str(e)), file=sys.stderr)
         exit(1)
@@ -149,15 +150,15 @@
 for sigmafile in get_inputs(cmdargs.inputs, cmdargs.recurse):
     print_verbose("* Processing Sigma input %s" % (sigmafile))
     try:
         if cmdargs.inputs == ['-']:
             f = sigmafile
         else:
             f = sigmafile.open(encoding='utf-8')
-        parser = SigmaCollectionParser(f, sigmaconfig, rulefilter)
+        parser = SigmaCollectionParser(f, sigmaconfigs, rulefilter)
         results = parser.generate(backend)
         for result in results:
             print(result, file=out)
     except OSError as e:
         print("Failed to open Sigma file %s: %s" % (sigmafile, str(e)), file=sys.stderr)
         error = 5
     except (yaml.parser.ParserError, yaml.scanner.ScannerError) as e:
```

## Comparing `sigmatools-0.8.dist-info/DESCRIPTION.rst` & `sigmatools-0.9.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `sigmatools-0.8.dist-info/metadata.json` & `sigmatools-0.9.dist-info/metadata.json`

 * *Files 0% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.9'"}*

```diff
@@ -60,9 +60,9 @@
             "requires": [
                 "coverage",
                 "yamllint"
             ]
         }
     ],
     "summary": "Tools for the Generic Signature Format for SIEM Systems",
-    "version": "0.8"
+    "version": "0.9"
 }
```

## Comparing `sigmatools-0.8.dist-info/METADATA` & `sigmatools-0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: sigmatools
-Version: 0.8
+Version: 0.9
 Summary: Tools for the Generic Signature Format for SIEM Systems
 Home-page: https://github.com/Neo23x0/sigma
 Author: Sigma Project
 Author-email: thomas@patzke.org
 License: LGPLv3
 Keywords: security monitoring siem logging signatures elasticsearch splunk ids sysmon
 Platform: UNKNOWN
```

## Comparing `sigmatools-0.8.dist-info/RECORD` & `sigmatools-0.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 sigma/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sigma/configuration.py,sha256=nI1GOT3Xrcql7vQg78PVRKQmZ8Dd04quUS8nxbdI6VM,10434
+sigma/configuration.py,sha256=w4ByQ3XMo_uR-CEzOIAU37veDlQwxyvEburx_fH--Iw,12960
 sigma/filter.py,sha256=BN2BHlDmcDx9sI1JIGIl6cccbN8L0B0wY5o3LXTM1NI,4768
 sigma/backends/arcsight.py,sha256=meq-RB1uFAtluJBcordo2cg_Re7W2u1m5UOY5JHxyp4,6686
-sigma/backends/base.py,sha256=L7xupoNLZ3hbZNvSkw8epMwnXLo-QwNClqt8DfCZ8Ck,10501
+sigma/backends/base.py,sha256=sEIPoy-Ksq4fcZOtXBap4BCt5a1iNMsCQRoyh7IHrgc,10546
 sigma/backends/discovery.py,sha256=-pWzdw24whIoglkEJjXMbY79zGjdvquZndEJy98tolc,1685
 sigma/backends/elasticsearch.py,sha256=kaTehwHLFxdgFUT_l1TzfGIFobsdt7tMyhOJmnK0ZCI,34250
 sigma/backends/exceptions.py,sha256=Zbbr3grB_GaoNt-uCAjWa3x515dOiy-x1hpqs8Cipsk,1164
 sigma/backends/graylog.py,sha256=k_5o3dV8gAwts9vE2C79-Agdv1DRA2_QHAV9867G2Dc,1388
 sigma/backends/logpoint.py,sha256=bmC24me5YvsSe1Akvm5YeNWXyodFrB7814QNq3NZG3c,2036
 sigma/backends/misc.py,sha256=r1MjkgF00sJRMaZpHIgd-wdyUjVT3EtJQMApFz2ItVA,2093
 sigma/backends/mixins.py,sha256=YYL_O1-lJDYyC5zS_8RlZRkiJ-7TT2Co0beVWRAh9Co,2895
 sigma/backends/netwitness.py,sha256=W8XnQiKJs-Mh9JnGrURaFRIeKLx72SCIThXVzQsfs0g,4439
 sigma/backends/powershell.py,sha256=kqlsEEKfM2xve7-_pm8CWCUeFREM7bSXLn3hukcJqIo,8381
 sigma/backends/qradar.py,sha256=sgk3fEsbDtnkDxjwNtIPSpERyh4Li2bTcDS4nw3Cz-I,8613
 sigma/backends/qualys.py,sha256=juUMvRVny7c52lzOuZ5lTXthiaNrtbZmTqVLLFue2Xo,4138
 sigma/backends/splunk.py,sha256=tcnOGPMAmfK2EjIn6wK-OZW_fCAaGusoCLiIS6y_nYQ,7573
 sigma/backends/sumologic.py,sha256=RIz8wugq7a2GyfCpEE_FrsqzcQ2iCmrmExVfDa0GomM,11392
 sigma/backends/tools.py,sha256=gApXHJbNNe7R7QyCoWI2hN9jXSCHFMtsxH69BNfuCi0,2806
-sigma/backends/wdatp.py,sha256=eb_8JSVknNpv8JHWG0I82CnYyio1HieObepFWg69Dc0,10122
-sigma/config/exceptions.py,sha256=AU-FD1G_5CmwJK4lhjgEcQe0KakR87u02rm0Istr3rg,827
-sigma/config/mapping.py,sha256=v0ZWPm3OwKVYh157xKfqPK8VRnptBHZ4GTxXpE7CMnY,5629
-sigma/parser/base.py,sha256=PX6mv2Vr-WQXSByQ6NjeoCm9H7MkYUKNX2ZKt5fQL2k,3284
+sigma/backends/wdatp.py,sha256=JEvKThsg5mMfW2d_DmWtuPop6gO3btT_TTYbCAKn7dU,10429
+sigma/config/exceptions.py,sha256=_W2NC7yYVMfMgBMLuTpBWDahuAQbq5Fg4ibTqGtGP9M,885
+sigma/config/mapping.py,sha256=rJ-uld9KFisC7sC6LhzDmGufWKsxwSXGvkc7xJYNJZ4,10061
+sigma/parser/base.py,sha256=bfPsuexx3xU8i9MYCACNxwBx27sgtN6BW_LU0_ETCxg,3304
 sigma/parser/collection.py,sha256=VdOwlllJYWystB7lp3Lo_laRDvsLp_4E2RrO5Y-gESk,3471
-sigma/parser/condition.py,sha256=MPihO-HHsqQwQOGx-6of_-zxJKvC60EExuuVqK0HAHQ,26573
+sigma/parser/condition.py,sha256=xGK3pBq4Os4HpEqGf6zSVqCIJg_PqHjvDs33bZ1ScDw,26326
 sigma/parser/exceptions.py,sha256=8KnEtjIZ5bv2pV9Aph_IOsWFfULdNzRUDWLZIVXh2rQ,817
-sigma/parser/rule.py,sha256=P0S-X8pXrv6X6Lf6LsBoQZ8QLfcdkNGeTg8evhp_00A,5485
-sigmatools-0.8.data/data/etc/sigma/arcsight.yml,sha256=-0Ls68TdruJ6Xr94tB4UJS8JlsRtfcRWplFhy8rE8zo,2227
-sigmatools-0.8.data/data/etc/sigma/elk-defaultindex-filebeat.yml,sha256=WtQ1V9N-oQVIoaivhPfjPa3-hIEgcj9wg_rn4cDUGHY,31
-sigmatools-0.8.data/data/etc/sigma/elk-defaultindex-logstash.yml,sha256=HNRZbuU6og7aZFXB2986nEjfMV15uKqENpzXDHUzqRw,31
-sigmatools-0.8.data/data/etc/sigma/elk-defaultindex.yml,sha256=PrdBfNHm9DK-W0gx8W0Rv8cAl2nPNoit3Y81MH4dxtM,48
-sigmatools-0.8.data/data/etc/sigma/elk-linux.yml,sha256=SuZviSQIHxVgI73qhWgEC5CCcqQR6xwAXFVRngkKhMY,345
-sigmatools-0.8.data/data/etc/sigma/elk-windows.yml,sha256=D6ougEN0I-qVlOLyEbI9K6fAXswswcuX7aSSgLzpPpM,841
-sigmatools-0.8.data/data/etc/sigma/elk-winlogbeat.yml,sha256=kWDQAGwm9IpS8al6LoICIoyEWNgEulsCACzyi66Nijo,3646
-sigmatools-0.8.data/data/etc/sigma/helk.yml,sha256=UF-X5BppF191jNCDxUuDBImo3j3eCaOXzVsiDwFdnHY,4601
-sigmatools-0.8.data/data/etc/sigma/logpoint-windows-all.yml,sha256=fOzu60o1fHbfLnjC2jQeRkNQGlszAODr-oQSgyF8P58,3346
-sigmatools-0.8.data/data/etc/sigma/netwitness.yml,sha256=9lXy2uAu8vWzHyStNVmkNEHXfGyqiW7EpypukpGgZ7g,1641
-sigmatools-0.8.data/data/etc/sigma/powershell-windows-all.yml,sha256=2Wb0wm4dmzliXAzLX1jtvzA0arso0C6ZX3p4NJYO7Mo,1715
-sigmatools-0.8.data/data/etc/sigma/qradar.yml,sha256=cZwo0aGBlAtEl3jKgsgdauAr8NbBkoOWcf6STitun-E,659
-sigmatools-0.8.data/data/etc/sigma/qualys.yml,sha256=kmbeFueKaV75oyqNClw8OfB76krnS6vHJgQG5wkwjvE,395
-sigmatools-0.8.data/data/etc/sigma/spark.yml,sha256=LbFiY_fdv5cXb5BpL-EvzLb1bYcmNcPbhiGqgId9bvc,1510
-sigmatools-0.8.data/data/etc/sigma/splunk-windows-all.yml,sha256=e4ZdgZDZeG2hFXzvWkLcRpN5FKhVlhlKUbeA7bmReOY,1820
-sigmatools-0.8.data/data/etc/sigma/sumologic.yml,sha256=4sdXtMLJfE9EtXfTk4S1DVIvkZzgiRa70QT5EwvjfpQ,1371
-sigmatools-0.8.data/scripts/merge_sigma,sha256=_kovq9aDJmhPj_dKsi-YbKzWsRLKl2MNNW7uMM4p6zs,1313
-sigmatools-0.8.data/scripts/sigma2misp,sha256=8daZlnFX0Ud0eHjhIRg59CsPFTFicQ8Owtj-8ciPDC4,2286
-sigmatools-0.8.data/scripts/sigmac,sha256=anQDZwDM8h6vEjE7WLYSswAnMWLzKwYTHr9zkfbqam8,9011
-sigmatools-0.8.dist-info/DESCRIPTION.rst,sha256=jZmy3hgmJVwWmrCc7upBcDIAm7MYvsbKHqs4fXT5Pi0,4489
-sigmatools-0.8.dist-info/METADATA,sha256=xEO93oUoT8d0RIPqE3Nm1DNmaAW87j-GXb5bnv7lTtk,5560
-sigmatools-0.8.dist-info/RECORD,,
-sigmatools-0.8.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-sigmatools-0.8.dist-info/metadata.json,sha256=2oiBo8bOK8ek2icQaKRvdWHzigycDl0kMyYO8oo7HCc,1174
-sigmatools-0.8.dist-info/top_level.txt,sha256=I_VNou6ONc4M4m956fkL-E_vyIg2YVorgJ5yiqIpsxA,6
+sigma/parser/rule.py,sha256=f8YbD6SeUEZ_dmj8ecz4yc7cMn4aHE-rLuqpUROOyQk,7148
+sigmatools-0.9.data/data/etc/sigma/arcsight.yml,sha256=-0Ls68TdruJ6Xr94tB4UJS8JlsRtfcRWplFhy8rE8zo,2227
+sigmatools-0.9.data/data/etc/sigma/elk-defaultindex-filebeat.yml,sha256=WtQ1V9N-oQVIoaivhPfjPa3-hIEgcj9wg_rn4cDUGHY,31
+sigmatools-0.9.data/data/etc/sigma/elk-defaultindex-logstash.yml,sha256=HNRZbuU6og7aZFXB2986nEjfMV15uKqENpzXDHUzqRw,31
+sigmatools-0.9.data/data/etc/sigma/elk-defaultindex.yml,sha256=PrdBfNHm9DK-W0gx8W0Rv8cAl2nPNoit3Y81MH4dxtM,48
+sigmatools-0.9.data/data/etc/sigma/elk-linux.yml,sha256=SuZviSQIHxVgI73qhWgEC5CCcqQR6xwAXFVRngkKhMY,345
+sigmatools-0.9.data/data/etc/sigma/elk-windows.yml,sha256=D6ougEN0I-qVlOLyEbI9K6fAXswswcuX7aSSgLzpPpM,841
+sigmatools-0.9.data/data/etc/sigma/elk-winlogbeat.yml,sha256=HwBS13TABJ84kfHFO_t3zjUf8WctCyZ8RoLCrANcYPg,3752
+sigmatools-0.9.data/data/etc/sigma/helk.yml,sha256=UF-X5BppF191jNCDxUuDBImo3j3eCaOXzVsiDwFdnHY,4601
+sigmatools-0.9.data/data/etc/sigma/logpoint-windows-all.yml,sha256=fOzu60o1fHbfLnjC2jQeRkNQGlszAODr-oQSgyF8P58,3346
+sigmatools-0.9.data/data/etc/sigma/netwitness.yml,sha256=9lXy2uAu8vWzHyStNVmkNEHXfGyqiW7EpypukpGgZ7g,1641
+sigmatools-0.9.data/data/etc/sigma/powershell-windows-all.yml,sha256=2Wb0wm4dmzliXAzLX1jtvzA0arso0C6ZX3p4NJYO7Mo,1715
+sigmatools-0.9.data/data/etc/sigma/qradar.yml,sha256=cZwo0aGBlAtEl3jKgsgdauAr8NbBkoOWcf6STitun-E,659
+sigmatools-0.9.data/data/etc/sigma/qualys.yml,sha256=kmbeFueKaV75oyqNClw8OfB76krnS6vHJgQG5wkwjvE,395
+sigmatools-0.9.data/data/etc/sigma/spark.yml,sha256=LbFiY_fdv5cXb5BpL-EvzLb1bYcmNcPbhiGqgId9bvc,1510
+sigmatools-0.9.data/data/etc/sigma/splunk-windows-all.yml,sha256=e4ZdgZDZeG2hFXzvWkLcRpN5FKhVlhlKUbeA7bmReOY,1820
+sigmatools-0.9.data/data/etc/sigma/sumologic.yml,sha256=4sdXtMLJfE9EtXfTk4S1DVIvkZzgiRa70QT5EwvjfpQ,1371
+sigmatools-0.9.data/data/etc/sigma/generic/sysmon.yml,sha256=04nRZUntVx7UXMR2IbpzI2vbVxTXIIX5-04xvFvtlu8,211
+sigmatools-0.9.data/data/etc/sigma/generic/windows-audit.yml,sha256=vt9iLkypHuIdGV5hm2I6bnGMu2PPhJwaK5pe9YOtKHA,328
+sigmatools-0.9.data/scripts/merge_sigma,sha256=_kovq9aDJmhPj_dKsi-YbKzWsRLKl2MNNW7uMM4p6zs,1313
+sigmatools-0.9.data/scripts/sigma2misp,sha256=8daZlnFX0Ud0eHjhIRg59CsPFTFicQ8Owtj-8ciPDC4,2286
+sigmatools-0.9.data/scripts/sigmac,sha256=LgPW5D05fPotV1rW6ZlIi7lh0Z9tZpuPh96moWjfg70,9294
+sigmatools-0.9.dist-info/DESCRIPTION.rst,sha256=jZmy3hgmJVwWmrCc7upBcDIAm7MYvsbKHqs4fXT5Pi0,4489
+sigmatools-0.9.dist-info/METADATA,sha256=Enq8PKyhT5pbmdqP_bIsOfdmWmth1mrKKbLB467YdOE,5560
+sigmatools-0.9.dist-info/RECORD,,
+sigmatools-0.9.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+sigmatools-0.9.dist-info/metadata.json,sha256=UCSsAOVE2874YniA_wDuYl-RC18Mw-HjRrRav-X1zuo,1174
+sigmatools-0.9.dist-info/top_level.txt,sha256=I_VNou6ONc4M4m956fkL-E_vyIg2YVorgJ5yiqIpsxA,6
```

