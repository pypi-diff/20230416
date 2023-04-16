# Comparing `tmp/wtforms-bootstrap5-0.1.6.tar.gz` & `tmp/wtforms-bootstrap5-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtforms-bootstrap5-0.1.6.tar", max compression
+gzip compressed data, was "wtforms-bootstrap5-0.2.0.tar", max compression
```

## Comparing `wtforms-bootstrap5-0.1.6.tar` & `wtforms-bootstrap5-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-02-23 20:50:34.208137 wtforms-bootstrap5-0.1.6/LICENSE
--rw-r--r--   0        0        0     8111 2023-02-23 20:50:34.208137 wtforms-bootstrap5-0.1.6/README.md
--rw-r--r--   0        0        0      532 2023-02-23 20:50:34.208137 wtforms-bootstrap5-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      305 2023-02-23 20:50:34.212137 wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/__init__.py
--rw-r--r--   0        0        0     5635 2023-02-23 20:50:34.212137 wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/context.py
--rw-r--r--   0        0        0      805 2023-02-23 20:50:34.212137 wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/helpers.py
--rw-r--r--   0        0        0     1837 2023-02-23 20:50:34.212137 wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/registry.py
--rw-r--r--   0        0        0     6931 2023-02-23 20:50:34.212137 wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/renderers.py
--rw-r--r--   0        0        0     9067 2023-02-23 20:50:39.088661 wtforms-bootstrap5-0.1.6/setup.py
--rw-r--r--   0        0        0     8833 2023-02-23 20:50:39.089368 wtforms-bootstrap5-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9037 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/README.md
+-rw-r--r--   0        0        0      532 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/__init__.py
+-rw-r--r--   0        0        0     6160 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/context.py
+-rw-r--r--   0        0        0      805 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/helpers.py
+-rw-r--r--   0        0        0     1837 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/registry.py
+-rw-r--r--   0        0        0     7094 2023-04-16 02:50:24.072193 wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/renderers.py
+-rw-r--r--   0        0        0    10029 2023-04-16 02:50:27.472063 wtforms-bootstrap5-0.2.0/setup.py
+-rw-r--r--   0        0        0     9759 2023-04-16 02:50:27.472852 wtforms-bootstrap5-0.2.0/PKG-INFO
```

### Comparing `wtforms-bootstrap5-0.1.6/LICENSE` & `wtforms-bootstrap5-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wtforms-bootstrap5-0.1.6/README.md` & `wtforms-bootstrap5-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -149,14 +149,49 @@
         enctype="application/x-www-form-urlencoded",
         form_class="my-form",
         form_attrs=dict(custom="value")
     )
 )
 ```
 
+### Add submit button or other fields
+
+Sometimes, define a submit button for each form is not desirable.
+Or, the form could be automatically generated and doesn't come with a submit button.
+In those cases, you can use `add_field` to add any extra fields into the end of the form.
+Like this:
+
+```python
+html = (
+    renderer_context
+    .add_field("submit", SubmitField())
+    .field(
+        "submit",
+        field_wrapper_class="offset-2",
+        field_wrapper_enabled=True,
+    )
+).render(form)
+```
+
+Since adding a submit button is very common, so you can also use `add_submit` instead if the field to add is a `SubmitField`.
+
+```python
+html = (
+    renderer_context
+    .add_submit("submit")
+    .field(
+        "submit",
+        field_wrapper_class="offset-2",
+        field_wrapper_enabled=True,
+    )
+).render(form)
+```
+
+As you can see in the example, the decorate options also work for the newly added submit field.
+
 ### Field HTML structure
 
 In general, the field HTML structure can be controlled by the option values and it looks like this
 
 ```html
 <!-- enabled by .row_enabled, default: true -->
 <div class=".row_class" {.row_attrs}>
```

### Comparing `wtforms-bootstrap5-0.1.6/pyproject.toml` & `wtforms-bootstrap5-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wtforms-bootstrap5"
-version = "0.1.6"
+version = "0.2.0"
 description = "Simple library for rendering WTForms in HTML as Bootstrap 5 form controls"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/wtforms-bootstrap5"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/context.py` & `wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import typing
 
 from markupsafe import Markup
+from wtforms import SubmitField
+from wtforms.fields.core import UnboundField
 
 from .helpers import traverse_base_classes
 from .registry import DEFAULT_REGISTRY
 from .registry import FormElement
 from .registry import RendererRegistry
 
 
@@ -98,25 +100,32 @@
     help_class: typing.Optional[str] = "form-text"
     # extra attributes help message div
     help_attrs: typing.Dict[str, str] = dataclasses.field(default_factory=dict)
     # enable help message
     help_enabled: bool = True
 
 
+@dataclasses.dataclass(frozen=True)
+class ExtraField:
+    name: str
+    field: UnboundField
+
+
 class RendererContext:
     def __init__(
         self,
         registry: RendererRegistry = DEFAULT_REGISTRY,
         default_form_options: FormOptions = FormOptions(),
         default_field_options: FieldOptions = FieldOptions(),
     ):
         self.form_options = default_form_options
         self.default_field_options = default_field_options
         self.registry = registry
         self.field_options: typing.Dict[str, FieldOptions] = {}
+        self.extra_fields: typing.List[UnboundField] = []
 
     def form(self, **kwargs) -> RendererContext:
         old_options = dataclasses.asdict(self.form_options)
         self.form_options = FormOptions(**(old_options | kwargs))
         return self
 
     def field(self, *names: str, **kwargs: str) -> RendererContext:
@@ -129,14 +138,21 @@
 
     def default_field(self, **kwargs: str) -> RendererContext:
         self.default_field_options = FieldOptions(
             **(dataclasses.asdict(self.default_field_options) | kwargs)
         )
         return self
 
+    def add_field(self, name: str, field: UnboundField) -> RendererContext:
+        self.extra_fields.append(ExtraField(name=name, field=field))
+        return self
+
+    def add_submit(self, name="submit", **kwargs) -> RendererContext:
+        return self.add_field(name, SubmitField(**kwargs))
+
     def render(self, element: FormElement) -> Markup:
         base_class_paths: typing.List[typing.Tuple] = traverse_base_classes(
             cls=element.__class__
         )
         for path in base_class_paths:
             current_metadata = self.registry.class_metadata
             metadatas = [current_metadata]
```

### Comparing `wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/helpers.py` & `wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/helpers.py`

 * *Files identical despite different names*

### Comparing `wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/registry.py` & `wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/registry.py`

 * *Files identical despite different names*

### Comparing `wtforms-bootstrap5-0.1.6/wtforms_bootstrap5/renderers.py` & `wtforms-bootstrap5-0.2.0/wtforms_bootstrap5/renderers.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
 
 @register(target_cls=Form)
 def render_form(context: RendererContext, element: FormElement) -> Markup:
     form: Form = element
     form_options = context.form_options
     fields = [context.render(field) for field in form._fields.values()]
+    for extra_field in context.extra_fields:
+        field = extra_field.field.bind(form=form, name=extra_field.name)
+        fields.append(context.render(field))
     content = "\n".join(fields)
     base_attrs = {}
     if form_options.action is not None:
         base_attrs["action"] = form_options.action
     if form_options.method is not None:
         base_attrs["method"] = form_options.method
     if form_options.enctype is not None:
```

### Comparing `wtforms-bootstrap5-0.1.6/setup.py` & `wtforms-bootstrap5-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['WTForms>=3.0.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'wtforms-bootstrap5',
-    'version': '0.1.6',
+    'version': '0.2.0',
     'description': 'Simple library for rendering WTForms in HTML as Bootstrap 5 form controls',
-    'long_description': '# WTForms-Bootstrap5\nSimple library for rendering WTForms in HTML as Bootstrap 5 form controls\n\n**Notice: this project is still in very early stage, the API may change a lots rapidly**\n\n## Features\n\n- **MIT licensed** - it doesn\'t infect your code\n- **Light weight** - not much code and little dependencies\n- **Latest Bootstrap 5** - generates forms in latest Bootstrap 5 style \n- **Highly customizable** - you can generate different kind of Bootstrap 5 form controls and layouts\n- **Template engine friendly** - chained method calls making it easy to integrate with template engine\n- **Covered with automatic tests** - yep, we have test cases\n\n## Why?\n\nEverytime I build a website with [WTForms](https://wtforms.readthedocs.io), I spend way too much time in writing HTML and [Jinja template](https://jinja.palletsprojects.com/) for rendering a form as [Bootstrap 5 form controls](https://getbootstrap.com/docs/5.2/forms/overview/).\nWork smart is an important value we have here at [Launch Platform](https://launchplatform.com), so I wonder why not make a library for making rendering Bootstrap 5 style WTForms controls easily?\nSo here you go, wtforms-bootstrap5 is created, open sourced under MIT license.\nIt\'s a simple Python library for rendering WTForms in Bootstrap 5 favor.\n\n## Install\n\nTo install the formatter, simply run\n\n```bash\npip install wtforms-bootstrap5\n```\n\n## Example\n\nFirst, you define your form as you would usually do with WTForms:\n\n```python\nfrom wtforms import Form\nfrom wtforms import EmailField\nfrom wtforms import PasswordField\nfrom wtforms import SelectField\nfrom wtforms import BooleanField\nfrom wtforms import SubmitField\n\n\nclass MyForm(Form):\n    email = EmailField("Email", render_kw=dict(placeholder="Foobar"))\n    password = PasswordField("Password", description="Your super secret password")\n    city = SelectField("City", choices=["Los Angle", "San Francisco", "New York"])\n    agree_terms = BooleanField("I agrees to terms and service")\n    submit = SubmitField()\n\n```\n\nThen you can use `RenderContext` for rendering your form like this\n\n```python\nfrom wtforms_bootstrap5 import RendererContext\n\nform = MyForm()\ncontext = RendererContext()\nhtml = context.render(form)\n```\n\nThe form will be rendered as HTML like\n\n```html\n<form method="POST"><div class="mb-3"><label class="form-label" for="email">Email</label><input class="form-control" id="email" name="email" type="email" value=""></div>\n<div class="mb-3"><label class="form-label" for="password">Password</label><input class="form-control" id="password" name="password" type="password" value=""><div class="form-text">Your super secret password</div></div>\n<div class="mb-3"><label class="form-label" for="city">City</label><select class="form-select" id="city" name="city"><option value="Los Angle">Los Angle</option><option value="San Francisco">San Francisco</option><option value="New York">New York</option></select></div>\n<div class="mb-3"><div class="form-check"><label class="form-check-label" for="agree_terms">I agrees to terms and service</label><input class="form-check-input" id="agree_terms" name="agree_terms" type="checkbox" value="y"></div></div>\n<div class="mb-3"><input class="btn btn-primary" id="submit" name="submit" type="submit" value="Submit"></div></form>\n```\n\nAnd it will look like this\n\n<p align="center">\n  <img src="assets/default-style-example.png?raw=true" alt="Form rendered in Bootstrap 5 favor" />\n</p>\n\nBy default, a sensible simple layout style will be used.\n\n## Customize the form\n\nThere are many similar open source libraries out there, but most of them are very hard to customize.\nOnce you adopt it, then you can only render your form in a specific style.\nAs a result, I found myself writing HTML manually without using the library to save time.\n\nTo avoid the same mistake, we want to make wtforms-bootstrap5 very easy to customize without compromising too much of its reusability.\nHere\'s an example how you can turn the example above into a column based form.\n\n```python\nhtml = (\n    renderer_context\n    .form(action="/sign-up")\n    .default_field(\n        row_class="row mb-3",\n        label_class="form-label col-2",\n        field_wrapper_class="col-10",\n        field_wrapper_enabled=True,\n    )\n    .field(\n        "agree_terms",\n        wrapper_class="offset-2",\n        wrapper_enabled=True,\n        field_wrapper_enabled=False,\n    )\n    .field(\n        "submit",\n        field_wrapper_class="offset-2",\n        field_wrapper_enabled=True,\n    )\n).render(form)\n```\n\nAnd this is how it looks like\n\n<p align="center">\n  <img src="assets/column-style-example.png?raw=true" alt="Form rendered in Bootstrap 5 favor" />\n</p>\n\nAs you can see in the example, we use `default_field` method for overwriting the options of all fields by default.\nWe also use `field` method for overwriting the options for a specific field.\nThe `field` method takes multiple input name arguments, so that you can overwrite options for multiple fields at once like this\n\n```python\nhtml = (context\n    .field("email", "password", label_class="my-custom-class", ...)\n)\n```\n\nPlease notice that, **the order of `default_field` and `field` method calls matter**.\nWhen `field` is called, the current default field options will be used as the default values.\nSo if you make the calls in order like this\n\n```python\nhtml = (context\n    .field("email", row_class="row")\n    .default_field(label_class="my-custom-class")\n)\n```\n\nThe `label_class` for `email` field here will be `form-label` instead of `my-custom-class` since when it\'s called, the original default value was still `form-label`.\n\nTo customize the form element, you can use the `form` method like this\n\n```python\nhtml = (context\n    .form(\n        method="POST",\n        action="/sign-up",\n        enctype="application/x-www-form-urlencoded",\n        form_class="my-form",\n        form_attrs=dict(custom="value")\n    )\n)\n```\n\n### Field HTML structure\n\nIn general, the field HTML structure can be controlled by the option values and it looks like this\n\n```html\n<!-- enabled by .row_enabled, default: true -->\n<div class=".row_class" {.row_attrs}>\n  <!-- enabled by .wrapper_enabled, default: false -->\n  <div class=".wrapper_class" {.wrapper_attrs}>\n    <!-- enabled by .label_enabled, default: true -->\n    <label class=".label_class" for="email" {.label_attrs}>Email</label>\n    <!-- enabled by .field_wrapper_enabled, default: false -->\n    <div class=".field_wrapper" {.field_wrapper_attrs}>\n      <input class=".field_class" id="email" name="email" type="email" value="" {.field_attrs}>\n      <!-- enabled by .help_enabled, default: true -->\n      <div class=".help_class" {.helper_attrs}>Your super secret password</div>\n      <!-- enabled by .error_enabled, default: true -->\n      <div class=".error_class" {.error_attrs}>Bad password</div>\n    </div>\n  </div>\n</div>\n```\n\n## Integrate with template engine\n\nWe want to make it as easy as possible to integrate with template engine such as [Jinja](https://jinja.palletsprojects.com/).\nThat\'s why we use chained method calls for customizing the form.\nYou should be able to pass the `form` and `RenderContext` objects and write all your form customization from the template.\nThis way, you don\'t get your view relative code pollute your controller code.\nFor example, after passing `form` and `render_context` object, you can write this in Jinja:\n\n```html\n<h1>New user</h1>\n\n{{\n    renderer_context\n        .default_field(\n            row_class="row mb-3",\n            label_class="form-label col-2",\n            field_wrapper_class="col-10",\n            field_wrapper_enabled=True,\n        )\n        .field(\n            "agree_terms",\n            wrapper_class="offset-2",\n            wrapper_enabled=True,\n            field_wrapper_enabled=False,\n        )\n        .field(\n            "submit",\n            field_wrapper_class="offset-2",\n            field_wrapper_enabled=True,\n        )\n    ).render(form)\n}}\n```\n\n## Feedbacks\n\nFeedbacks, bugs reporting or feature requests are welcome 🙌, just please open an issue.\nNo guarantee we have time to deal with them, but will see what we can do.\n',
+    'long_description': '# WTForms-Bootstrap5\nSimple library for rendering WTForms in HTML as Bootstrap 5 form controls\n\n**Notice: this project is still in very early stage, the API may change a lots rapidly**\n\n## Features\n\n- **MIT licensed** - it doesn\'t infect your code\n- **Light weight** - not much code and little dependencies\n- **Latest Bootstrap 5** - generates forms in latest Bootstrap 5 style \n- **Highly customizable** - you can generate different kind of Bootstrap 5 form controls and layouts\n- **Template engine friendly** - chained method calls making it easy to integrate with template engine\n- **Covered with automatic tests** - yep, we have test cases\n\n## Why?\n\nEverytime I build a website with [WTForms](https://wtforms.readthedocs.io), I spend way too much time in writing HTML and [Jinja template](https://jinja.palletsprojects.com/) for rendering a form as [Bootstrap 5 form controls](https://getbootstrap.com/docs/5.2/forms/overview/).\nWork smart is an important value we have here at [Launch Platform](https://launchplatform.com), so I wonder why not make a library for making rendering Bootstrap 5 style WTForms controls easily?\nSo here you go, wtforms-bootstrap5 is created, open sourced under MIT license.\nIt\'s a simple Python library for rendering WTForms in Bootstrap 5 favor.\n\n## Install\n\nTo install the formatter, simply run\n\n```bash\npip install wtforms-bootstrap5\n```\n\n## Example\n\nFirst, you define your form as you would usually do with WTForms:\n\n```python\nfrom wtforms import Form\nfrom wtforms import EmailField\nfrom wtforms import PasswordField\nfrom wtforms import SelectField\nfrom wtforms import BooleanField\nfrom wtforms import SubmitField\n\n\nclass MyForm(Form):\n    email = EmailField("Email", render_kw=dict(placeholder="Foobar"))\n    password = PasswordField("Password", description="Your super secret password")\n    city = SelectField("City", choices=["Los Angle", "San Francisco", "New York"])\n    agree_terms = BooleanField("I agrees to terms and service")\n    submit = SubmitField()\n\n```\n\nThen you can use `RenderContext` for rendering your form like this\n\n```python\nfrom wtforms_bootstrap5 import RendererContext\n\nform = MyForm()\ncontext = RendererContext()\nhtml = context.render(form)\n```\n\nThe form will be rendered as HTML like\n\n```html\n<form method="POST"><div class="mb-3"><label class="form-label" for="email">Email</label><input class="form-control" id="email" name="email" type="email" value=""></div>\n<div class="mb-3"><label class="form-label" for="password">Password</label><input class="form-control" id="password" name="password" type="password" value=""><div class="form-text">Your super secret password</div></div>\n<div class="mb-3"><label class="form-label" for="city">City</label><select class="form-select" id="city" name="city"><option value="Los Angle">Los Angle</option><option value="San Francisco">San Francisco</option><option value="New York">New York</option></select></div>\n<div class="mb-3"><div class="form-check"><label class="form-check-label" for="agree_terms">I agrees to terms and service</label><input class="form-check-input" id="agree_terms" name="agree_terms" type="checkbox" value="y"></div></div>\n<div class="mb-3"><input class="btn btn-primary" id="submit" name="submit" type="submit" value="Submit"></div></form>\n```\n\nAnd it will look like this\n\n<p align="center">\n  <img src="assets/default-style-example.png?raw=true" alt="Form rendered in Bootstrap 5 favor" />\n</p>\n\nBy default, a sensible simple layout style will be used.\n\n## Customize the form\n\nThere are many similar open source libraries out there, but most of them are very hard to customize.\nOnce you adopt it, then you can only render your form in a specific style.\nAs a result, I found myself writing HTML manually without using the library to save time.\n\nTo avoid the same mistake, we want to make wtforms-bootstrap5 very easy to customize without compromising too much of its reusability.\nHere\'s an example how you can turn the example above into a column based form.\n\n```python\nhtml = (\n    renderer_context\n    .form(action="/sign-up")\n    .default_field(\n        row_class="row mb-3",\n        label_class="form-label col-2",\n        field_wrapper_class="col-10",\n        field_wrapper_enabled=True,\n    )\n    .field(\n        "agree_terms",\n        wrapper_class="offset-2",\n        wrapper_enabled=True,\n        field_wrapper_enabled=False,\n    )\n    .field(\n        "submit",\n        field_wrapper_class="offset-2",\n        field_wrapper_enabled=True,\n    )\n).render(form)\n```\n\nAnd this is how it looks like\n\n<p align="center">\n  <img src="assets/column-style-example.png?raw=true" alt="Form rendered in Bootstrap 5 favor" />\n</p>\n\nAs you can see in the example, we use `default_field` method for overwriting the options of all fields by default.\nWe also use `field` method for overwriting the options for a specific field.\nThe `field` method takes multiple input name arguments, so that you can overwrite options for multiple fields at once like this\n\n```python\nhtml = (context\n    .field("email", "password", label_class="my-custom-class", ...)\n)\n```\n\nPlease notice that, **the order of `default_field` and `field` method calls matter**.\nWhen `field` is called, the current default field options will be used as the default values.\nSo if you make the calls in order like this\n\n```python\nhtml = (context\n    .field("email", row_class="row")\n    .default_field(label_class="my-custom-class")\n)\n```\n\nThe `label_class` for `email` field here will be `form-label` instead of `my-custom-class` since when it\'s called, the original default value was still `form-label`.\n\nTo customize the form element, you can use the `form` method like this\n\n```python\nhtml = (context\n    .form(\n        method="POST",\n        action="/sign-up",\n        enctype="application/x-www-form-urlencoded",\n        form_class="my-form",\n        form_attrs=dict(custom="value")\n    )\n)\n```\n\n### Add submit button or other fields\n\nSometimes, define a submit button for each form is not desirable.\nOr, the form could be automatically generated and doesn\'t come with a submit button.\nIn those cases, you can use `add_field` to add any extra fields into the end of the form.\nLike this:\n\n```python\nhtml = (\n    renderer_context\n    .add_field("submit", SubmitField())\n    .field(\n        "submit",\n        field_wrapper_class="offset-2",\n        field_wrapper_enabled=True,\n    )\n).render(form)\n```\n\nSince adding a submit button is very common, so you can also use `add_submit` instead if the field to add is a `SubmitField`.\n\n```python\nhtml = (\n    renderer_context\n    .add_submit("submit")\n    .field(\n        "submit",\n        field_wrapper_class="offset-2",\n        field_wrapper_enabled=True,\n    )\n).render(form)\n```\n\nAs you can see in the example, the decorate options also work for the newly added submit field.\n\n### Field HTML structure\n\nIn general, the field HTML structure can be controlled by the option values and it looks like this\n\n```html\n<!-- enabled by .row_enabled, default: true -->\n<div class=".row_class" {.row_attrs}>\n  <!-- enabled by .wrapper_enabled, default: false -->\n  <div class=".wrapper_class" {.wrapper_attrs}>\n    <!-- enabled by .label_enabled, default: true -->\n    <label class=".label_class" for="email" {.label_attrs}>Email</label>\n    <!-- enabled by .field_wrapper_enabled, default: false -->\n    <div class=".field_wrapper" {.field_wrapper_attrs}>\n      <input class=".field_class" id="email" name="email" type="email" value="" {.field_attrs}>\n      <!-- enabled by .help_enabled, default: true -->\n      <div class=".help_class" {.helper_attrs}>Your super secret password</div>\n      <!-- enabled by .error_enabled, default: true -->\n      <div class=".error_class" {.error_attrs}>Bad password</div>\n    </div>\n  </div>\n</div>\n```\n\n## Integrate with template engine\n\nWe want to make it as easy as possible to integrate with template engine such as [Jinja](https://jinja.palletsprojects.com/).\nThat\'s why we use chained method calls for customizing the form.\nYou should be able to pass the `form` and `RenderContext` objects and write all your form customization from the template.\nThis way, you don\'t get your view relative code pollute your controller code.\nFor example, after passing `form` and `render_context` object, you can write this in Jinja:\n\n```html\n<h1>New user</h1>\n\n{{\n    renderer_context\n        .default_field(\n            row_class="row mb-3",\n            label_class="form-label col-2",\n            field_wrapper_class="col-10",\n            field_wrapper_enabled=True,\n        )\n        .field(\n            "agree_terms",\n            wrapper_class="offset-2",\n            wrapper_enabled=True,\n            field_wrapper_enabled=False,\n        )\n        .field(\n            "submit",\n            field_wrapper_class="offset-2",\n            field_wrapper_enabled=True,\n        )\n    ).render(form)\n}}\n```\n\n## Feedbacks\n\nFeedbacks, bugs reporting or feature requests are welcome 🙌, just please open an issue.\nNo guarantee we have time to deal with them, but will see what we can do.\n',
     'author': 'Fang-Pen Lin',
     'author_email': 'fangpen@launchplatform.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/LaunchPlatform/wtforms-bootstrap5',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wtforms-bootstrap5-0.1.6/PKG-INFO` & `wtforms-bootstrap5-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtforms-bootstrap5
-Version: 0.1.6
+Version: 0.2.0
 Summary: Simple library for rendering WTForms in HTML as Bootstrap 5 form controls
 Home-page: https://github.com/LaunchPlatform/wtforms-bootstrap5
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -167,14 +167,49 @@
         enctype="application/x-www-form-urlencoded",
         form_class="my-form",
         form_attrs=dict(custom="value")
     )
 )
 ```
 
+### Add submit button or other fields
+
+Sometimes, define a submit button for each form is not desirable.
+Or, the form could be automatically generated and doesn't come with a submit button.
+In those cases, you can use `add_field` to add any extra fields into the end of the form.
+Like this:
+
+```python
+html = (
+    renderer_context
+    .add_field("submit", SubmitField())
+    .field(
+        "submit",
+        field_wrapper_class="offset-2",
+        field_wrapper_enabled=True,
+    )
+).render(form)
+```
+
+Since adding a submit button is very common, so you can also use `add_submit` instead if the field to add is a `SubmitField`.
+
+```python
+html = (
+    renderer_context
+    .add_submit("submit")
+    .field(
+        "submit",
+        field_wrapper_class="offset-2",
+        field_wrapper_enabled=True,
+    )
+).render(form)
+```
+
+As you can see in the example, the decorate options also work for the newly added submit field.
+
 ### Field HTML structure
 
 In general, the field HTML structure can be controlled by the option values and it looks like this
 
 ```html
 <!-- enabled by .row_enabled, default: true -->
 <div class=".row_class" {.row_attrs}>
```

