# Comparing `tmp/imagemangler-0.1.5.tar.gz` & `tmp/imagemangler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagemangler-0.1.5.tar", max compression
+gzip compressed data, was "imagemangler-0.1.6.tar", max compression
```

## Comparing `imagemangler-0.1.5.tar` & `imagemangler-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      856 2023-04-12 18:32:44.389305 imagemangler-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.5/imagemangler/__init__.py
--rw-r--r--   0        0        0     1889 2023-04-12 18:50:06.765976 imagemangler-0.1.5/imagemangler/cli.py
--rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.5/imagemangler/core/__init__.py
--rw-r--r--   0        0        0      564 2023-04-12 18:29:29.685971 imagemangler-0.1.5/imagemangler/core/mangler.py
--rw-r--r--   0        0        0      567 2023-04-12 18:29:29.689304 imagemangler-0.1.5/imagemangler/core/utils.py
--rw-r--r--   0        0        0      548 2023-04-12 18:50:13.935976 imagemangler-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 imagemangler-0.1.5/setup.py
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 imagemangler-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1034 2023-04-13 14:03:36.787075 imagemangler-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 10:06:57.002508 imagemangler-0.1.6/imagemangler/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-13 12:28:11.783497 imagemangler-0.1.6/imagemangler/cli.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:09:01.962509 imagemangler-0.1.6/imagemangler/core/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-13 12:08:34.746781 imagemangler-0.1.6/imagemangler/core/mangler.py
+-rw-r--r--   0        0        0      567 2023-04-13 11:47:19.910060 imagemangler-0.1.6/imagemangler/core/utils.py
+-rw-r--r--   0        0        0      758 2023-04-16 15:00:01.688883 imagemangler-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 imagemangler-0.1.6/setup.py
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 imagemangler-0.1.6/PKG-INFO
```

### Comparing `imagemangler-0.1.5/README.md` & `imagemangler-0.1.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,65 @@
-00000000: 215b 6c6f 676f 5d28 6874 7470 733a 2f2f  ![logo](https://
-00000010: 6769 7468 7562 2e63 6f6d 2f6d 6967 7565  github.com/migue
-00000020: 6c76 616c 656e 7465 2f69 6d61 6765 6d61  lvalente/imagema
-00000030: 6e67 6c65 722f 626c 6f62 2f6d 6173 7465  ngler/blob/maste
-00000040: 722f 6c6f 676f 2e70 6e67 3f72 6177 3d74  r/logo.png?raw=t
-00000050: 7275 6529 0a0a 0a49 6d61 6765 204d 616e  rue)...Image Man
-00000060: 676c 6572 2069 7320 6120 636f 6d6d 616e  gler is a comman
-00000070: 642d 6c69 6e65 2074 6f6f 6c20 746f 2064  d-line tool to d
-00000080: 6574 6572 696f 7261 7465 2061 6e20 696d  eteriorate an im
-00000090: 6167 6520 6974 6572 6174 6976 656c 7920  age iteratively 
-000000a0: 7573 696e 6720 6c6f 7373 7920 616c 676f  using lossy algo
-000000b0: 7269 7468 6d73 2e0a 0a23 2049 6e73 7461  rithms...# Insta
-000000c0: 6c6c 6174 696f 6e0a 0a59 6f75 2063 616e  llation..You can
-000000d0: 2069 6e73 7461 6c6c 2049 6d61 6765 204d   install Image M
-000000e0: 616e 676c 6572 2076 6961 2070 6970 3a0a  angler via pip:.
-000000f0: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-00000100: 7461 6c6c 2069 6d61 6765 6d61 6e67 6c65  tall imagemangle
-00000110: 720a 6060 600a 0a23 2055 7361 6765 0a0a  r.```..# Usage..
-00000120: 596f 7520 6361 6e20 7275 6e20 496d 6167  You can run Imag
-00000130: 6520 4d61 6e67 6c65 7220 6279 2069 6e76  e Mangler by inv
-00000140: 6f6b 696e 6720 7468 6520 696d 6167 656d  oking the imagem
-00000150: 616e 676c 6572 2063 6f6d 6d61 6e64 2069  angler command i
-00000160: 6e20 7468 6520 7465 726d 696e 616c 2c20  n the terminal, 
-00000170: 666f 6c6c 6f77 6564 2062 7920 7468 6520  followed by the 
-00000180: 7061 7468 206f 6620 7468 6520 696d 6167  path of the imag
-00000190: 6520 6669 6c65 2079 6f75 2077 616e 7420  e file you want 
-000001a0: 746f 206d 616e 676c 653a 0a0a 6060 6062  to mangle:..```b
-000001b0: 6173 680a 696d 6167 656d 616e 676c 6572  ash.imagemangler
-000001c0: 2070 6174 682f 746f 2f69 6d61 6765 2e6a   path/to/image.j
-000001d0: 7067 0a60 6060 0a0a 4279 2064 6566 6175  pg.```..By defau
-000001e0: 6c74 2c20 496d 6167 6520 4d61 6e67 6c65  lt, Image Mangle
-000001f0: 7220 7769 6c6c 2061 7574 6f6d 6174 6963  r will automatic
-00000200: 616c 6c79 206d 616e 676c 6520 7468 6520  ally mangle the 
-00000210: 696d 6167 6520 6163 726f 7373 2061 6c6c  image across all
-00000220: 2071 7561 6c69 7479 2073 7465 7073 2077   quality steps w
-00000230: 6974 6820 6120 6261 7365 2071 7561 6c69  ith a base quali
-00000240: 7479 206f 6620 3730 2061 6e64 2061 2071  ty of 70 and a q
-00000250: 7561 6c69 7479 2073 7465 7020 6f66 2032  uality step of 2
-00000260: 2e20 596f 7520 6361 6e20 7370 6563 6966  . You can specif
-00000270: 7920 796f 7572 206f 776e 2076 616c 7565  y your own value
-00000280: 7320 666f 7220 7468 6573 6520 7061 7261  s for these para
-00000290: 6d65 7465 7273 2075 7369 6e67 2074 6865  meters using the
-000002a0: 206f 7074 696f 6e61 6c20 666c 6167 733a   optional flags:
-000002b0: 0a0a 0a60 6060 6261 7368 0a69 6d61 6765  ...```bash.image
-000002c0: 6d61 6e67 6c65 7220 7061 7468 2f74 6f2f  mangler path/to/
-000002d0: 696d 6167 652e 6a70 6720 2d2d 7175 616c  image.jpg --qual
-000002e0: 6974 7920 3630 202d 2d71 7561 6c69 7479  ity 60 --quality
-000002f0: 2d73 7465 7020 3520 2d2d 6e6f 2d61 7574  -step 5 --no-aut
-00000300: 6f2d 6d61 6e67 6c65 0a60 6060 0a0a 466f  o-mangle.```..Fo
-00000310: 7220 6120 6d6f 7265 2064 6574 6169 6c73  r a more details
-00000320: 2079 6f75 2063 616e 2075 7365 2060 2d2d   you can use `--
-00000330: 6865 6c70 603a 0a0a 6060 6062 6173 680a  help`:..```bash.
-00000340: 696d 6167 656d 616e 676c 6572 202d 2d68  imagemangler --h
-00000350: 656c 700a 6060 600a                      elp.```.
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000020: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000030: 2f6d 6967 7565 6c76 616c 656e 7465 2f69  /miguelvalente/i
+00000040: 6d61 6765 6d61 6e67 6c65 722f 626c 6f62  magemangler/blob
+00000050: 2f6d 6173 7465 722f 6c6f 676f 2e70 6e67  /master/logo.png
+00000060: 3f72 6177 3d74 7275 6522 3e3c 696d 6720  ?raw=true"><img 
+00000070: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000080: 6875 622e 636f 6d2f 6d69 6775 656c 7661  hub.com/miguelva
+00000090: 6c65 6e74 652f 696d 6167 656d 616e 676c  lente/imagemangl
+000000a0: 6572 2f62 6c6f 622f 6d61 7374 6572 2f6c  er/blob/master/l
+000000b0: 6f67 6f2e 706e 673f 7261 773d 7472 7565  ogo.png?raw=true
+000000c0: 2220 616c 743d 2249 6d61 6765 4d61 6e67  " alt="ImageMang
+000000d0: 6c65 7222 3e3c 2f61 3e0a 3c2f 703e 0a3c  ler"></a>.</p>.<
+000000e0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000000f0: 3e0a 2020 2020 3c65 6d3e 496d 6167 6520  >.    <em>Image 
+00000100: 4d61 6e67 6c65 7220 6973 2061 2063 6f6d  Mangler is a com
+00000110: 6d61 6e64 2d6c 696e 6520 746f 6f6c 2074  mand-line tool t
+00000120: 6f20 6465 7465 7269 6f72 6174 6520 616e  o deteriorate an
+00000130: 2069 6d61 6765 2069 7465 7261 7469 7665   image iterative
+00000140: 6c79 2075 7369 6e67 206c 6f73 7379 2061  ly using lossy a
+00000150: 6c67 6f72 6974 686d 732e 3c2f 656d 3e0a  lgorithms.</em>.
+00000160: 3c2f 703e 0a0a 2d2d 2d0a 0a23 2049 6e73  </p>..---..# Ins
+00000170: 7461 6c6c 6174 696f 6e0a 0a59 6f75 2063  tallation..You c
+00000180: 616e 2069 6e73 7461 6c6c 2049 6d61 6765  an install Image
+00000190: 204d 616e 676c 6572 2076 6961 2070 6970   Mangler via pip
+000001a0: 3a0a 0a60 6060 6261 7368 0a70 6970 2069  :..```bash.pip i
+000001b0: 6e73 7461 6c6c 2069 6d61 6765 6d61 6e67  nstall imagemang
+000001c0: 6c65 720a 6060 600a 0a23 2055 7361 6765  ler.```..# Usage
+000001d0: 0a0a 596f 7520 6361 6e20 7275 6e20 496d  ..You can run Im
+000001e0: 6167 6520 4d61 6e67 6c65 7220 6279 2069  age Mangler by i
+000001f0: 6e76 6f6b 696e 6720 7468 6520 696d 6167  nvoking the imag
+00000200: 656d 616e 676c 6572 2063 6f6d 6d61 6e64  emangler command
+00000210: 2069 6e20 7468 6520 7465 726d 696e 616c   in the terminal
+00000220: 2c20 666f 6c6c 6f77 6564 2062 7920 7468  , followed by th
+00000230: 6520 7061 7468 206f 6620 7468 6520 696d  e path of the im
+00000240: 6167 6520 6669 6c65 2079 6f75 2077 616e  age file you wan
+00000250: 7420 746f 206d 616e 676c 653a 0a0a 6060  t to mangle:..``
+00000260: 6062 6173 680a 696d 6167 656d 616e 676c  `bash.imagemangl
+00000270: 6572 2070 6174 682f 746f 2f69 6d61 6765  er path/to/image
+00000280: 2e6a 7067 0a60 6060 0a0a 4279 2064 6566  .jpg.```..By def
+00000290: 6175 6c74 2c20 496d 6167 6520 4d61 6e67  ault, Image Mang
+000002a0: 6c65 7220 7769 6c6c 2061 7574 6f6d 6174  ler will automat
+000002b0: 6963 616c 6c79 206d 616e 676c 6520 7468  ically mangle th
+000002c0: 6520 696d 6167 6520 6163 726f 7373 2061  e image across a
+000002d0: 6c6c 2071 7561 6c69 7479 2073 7465 7073  ll quality steps
+000002e0: 2077 6974 6820 6120 6261 7365 2071 7561   with a base qua
+000002f0: 6c69 7479 206f 6620 3730 2061 6e64 2061  lity of 70 and a
+00000300: 2071 7561 6c69 7479 2073 7465 7020 6f66   quality step of
+00000310: 2032 2e20 596f 7520 6361 6e20 7370 6563   2. You can spec
+00000320: 6966 7920 796f 7572 206f 776e 2076 616c  ify your own val
+00000330: 7565 7320 666f 7220 7468 6573 6520 7061  ues for these pa
+00000340: 7261 6d65 7465 7273 2075 7369 6e67 2074  rameters using t
+00000350: 6865 206f 7074 696f 6e61 6c20 666c 6167  he optional flag
+00000360: 733a 0a0a 0a60 6060 6261 7368 0a69 6d61  s:...```bash.ima
+00000370: 6765 6d61 6e67 6c65 7220 7061 7468 2f74  gemangler path/t
+00000380: 6f2f 696d 6167 652e 6a70 6720 2d2d 7175  o/image.jpg --qu
+00000390: 616c 6974 7920 3630 202d 2d71 7561 6c69  ality 60 --quali
+000003a0: 7479 2d73 7465 7020 3520 2d2d 6e6f 2d61  ty-step 5 --no-a
+000003b0: 7574 6f2d 6d61 6e67 6c65 0a60 6060 0a0a  uto-mangle.```..
+000003c0: 466f 7220 6120 6d6f 7265 2064 6574 6169  For a more detai
+000003d0: 6c73 2079 6f75 2063 616e 2075 7365 2060  ls you can use `
+000003e0: 2d2d 6865 6c70 603a 0a0a 6060 6062 6173  --help`:..```bas
+000003f0: 680a 696d 6167 656d 616e 676c 6572 202d  h.imagemangler -
+00000400: 2d68 656c 700a 6060 600a                 -help.```.
```

### Comparing `imagemangler-0.1.5/imagemangler/cli.py` & `imagemangler-0.1.6/imagemangler/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,19 @@
         True, help="Automatically mangle the image across all quality steps"
     ),
 ):
     """
     Mangle an image by deteriorating it iteratively with
     quality reduction of lossy algorithms
     """
+    # write a funtion to change the extension of the image to jpeg if it is jpg
     extension = image_path.split(".")[-1]
+    if extension == "jpg":
+        extension = "jpeg"
+
     img = Image.open(io.BytesIO(open(image_path, "rb").read()))
 
     mangled_images = []
     while True:
         img = deteriorate(img, extension=extension, quality=quality)
         mangled_images.append(img)
 
@@ -48,18 +52,18 @@
     image_name = image_path.split("/")[-1]
     image_no_ext = image_name.split(".")[0]
 
     print("🖨")
     print(f"Your image `{image_name}` was mangled {len(mangled_images)} times!")
     print("🖨")
 
-    if typer.confirm("Do you want to save all mangled images?"):
+    if typer.confirm("Do you want to save all mangled images?", default=True):
         with zipfile.ZipFile(f"mangled_{image_no_ext}.zip", "w") as zip_file:
             zip_images(zip_file, mangled_images, extension)
         print(f"Your mangled images were saved to mangled_{image_no_ext}.zip")
-    elif typer.confirm("Do you want to save the last mangled image?"):
-        img.save(f"mangled_img.{extension}")
+    elif typer.confirm("Do you want to save the last mangled image?", default=True):
+        img.save(f"mangled_img.{extension}", format=extension)
         print(f"Your mangled image was saved to mangled_img.{extension}")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `imagemangler-0.1.5/imagemangler/core/mangler.py` & `imagemangler-0.1.6/imagemangler/core/mangler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import io
 
 from PIL import Image
 
 
 def deteriorate(
-    img: Image,
+    img: Image.Image,
     extension,
     optimize: bool = True,
     quality: int = 20,
-) -> Image:
+) -> Image.Image:
     """Deteriorate the image quality for `iterations` number of times"""
 
     compressed_buffer = io.BytesIO()
     img.save(compressed_buffer, format=extension, optimize=optimize, quality=quality)
 
     # Get the compressed image data as bytes
     compressed_bytes = compressed_buffer.getvalue()
```

### Comparing `imagemangler-0.1.5/imagemangler/core/utils.py` & `imagemangler-0.1.6/imagemangler/core/utils.py`

 * *Files identical despite different names*

### Comparing `imagemangler-0.1.5/pyproject.toml` & `imagemangler-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imagemangler"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["miguelvalente <miguelvalente@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pillow = "^9.5.0"
@@ -13,14 +13,25 @@
 numpy = "^1.24.2"
 
 [tool.poetry.group.dev]
 optional=true
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
+mypy = "^1.2.0"
+types-pillow = "^9.4.0.19"
+ruff = "^0.0.261"
+pytest = "^7.3.0"
+coverage = "^7.2.3"
+pytest-cov = "^4.0.0"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 imagemangler = "imagemangler.cli:app"
+
+[[tool.mypy.overrides]]
+module = "cv2.*"
+ignore_missing_imports = true
```

### Comparing `imagemangler-0.1.5/setup.py` & `imagemangler-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,89 +20,101 @@
 00000130: 7269 7074 7327 3a20 5b27 696d 6167 656d  ripts': ['imagem
 00000140: 616e 676c 6572 203d 2069 6d61 6765 6d61  angler = imagema
 00000150: 6e67 6c65 722e 636c 693a 6170 7027 5d7d  ngler.cli:app']}
 00000160: 0a0a 7365 7475 705f 6b77 6172 6773 203d  ..setup_kwargs =
 00000170: 207b 0a20 2020 2027 6e61 6d65 273a 2027   {.    'name': '
 00000180: 696d 6167 656d 616e 676c 6572 272c 0a20  imagemangler',. 
 00000190: 2020 2027 7665 7273 696f 6e27 3a20 2730     'version': '0
-000001a0: 2e31 2e35 272c 0a20 2020 2027 6465 7363  .1.5',.    'desc
+000001a0: 2e31 2e36 272c 0a20 2020 2027 6465 7363  .1.6',.    'desc
 000001b0: 7269 7074 696f 6e27 3a20 2727 2c0a 2020  ription': '',.  
 000001c0: 2020 276c 6f6e 675f 6465 7363 7269 7074    'long_descript
-000001d0: 696f 6e27 3a20 2721 5b6c 6f67 6f5d 2868  ion': '![logo](h
-000001e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001f0: 6d2f 6d69 6775 656c 7661 6c65 6e74 652f  m/miguelvalente/
-00000200: 696d 6167 656d 616e 676c 6572 2f62 6c6f  imagemangler/blo
-00000210: 622f 6d61 7374 6572 2f6c 6f67 6f2e 706e  b/master/logo.pn
-00000220: 673f 7261 773d 7472 7565 295c 6e5c 6e5c  g?raw=true)\n\n\
-00000230: 6e49 6d61 6765 204d 616e 676c 6572 2069  nImage Mangler i
-00000240: 7320 6120 636f 6d6d 616e 642d 6c69 6e65  s a command-line
-00000250: 2074 6f6f 6c20 746f 2064 6574 6572 696f   tool to deterio
-00000260: 7261 7465 2061 6e20 696d 6167 6520 6974  rate an image it
-00000270: 6572 6174 6976 656c 7920 7573 696e 6720  eratively using 
-00000280: 6c6f 7373 7920 616c 676f 7269 7468 6d73  lossy algorithms
-00000290: 2e5c 6e5c 6e23 2049 6e73 7461 6c6c 6174  .\n\n# Installat
-000002a0: 696f 6e5c 6e5c 6e59 6f75 2063 616e 2069  ion\n\nYou can i
-000002b0: 6e73 7461 6c6c 2049 6d61 6765 204d 616e  nstall Image Man
-000002c0: 676c 6572 2076 6961 2070 6970 3a5c 6e5c  gler via pip:\n\
-000002d0: 6e60 6060 6261 7368 5c6e 7069 7020 696e  n```bash\npip in
-000002e0: 7374 616c 6c20 696d 6167 656d 616e 676c  stall imagemangl
-000002f0: 6572 5c6e 6060 605c 6e5c 6e23 2055 7361  er\n```\n\n# Usa
-00000300: 6765 5c6e 5c6e 596f 7520 6361 6e20 7275  ge\n\nYou can ru
-00000310: 6e20 496d 6167 6520 4d61 6e67 6c65 7220  n Image Mangler 
-00000320: 6279 2069 6e76 6f6b 696e 6720 7468 6520  by invoking the 
-00000330: 696d 6167 656d 616e 676c 6572 2063 6f6d  imagemangler com
-00000340: 6d61 6e64 2069 6e20 7468 6520 7465 726d  mand in the term
-00000350: 696e 616c 2c20 666f 6c6c 6f77 6564 2062  inal, followed b
-00000360: 7920 7468 6520 7061 7468 206f 6620 7468  y the path of th
-00000370: 6520 696d 6167 6520 6669 6c65 2079 6f75  e image file you
-00000380: 2077 616e 7420 746f 206d 616e 676c 653a   want to mangle:
-00000390: 5c6e 5c6e 6060 6062 6173 685c 6e69 6d61  \n\n```bash\nima
-000003a0: 6765 6d61 6e67 6c65 7220 7061 7468 2f74  gemangler path/t
-000003b0: 6f2f 696d 6167 652e 6a70 675c 6e60 6060  o/image.jpg\n```
-000003c0: 5c6e 5c6e 4279 2064 6566 6175 6c74 2c20  \n\nBy default, 
-000003d0: 496d 6167 6520 4d61 6e67 6c65 7220 7769  Image Mangler wi
-000003e0: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
-000003f0: 206d 616e 676c 6520 7468 6520 696d 6167   mangle the imag
-00000400: 6520 6163 726f 7373 2061 6c6c 2071 7561  e across all qua
-00000410: 6c69 7479 2073 7465 7073 2077 6974 6820  lity steps with 
-00000420: 6120 6261 7365 2071 7561 6c69 7479 206f  a base quality o
-00000430: 6620 3730 2061 6e64 2061 2071 7561 6c69  f 70 and a quali
-00000440: 7479 2073 7465 7020 6f66 2032 2e20 596f  ty step of 2. Yo
-00000450: 7520 6361 6e20 7370 6563 6966 7920 796f  u can specify yo
-00000460: 7572 206f 776e 2076 616c 7565 7320 666f  ur own values fo
-00000470: 7220 7468 6573 6520 7061 7261 6d65 7465  r these paramete
-00000480: 7273 2075 7369 6e67 2074 6865 206f 7074  rs using the opt
-00000490: 696f 6e61 6c20 666c 6167 733a 5c6e 5c6e  ional flags:\n\n
-000004a0: 5c6e 6060 6062 6173 685c 6e69 6d61 6765  \n```bash\nimage
-000004b0: 6d61 6e67 6c65 7220 7061 7468 2f74 6f2f  mangler path/to/
-000004c0: 696d 6167 652e 6a70 6720 2d2d 7175 616c  image.jpg --qual
-000004d0: 6974 7920 3630 202d 2d71 7561 6c69 7479  ity 60 --quality
-000004e0: 2d73 7465 7020 3520 2d2d 6e6f 2d61 7574  -step 5 --no-aut
-000004f0: 6f2d 6d61 6e67 6c65 5c6e 6060 605c 6e5c  o-mangle\n```\n\
-00000500: 6e46 6f72 2061 206d 6f72 6520 6465 7461  nFor a more deta
-00000510: 696c 7320 796f 7520 6361 6e20 7573 6520  ils you can use 
-00000520: 602d 2d68 656c 7060 3a5c 6e5c 6e60 6060  `--help`:\n\n```
-00000530: 6261 7368 5c6e 696d 6167 656d 616e 676c  bash\nimagemangl
-00000540: 6572 202d 2d68 656c 705c 6e60 6060 5c6e  er --help\n```\n
-00000550: 272c 0a20 2020 2027 6175 7468 6f72 273a  ',.    'author':
-00000560: 2027 6d69 6775 656c 7661 6c65 6e74 6527   'miguelvalente'
-00000570: 2c0a 2020 2020 2761 7574 686f 725f 656d  ,.    'author_em
-00000580: 6169 6c27 3a20 276d 6967 7565 6c76 616c  ail': 'miguelval
-00000590: 656e 7465 4070 726f 746f 6e6d 6169 6c2e  ente@protonmail.
-000005a0: 636f 6d27 2c0a 2020 2020 276d 6169 6e74  com',.    'maint
-000005b0: 6169 6e65 7227 3a20 274e 6f6e 6527 2c0a  ainer': 'None',.
-000005c0: 2020 2020 276d 6169 6e74 6169 6e65 725f      'maintainer_
-000005d0: 656d 6169 6c27 3a20 274e 6f6e 6527 2c0a  email': 'None',.
-000005e0: 2020 2020 2775 726c 273a 2027 4e6f 6e65      'url': 'None
-000005f0: 272c 0a20 2020 2027 7061 636b 6167 6573  ',.    'packages
-00000600: 273a 2070 6163 6b61 6765 732c 0a20 2020  ': packages,.   
-00000610: 2027 7061 636b 6167 655f 6461 7461 273a   'package_data':
-00000620: 2070 6163 6b61 6765 5f64 6174 612c 0a20   package_data,. 
-00000630: 2020 2027 696e 7374 616c 6c5f 7265 7175     'install_requ
-00000640: 6972 6573 273a 2069 6e73 7461 6c6c 5f72  ires': install_r
-00000650: 6571 7569 7265 732c 0a20 2020 2027 656e  equires,.    'en
-00000660: 7472 795f 706f 696e 7473 273a 2065 6e74  try_points': ent
-00000670: 7279 5f70 6f69 6e74 732c 0a20 2020 2027  ry_points,.    '
-00000680: 7079 7468 6f6e 5f72 6571 7569 7265 7327  python_requires'
-00000690: 3a20 273e 3d33 2e31 302c 3c34 2e30 272c  : '>=3.10,<4.0',
-000006a0: 0a7d 0a0a 0a73 6574 7570 282a 2a73 6574  .}...setup(**set
-000006b0: 7570 5f6b 7761 7267 7329 0a              up_kwargs).
+000001d0: 696f 6e27 3a20 273c 7020 616c 6967 6e3d  ion': '<p align=
+000001e0: 2263 656e 7465 7222 3e5c 6e20 203c 6120  "center">\n  <a 
+000001f0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000200: 7468 7562 2e63 6f6d 2f6d 6967 7565 6c76  thub.com/miguelv
+00000210: 616c 656e 7465 2f69 6d61 6765 6d61 6e67  alente/imagemang
+00000220: 6c65 722f 626c 6f62 2f6d 6173 7465 722f  ler/blob/master/
+00000230: 6c6f 676f 2e70 6e67 3f72 6177 3d74 7275  logo.png?raw=tru
+00000240: 6522 3e3c 696d 6720 7372 633d 2268 7474  e"><img src="htt
+00000250: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000260: 6d69 6775 656c 7661 6c65 6e74 652f 696d  miguelvalente/im
+00000270: 6167 656d 616e 676c 6572 2f62 6c6f 622f  agemangler/blob/
+00000280: 6d61 7374 6572 2f6c 6f67 6f2e 706e 673f  master/logo.png?
+00000290: 7261 773d 7472 7565 2220 616c 743d 2249  raw=true" alt="I
+000002a0: 6d61 6765 4d61 6e67 6c65 7222 3e3c 2f61  mageMangler"></a
+000002b0: 3e5c 6e3c 2f70 3e5c 6e3c 7020 616c 6967  >\n</p>\n<p alig
+000002c0: 6e3d 2263 656e 7465 7222 3e5c 6e20 2020  n="center">\n   
+000002d0: 203c 656d 3e49 6d61 6765 204d 616e 676c   <em>Image Mangl
+000002e0: 6572 2069 7320 6120 636f 6d6d 616e 642d  er is a command-
+000002f0: 6c69 6e65 2074 6f6f 6c20 746f 2064 6574  line tool to det
+00000300: 6572 696f 7261 7465 2061 6e20 696d 6167  eriorate an imag
+00000310: 6520 6974 6572 6174 6976 656c 7920 7573  e iteratively us
+00000320: 696e 6720 6c6f 7373 7920 616c 676f 7269  ing lossy algori
+00000330: 7468 6d73 2e3c 2f65 6d3e 5c6e 3c2f 703e  thms.</em>\n</p>
+00000340: 5c6e 5c6e 2d2d 2d5c 6e5c 6e23 2049 6e73  \n\n---\n\n# Ins
+00000350: 7461 6c6c 6174 696f 6e5c 6e5c 6e59 6f75  tallation\n\nYou
+00000360: 2063 616e 2069 6e73 7461 6c6c 2049 6d61   can install Ima
+00000370: 6765 204d 616e 676c 6572 2076 6961 2070  ge Mangler via p
+00000380: 6970 3a5c 6e5c 6e60 6060 6261 7368 5c6e  ip:\n\n```bash\n
+00000390: 7069 7020 696e 7374 616c 6c20 696d 6167  pip install imag
+000003a0: 656d 616e 676c 6572 5c6e 6060 605c 6e5c  emangler\n```\n\
+000003b0: 6e23 2055 7361 6765 5c6e 5c6e 596f 7520  n# Usage\n\nYou 
+000003c0: 6361 6e20 7275 6e20 496d 6167 6520 4d61  can run Image Ma
+000003d0: 6e67 6c65 7220 6279 2069 6e76 6f6b 696e  ngler by invokin
+000003e0: 6720 7468 6520 696d 6167 656d 616e 676c  g the imagemangl
+000003f0: 6572 2063 6f6d 6d61 6e64 2069 6e20 7468  er command in th
+00000400: 6520 7465 726d 696e 616c 2c20 666f 6c6c  e terminal, foll
+00000410: 6f77 6564 2062 7920 7468 6520 7061 7468  owed by the path
+00000420: 206f 6620 7468 6520 696d 6167 6520 6669   of the image fi
+00000430: 6c65 2079 6f75 2077 616e 7420 746f 206d  le you want to m
+00000440: 616e 676c 653a 5c6e 5c6e 6060 6062 6173  angle:\n\n```bas
+00000450: 685c 6e69 6d61 6765 6d61 6e67 6c65 7220  h\nimagemangler 
+00000460: 7061 7468 2f74 6f2f 696d 6167 652e 6a70  path/to/image.jp
+00000470: 675c 6e60 6060 5c6e 5c6e 4279 2064 6566  g\n```\n\nBy def
+00000480: 6175 6c74 2c20 496d 6167 6520 4d61 6e67  ault, Image Mang
+00000490: 6c65 7220 7769 6c6c 2061 7574 6f6d 6174  ler will automat
+000004a0: 6963 616c 6c79 206d 616e 676c 6520 7468  ically mangle th
+000004b0: 6520 696d 6167 6520 6163 726f 7373 2061  e image across a
+000004c0: 6c6c 2071 7561 6c69 7479 2073 7465 7073  ll quality steps
+000004d0: 2077 6974 6820 6120 6261 7365 2071 7561   with a base qua
+000004e0: 6c69 7479 206f 6620 3730 2061 6e64 2061  lity of 70 and a
+000004f0: 2071 7561 6c69 7479 2073 7465 7020 6f66   quality step of
+00000500: 2032 2e20 596f 7520 6361 6e20 7370 6563   2. You can spec
+00000510: 6966 7920 796f 7572 206f 776e 2076 616c  ify your own val
+00000520: 7565 7320 666f 7220 7468 6573 6520 7061  ues for these pa
+00000530: 7261 6d65 7465 7273 2075 7369 6e67 2074  rameters using t
+00000540: 6865 206f 7074 696f 6e61 6c20 666c 6167  he optional flag
+00000550: 733a 5c6e 5c6e 5c6e 6060 6062 6173 685c  s:\n\n\n```bash\
+00000560: 6e69 6d61 6765 6d61 6e67 6c65 7220 7061  nimagemangler pa
+00000570: 7468 2f74 6f2f 696d 6167 652e 6a70 6720  th/to/image.jpg 
+00000580: 2d2d 7175 616c 6974 7920 3630 202d 2d71  --quality 60 --q
+00000590: 7561 6c69 7479 2d73 7465 7020 3520 2d2d  uality-step 5 --
+000005a0: 6e6f 2d61 7574 6f2d 6d61 6e67 6c65 5c6e  no-auto-mangle\n
+000005b0: 6060 605c 6e5c 6e46 6f72 2061 206d 6f72  ```\n\nFor a mor
+000005c0: 6520 6465 7461 696c 7320 796f 7520 6361  e details you ca
+000005d0: 6e20 7573 6520 602d 2d68 656c 7060 3a5c  n use `--help`:\
+000005e0: 6e5c 6e60 6060 6261 7368 5c6e 696d 6167  n\n```bash\nimag
+000005f0: 656d 616e 676c 6572 202d 2d68 656c 705c  emangler --help\
+00000600: 6e60 6060 5c6e 272c 0a20 2020 2027 6175  n```\n',.    'au
+00000610: 7468 6f72 273a 2027 6d69 6775 656c 7661  thor': 'miguelva
+00000620: 6c65 6e74 6527 2c0a 2020 2020 2761 7574  lente',.    'aut
+00000630: 686f 725f 656d 6169 6c27 3a20 276d 6967  hor_email': 'mig
+00000640: 7565 6c76 616c 656e 7465 4070 726f 746f  uelvalente@proto
+00000650: 6e6d 6169 6c2e 636f 6d27 2c0a 2020 2020  nmail.com',.    
+00000660: 276d 6169 6e74 6169 6e65 7227 3a20 274e  'maintainer': 'N
+00000670: 6f6e 6527 2c0a 2020 2020 276d 6169 6e74  one',.    'maint
+00000680: 6169 6e65 725f 656d 6169 6c27 3a20 274e  ainer_email': 'N
+00000690: 6f6e 6527 2c0a 2020 2020 2775 726c 273a  one',.    'url':
+000006a0: 2027 4e6f 6e65 272c 0a20 2020 2027 7061   'None',.    'pa
+000006b0: 636b 6167 6573 273a 2070 6163 6b61 6765  ckages': package
+000006c0: 732c 0a20 2020 2027 7061 636b 6167 655f  s,.    'package_
+000006d0: 6461 7461 273a 2070 6163 6b61 6765 5f64  data': package_d
+000006e0: 6174 612c 0a20 2020 2027 696e 7374 616c  ata,.    'instal
+000006f0: 6c5f 7265 7175 6972 6573 273a 2069 6e73  l_requires': ins
+00000700: 7461 6c6c 5f72 6571 7569 7265 732c 0a20  tall_requires,. 
+00000710: 2020 2027 656e 7472 795f 706f 696e 7473     'entry_points
+00000720: 273a 2065 6e74 7279 5f70 6f69 6e74 732c  ': entry_points,
+00000730: 0a20 2020 2027 7079 7468 6f6e 5f72 6571  .    'python_req
+00000740: 7569 7265 7327 3a20 273e 3d33 2e31 302c  uires': '>=3.10,
+00000750: 3c34 2e30 272c 0a7d 0a0a 0a73 6574 7570  <4.0',.}...setup
+00000760: 282a 2a73 6574 7570 5f6b 7761 7267 7329  (**setup_kwargs)
+00000770: 0a                                       .
```

### Comparing `imagemangler-0.1.5/PKG-INFO` & `imagemangler-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 696d 6167  : 2.1.Name: imag
 00000020: 656d 616e 676c 6572 0a56 6572 7369 6f6e  emangler.Version
-00000030: 3a20 302e 312e 350a 5375 6d6d 6172 793a  : 0.1.5.Summary:
+00000030: 3a20 302e 312e 360a 5375 6d6d 6172 793a  : 0.1.6.Summary:
 00000040: 200a 4175 7468 6f72 3a20 6d69 6775 656c   .Author: miguel
 00000050: 7661 6c65 6e74 650a 4175 7468 6f72 2d65  valente.Author-e
 00000060: 6d61 696c 3a20 6d69 6775 656c 7661 6c65  mail: miguelvale
 00000070: 6e74 6540 7072 6f74 6f6e 6d61 696c 2e63  nte@protonmail.c
 00000080: 6f6d 0a52 6571 7569 7265 732d 5079 7468  om.Requires-Pyth
 00000090: 6f6e 3a20 3e3d 332e 3130 2c3c 342e 300a  on: >=3.10,<4.0.
 000000a0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
@@ -26,62 +26,73 @@
 00000190: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
 000001a0: 696c 6c6f 7720 283e 3d39 2e35 2e30 2c3c  illow (>=9.5.0,<
 000001b0: 3130 2e30 2e30 290a 5265 7175 6972 6573  10.0.0).Requires
 000001c0: 2d44 6973 743a 2074 7970 6572 5b61 6c6c  -Dist: typer[all
 000001d0: 5d20 283e 3d30 2e37 2e30 2c3c 302e 382e  ] (>=0.7.0,<0.8.
 000001e0: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
 000001f0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000200: 742f 6d61 726b 646f 776e 0a0a 215b 6c6f  t/markdown..![lo
-00000210: 676f 5d28 6874 7470 733a 2f2f 6769 7468  go](https://gith
-00000220: 7562 2e63 6f6d 2f6d 6967 7565 6c76 616c  ub.com/miguelval
-00000230: 656e 7465 2f69 6d61 6765 6d61 6e67 6c65  ente/imagemangle
-00000240: 722f 626c 6f62 2f6d 6173 7465 722f 6c6f  r/blob/master/lo
-00000250: 676f 2e70 6e67 3f72 6177 3d74 7275 6529  go.png?raw=true)
-00000260: 0a0a 0a49 6d61 6765 204d 616e 676c 6572  ...Image Mangler
-00000270: 2069 7320 6120 636f 6d6d 616e 642d 6c69   is a command-li
-00000280: 6e65 2074 6f6f 6c20 746f 2064 6574 6572  ne tool to deter
-00000290: 696f 7261 7465 2061 6e20 696d 6167 6520  iorate an image 
-000002a0: 6974 6572 6174 6976 656c 7920 7573 696e  iteratively usin
-000002b0: 6720 6c6f 7373 7920 616c 676f 7269 7468  g lossy algorith
-000002c0: 6d73 2e0a 0a23 2049 6e73 7461 6c6c 6174  ms...# Installat
-000002d0: 696f 6e0a 0a59 6f75 2063 616e 2069 6e73  ion..You can ins
-000002e0: 7461 6c6c 2049 6d61 6765 204d 616e 676c  tall Image Mangl
-000002f0: 6572 2076 6961 2070 6970 3a0a 0a60 6060  er via pip:..```
-00000300: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
-00000310: 2069 6d61 6765 6d61 6e67 6c65 720a 6060   imagemangler.``
-00000320: 600a 0a23 2055 7361 6765 0a0a 596f 7520  `..# Usage..You 
-00000330: 6361 6e20 7275 6e20 496d 6167 6520 4d61  can run Image Ma
-00000340: 6e67 6c65 7220 6279 2069 6e76 6f6b 696e  ngler by invokin
-00000350: 6720 7468 6520 696d 6167 656d 616e 676c  g the imagemangl
-00000360: 6572 2063 6f6d 6d61 6e64 2069 6e20 7468  er command in th
-00000370: 6520 7465 726d 696e 616c 2c20 666f 6c6c  e terminal, foll
-00000380: 6f77 6564 2062 7920 7468 6520 7061 7468  owed by the path
-00000390: 206f 6620 7468 6520 696d 6167 6520 6669   of the image fi
-000003a0: 6c65 2079 6f75 2077 616e 7420 746f 206d  le you want to m
-000003b0: 616e 676c 653a 0a0a 6060 6062 6173 680a  angle:..```bash.
-000003c0: 696d 6167 656d 616e 676c 6572 2070 6174  imagemangler pat
-000003d0: 682f 746f 2f69 6d61 6765 2e6a 7067 0a60  h/to/image.jpg.`
-000003e0: 6060 0a0a 4279 2064 6566 6175 6c74 2c20  ``..By default, 
-000003f0: 496d 6167 6520 4d61 6e67 6c65 7220 7769  Image Mangler wi
-00000400: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
-00000410: 206d 616e 676c 6520 7468 6520 696d 6167   mangle the imag
-00000420: 6520 6163 726f 7373 2061 6c6c 2071 7561  e across all qua
-00000430: 6c69 7479 2073 7465 7073 2077 6974 6820  lity steps with 
-00000440: 6120 6261 7365 2071 7561 6c69 7479 206f  a base quality o
-00000450: 6620 3730 2061 6e64 2061 2071 7561 6c69  f 70 and a quali
-00000460: 7479 2073 7465 7020 6f66 2032 2e20 596f  ty step of 2. Yo
-00000470: 7520 6361 6e20 7370 6563 6966 7920 796f  u can specify yo
-00000480: 7572 206f 776e 2076 616c 7565 7320 666f  ur own values fo
-00000490: 7220 7468 6573 6520 7061 7261 6d65 7465  r these paramete
-000004a0: 7273 2075 7369 6e67 2074 6865 206f 7074  rs using the opt
-000004b0: 696f 6e61 6c20 666c 6167 733a 0a0a 0a60  ional flags:...`
-000004c0: 6060 6261 7368 0a69 6d61 6765 6d61 6e67  ``bash.imagemang
-000004d0: 6c65 7220 7061 7468 2f74 6f2f 696d 6167  ler path/to/imag
-000004e0: 652e 6a70 6720 2d2d 7175 616c 6974 7920  e.jpg --quality 
-000004f0: 3630 202d 2d71 7561 6c69 7479 2d73 7465  60 --quality-ste
-00000500: 7020 3520 2d2d 6e6f 2d61 7574 6f2d 6d61  p 5 --no-auto-ma
-00000510: 6e67 6c65 0a60 6060 0a0a 466f 7220 6120  ngle.```..For a 
-00000520: 6d6f 7265 2064 6574 6169 6c73 2079 6f75  more details you
-00000530: 2063 616e 2075 7365 2060 2d2d 6865 6c70   can use `--help
-00000540: 603a 0a0a 6060 6062 6173 680a 696d 6167  `:..```bash.imag
-00000550: 656d 616e 676c 6572 202d 2d68 656c 700a  emangler --help.
-00000560: 6060 600a 0a                             ```..
+00000200: 742f 6d61 726b 646f 776e 0a0a 3c70 2061  t/markdown..<p a
+00000210: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000220: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000230: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6967  //github.com/mig
+00000240: 7565 6c76 616c 656e 7465 2f69 6d61 6765  uelvalente/image
+00000250: 6d61 6e67 6c65 722f 626c 6f62 2f6d 6173  mangler/blob/mas
+00000260: 7465 722f 6c6f 676f 2e70 6e67 3f72 6177  ter/logo.png?raw
+00000270: 3d74 7275 6522 3e3c 696d 6720 7372 633d  =true"><img src=
+00000280: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000290: 636f 6d2f 6d69 6775 656c 7661 6c65 6e74  com/miguelvalent
+000002a0: 652f 696d 6167 656d 616e 676c 6572 2f62  e/imagemangler/b
+000002b0: 6c6f 622f 6d61 7374 6572 2f6c 6f67 6f2e  lob/master/logo.
+000002c0: 706e 673f 7261 773d 7472 7565 2220 616c  png?raw=true" al
+000002d0: 743d 2249 6d61 6765 4d61 6e67 6c65 7222  t="ImageMangler"
+000002e0: 3e3c 2f61 3e0a 3c2f 703e 0a3c 7020 616c  ></a>.</p>.<p al
+000002f0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000300: 2020 3c65 6d3e 496d 6167 6520 4d61 6e67    <em>Image Mang
+00000310: 6c65 7220 6973 2061 2063 6f6d 6d61 6e64  ler is a command
+00000320: 2d6c 696e 6520 746f 6f6c 2074 6f20 6465  -line tool to de
+00000330: 7465 7269 6f72 6174 6520 616e 2069 6d61  teriorate an ima
+00000340: 6765 2069 7465 7261 7469 7665 6c79 2075  ge iteratively u
+00000350: 7369 6e67 206c 6f73 7379 2061 6c67 6f72  sing lossy algor
+00000360: 6974 686d 732e 3c2f 656d 3e0a 3c2f 703e  ithms.</em>.</p>
+00000370: 0a0a 2d2d 2d0a 0a23 2049 6e73 7461 6c6c  ..---..# Install
+00000380: 6174 696f 6e0a 0a59 6f75 2063 616e 2069  ation..You can i
+00000390: 6e73 7461 6c6c 2049 6d61 6765 204d 616e  nstall Image Man
+000003a0: 676c 6572 2076 6961 2070 6970 3a0a 0a60  gler via pip:..`
+000003b0: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+000003c0: 6c6c 2069 6d61 6765 6d61 6e67 6c65 720a  ll imagemangler.
+000003d0: 6060 600a 0a23 2055 7361 6765 0a0a 596f  ```..# Usage..Yo
+000003e0: 7520 6361 6e20 7275 6e20 496d 6167 6520  u can run Image 
+000003f0: 4d61 6e67 6c65 7220 6279 2069 6e76 6f6b  Mangler by invok
+00000400: 696e 6720 7468 6520 696d 6167 656d 616e  ing the imageman
+00000410: 676c 6572 2063 6f6d 6d61 6e64 2069 6e20  gler command in 
+00000420: 7468 6520 7465 726d 696e 616c 2c20 666f  the terminal, fo
+00000430: 6c6c 6f77 6564 2062 7920 7468 6520 7061  llowed by the pa
+00000440: 7468 206f 6620 7468 6520 696d 6167 6520  th of the image 
+00000450: 6669 6c65 2079 6f75 2077 616e 7420 746f  file you want to
+00000460: 206d 616e 676c 653a 0a0a 6060 6062 6173   mangle:..```bas
+00000470: 680a 696d 6167 656d 616e 676c 6572 2070  h.imagemangler p
+00000480: 6174 682f 746f 2f69 6d61 6765 2e6a 7067  ath/to/image.jpg
+00000490: 0a60 6060 0a0a 4279 2064 6566 6175 6c74  .```..By default
+000004a0: 2c20 496d 6167 6520 4d61 6e67 6c65 7220  , Image Mangler 
+000004b0: 7769 6c6c 2061 7574 6f6d 6174 6963 616c  will automatical
+000004c0: 6c79 206d 616e 676c 6520 7468 6520 696d  ly mangle the im
+000004d0: 6167 6520 6163 726f 7373 2061 6c6c 2071  age across all q
+000004e0: 7561 6c69 7479 2073 7465 7073 2077 6974  uality steps wit
+000004f0: 6820 6120 6261 7365 2071 7561 6c69 7479  h a base quality
+00000500: 206f 6620 3730 2061 6e64 2061 2071 7561   of 70 and a qua
+00000510: 6c69 7479 2073 7465 7020 6f66 2032 2e20  lity step of 2. 
+00000520: 596f 7520 6361 6e20 7370 6563 6966 7920  You can specify 
+00000530: 796f 7572 206f 776e 2076 616c 7565 7320  your own values 
+00000540: 666f 7220 7468 6573 6520 7061 7261 6d65  for these parame
+00000550: 7465 7273 2075 7369 6e67 2074 6865 206f  ters using the o
+00000560: 7074 696f 6e61 6c20 666c 6167 733a 0a0a  ptional flags:..
+00000570: 0a60 6060 6261 7368 0a69 6d61 6765 6d61  .```bash.imagema
+00000580: 6e67 6c65 7220 7061 7468 2f74 6f2f 696d  ngler path/to/im
+00000590: 6167 652e 6a70 6720 2d2d 7175 616c 6974  age.jpg --qualit
+000005a0: 7920 3630 202d 2d71 7561 6c69 7479 2d73  y 60 --quality-s
+000005b0: 7465 7020 3520 2d2d 6e6f 2d61 7574 6f2d  tep 5 --no-auto-
+000005c0: 6d61 6e67 6c65 0a60 6060 0a0a 466f 7220  mangle.```..For 
+000005d0: 6120 6d6f 7265 2064 6574 6169 6c73 2079  a more details y
+000005e0: 6f75 2063 616e 2075 7365 2060 2d2d 6865  ou can use `--he
+000005f0: 6c70 603a 0a0a 6060 6062 6173 680a 696d  lp`:..```bash.im
+00000600: 6167 656d 616e 676c 6572 202d 2d68 656c  agemangler --hel
+00000610: 700a 6060 600a 0a                        p.```..
```

