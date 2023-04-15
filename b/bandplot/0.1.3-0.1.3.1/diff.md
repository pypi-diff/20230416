# Comparing `tmp/bandplot-0.1.3-py3-none-any.whl.zip` & `tmp/bandplot-0.1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,11 @@
-Zip file size: 10040 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx       24 b- defN 23-Mar-10 00:14 bandplot/__init__.py
+Zip file size: 9274 bytes, number of entries: 9
+-rwxrwxrwx  2.0 unx       26 b- defN 23-Mar-30 18:56 bandplot/__init__.py
 -rwxrwxrwx  2.0 unx    27604 b- defN 23-Mar-05 05:05 bandplot/plots.py
 -rwxrwxrwx  2.0 unx     5809 b- defN 23-Mar-10 00:34 bandplot/readdata.py
--rwxrwxrwx  2.0 unx    15274 b- defN 23-Mar-10 00:48 bandplot/wrapper.py
--rwxrwxrwx  2.0 unx     1060 b- defN 23-Mar-10 00:48 bandplot-0.1.3.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     2854 b- defN 23-Mar-10 00:48 bandplot-0.1.3.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Mar-10 00:48 bandplot-0.1.3.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       87 b- defN 23-Mar-10 00:48 bandplot-0.1.3.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx        9 b- defN 23-Mar-10 00:48 bandplot-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      790 b- defN 23-Mar-10 00:48 bandplot-0.1.3.dist-info/RECORD
-10 files, 53603 bytes uncompressed, 8696 bytes compressed:  83.8%
+-rwxrwxrwx  2.0 unx    15274 b- defN 23-Apr-15 22:51 bandplot/wrapper.py
+-rwxrwxrwx  2.0 unx     2901 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       86 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx        9 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      711 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/RECORD
+9 files, 52512 bytes uncompressed, 8050 bytes compressed:  84.7%
```

## zipnote {}

```diff
@@ -6,26 +6,23 @@
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.3.dist-info/LICENSE
+Filename: bandplot-0.1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.3.dist-info/METADATA
+Filename: bandplot-0.1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.3.dist-info/WHEEL
+Filename: bandplot-0.1.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.3.dist-info/entry_points.txt
+Filename: bandplot-0.1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.3.dist-info/top_level.txt
-Comment: 
-
-Filename: bandplot-0.1.3.dist-info/RECORD
+Filename: bandplot-0.1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.3"
+__version__ = "0.1.3.1"
```

## bandplot/wrapper.py

```diff
@@ -8,41 +8,41 @@
 plt.rcParams['ytick.minor.visible'] = True
 plt.rcParams["mathtext.fontset"] = 'cm'
 
 def main():
     parser = argparse.ArgumentParser(description='Plot the band structure or DOS from vaspkit result.',
                                      epilog='''
 Example:
-bandplot -i band.dat -o pband.png -l g m k g -d PDOS* -F
+bandplot -i band.dat -o pband.png -l g m k g -d PDOS* -z
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
     parser.add_argument('-s', "--size",       type=int, nargs=2)
     parser.add_argument('-b', "--divided",    action='store_true',  help="plot the up and down spin in divided subplot")
     parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="energy (eV) range")
     parser.add_argument('-g', "--legend",     type=str, nargs=1,    help="legend labels")
     parser.add_argument('-a', "--location",   type=str.lower,       default='best',
                                                                     choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                     help="arrange the legend location, default best")
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', default=['-'],
                                                                     help="linestyle: solid, dashed, dashdot, dotted or tuple; default solid")
-    parser.add_argument('-W', "--linewidth",  type=str,             nargs='+', default=['0.8'], help="linewidth, default 0.8")
+    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', default=['0.8'], help="linewidth, default 0.8")
     parser.add_argument('-c', "--color",      type=str,             nargs='+', default=[],
                                                                     help="plot colors: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
     parser.add_argument('-i', "--input",      type=str,             default="BAND.dat", help="plot figure from .dat file, default BAND.dat")
     parser.add_argument('-o', "--output",     type=str,             default="BAND.png", help="plot figure filename, default BAND.png")
-    parser.add_argument('-K', "--klabels",    type=str,             default="KLABELS",  help="the filename of KLABELS")
+    parser.add_argument('-j', "--klabels",    type=str,             default="KLABELS",  help="the filename of KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
     parser.add_argument('-x', "--horizontal", type=float,           nargs=2, help="Density of states, electrons/eV range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
     parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
-    parser.add_argument('-w', "--wratios",    type=float,           help='width ratio for DOS subplot')
-    parser.add_argument('-F', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
+    parser.add_argument('-r', "--wratios",    type=float,           help='width ratio for DOS subplot')
+    parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
     parser.add_argument('-f', "--font",       type=str,             default='STIXGeneral', help="font to use")
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
     dosfiles = [f for i in args.dos for f in glob.glob(i)]
@@ -164,26 +164,26 @@
     parser.add_argument('-y', "--vertical",   type=float,           nargs=2, help="frequency (THz) range")
     parser.add_argument('-g', "--legend",     type=str,             nargs=1, help="legend labels")
     parser.add_argument('-a', "--location",   type=str.lower,       default='best',
                                                                     choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                     help="arrange the legend location, default best")
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', default=['-'],
                                                                     help="linestyle: solid, dashed, dashdot, dotted or tuple; default solid")
-    parser.add_argument('-W', "--linewidth",  type=str,             nargs='+', default=['0.8'], help="linewidth, default 0.8")
+    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', default=['0.8'], help="linewidth, default 0.8")
     parser.add_argument('-c', "--color",      type=str,             nargs='+', default=[],
                                                                     help="plot colors: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
     parser.add_argument('-i', "--input",      type=str,             default="BAND.dat", help="plot figure from .dat file, default BAND.dat")
     parser.add_argument('-o', "--output",     type=str,             default="BAND.png", help="plot figure filename, default BAND.png")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
     parser.add_argument('-x', "--horizontal", type=float,           nargs=2, help="Phonon density of states range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
-    parser.add_argument('-w', "--wratios",    type=float,           default=0.5, help='width ratio for DOS subplot, default 0.5')
-    parser.add_argument('-F', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
+    parser.add_argument('-r', "--wratios",    type=float,           default=0.5, help='width ratio for DOS subplot, default 0.5')
+    parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
     parser.add_argument('-f', "--font",       type=str,             default='STIXGeneral', help="font to use")
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
     linestyle = []
```

## Comparing `bandplot-0.1.3.dist-info/METADATA` & `bandplot-0.1.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
@@ -17,42 +17,40 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: matplotlib (>=3.4.0)
 Requires-Dist: numpy (>=1.22.0)
+Requires-Dist: matplotlib (>=3.4.0)
 
 [![bandplot](https://img.shields.io/pypi/v/bandplot?style=flat-square)](https://pypi.org/project/bandplot/)
 [![bandplot](https://img.shields.io/pypi/pyversions/bandplot?style=flat-square)](https://pypi.org/project/bandplot/)
 [![bandplot](https://img.shields.io/pypi/l/bandplot?style=flat-square)](https://pypi.org/project/bandplot/)
 [![bandplot](https://img.shields.io/pypi/dm/bandplot?style=flat-square)](https://pypi.org/project/bandplot/)
 [![bandplot](https://img.shields.io/pypi/wheel/bandplot?style=flat-square)](https://pypi.org/project/bandplot/)
 [![bandplot](https://img.shields.io/github/last-commit/lkccrr/bandplot?style=flat-square)](https://github.com/lkccrr/bandplot)
 [![bandplot](https://img.shields.io/github/release-date/lkccrr/bandplot?style=flat-square)](https://github.com/lkccrr/bandplot)
 
 ### bandplot
 
-Bandplot is used for plotting the band structure, DOS or phonon band structure plot from ***vaspkit*** or ***phonopy*** results. The code will provide two scripts, <b style="color:blue;"><i>bandplot</b></i> for band structure or DOS plotting from ***vaspkit*** <b style="color:darkred;"><i>\*.dat</b></i> files, and <b style="color:blue;"><i>pbandplot</b></i> for phonon band structure or DOS plotting from ***phonopy*** <b style="color:darkred;"><i>\*.dat</b></i> files.
+The <b style="color:green;"><i>bandplot</b></i> is used for electron band structure, DOS or phonon band structure, DOS plotting from ***vaspkit*** or ***phonopy*** results. The code will provide two scripts, <b style="color:blue;"><i>bandplot</b></i> for band structure or DOS plotting from ***vaspkit*** <b style="color:darkred;"><i>\*.dat</b></i> files, and <b style="color:blue;"><i>pbandplot</b></i> for phonon band structure or DOS plotting from ***phonopy*** <b style="color:darkred;"><i>\*.dat</b></i> files.
 ***
 <b style="color:blue;"><i>bandplot</b></i>
 * To execute <b style="color:blue;"><i>bandplot</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 bandplot -h
-bandplot -i band.dat -o band.png -l g m k g -d PDOS* -F
-bandplot -b -l g m k g -y -5 2
+bandplot -i band.dat -o band.png -l g m k g -d PDOS* -z
+bandplot -b -l g m k g -y -3 3
 ```
 ***
 <b style="color:blue;"><i>pbandplot</b></i>
 * To execute <b style="color:blue;"><i>pbandplot</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 pbandplot -h
-pbandplot -i band.dat -o pband.png -l g m k g -d projected_dos.dat
+pbandplot -i band.dat -o pband.png -l g m k g -d projected_dos.dat -z
 pbandplot -b 23 100 -l g m k g -y -2 110
 ```
 
-
-
```

