# Comparing `tmp/rescupybs-0.0.1.3.2-py3-none-any.whl.zip` & `tmp/rescupybs-0.0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8382 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx       31 b- defN 23-Mar-31 04:02 rescupybs/__init__.py
--rwxrwxrwx  2.0 unx     8230 b- defN 23-Apr-04 03:16 rescupybs/functions.py
+Zip file size: 9010 bytes, number of entries: 10
+-rwxrwxrwx  2.0 unx       29 b- defN 23-Apr-15 16:23 rescupybs/__init__.py
+-rwxrwxrwx  2.0 unx     8451 b- defN 23-Apr-15 22:42 rescupybs/functions.py
 -rwxrwxrwx  2.0 unx     6786 b- defN 23-Mar-31 04:58 rescupybs/plots.py
--rwxrwxrwx  2.0 unx    10461 b- defN 23-Mar-30 05:33 rescupybs/wrapper.py
--rwxrwxrwx  2.0 unx     1060 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     1858 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       53 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      825 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/RECORD
-10 files, 29406 bytes uncompressed, 6968 bytes compressed:  76.3%
+-rwxrwxrwx  2.0 unx    12318 b- defN 23-Apr-15 22:01 rescupybs/wrapper.py
+-rwxrwxrwx  2.0 unx     1060 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx     2963 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       88 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/RECORD
+10 files, 32610 bytes uncompressed, 7620 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: rescupybs/plots.py
 Comment: 
 
 Filename: rescupybs/wrapper.py
 Comment: 
 
-Filename: rescupybs-0.0.1.3.2.dist-info/LICENSE
+Filename: rescupybs-0.0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: rescupybs-0.0.1.3.2.dist-info/METADATA
+Filename: rescupybs-0.0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: rescupybs-0.0.1.3.2.dist-info/WHEEL
+Filename: rescupybs-0.0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: rescupybs-0.0.1.3.2.dist-info/entry_points.txt
+Filename: rescupybs-0.0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.3.2.dist-info/top_level.txt
+Filename: rescupybs-0.0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.3.2.dist-info/RECORD
+Filename: rescupybs-0.0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rescupybs/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.0.1.3.2"
+__version__ = "0.0.1.4"
```

## rescupybs/functions.py

```diff
@@ -2,14 +2,16 @@
 import h5py, re, pint, os
 from rescupy.totalenergy import TotalEnergy
 from ase import Atoms as ats
 from ase.io import read, write
 
 ureg = pint.UnitRegistry(system="atomic")
 
+# rescubs
+
 def exchange(array_a,array_b):
     l=len(array_a)
     m=np.arange(l)
     for i in range(2,l):
         fun1=np.polyfit(m[i-2:i], array_a[i-2:i], 1)
         fun2=np.polyfit(m[i-2:i], array_b[i-2:i], 1)
         p1=np.poly1d(fun1)
@@ -72,17 +74,18 @@
             eigenvalues = calc.energy.eigenvalues.T - calc.energy.efermi
             ispin = calc.system.hamiltonian.ispin
             formula = calc.system.atoms.formula
         else:
             chpts = chpts + [i + chpts[-1] + 1 for i in calc.system.kpoint.special_points]
             labels = labels + calc.system.kpoint.get_special_points_labels()
             eigenvalues = np.concatenate((eigenvalues, calc.energy.eigenvalues.T - calc.energy.efermi), axis=1)
-    filename = os.path.commonprefix(input)
-    if filename[-1] == '_':
-        filename = filename[:-1]
+    filename = os.path.commonprefix([os.path.split(i)[-1] for i in input]).rsplit('.',1)[0]
+    if not filename:
+        filename = 'nano_bs_out'
+    filename = filename.strip('_')
     for i in range(0, len(chpts)-1):
         if chpts[i] + 1 == chpts[i+1] and labels[i] == labels[i+1]:
             j = chpts[i]
             eigenvalues = np.delete(eigenvalues, j, axis=1)
             del chpts[i]
             del labels[i]
             for k in range(i, len(chpts)):
@@ -145,40 +148,46 @@
 def get_vbm_cbm(eigenvalues_s):
     max = np.max(eigenvalues_s[eigenvalues_s < 0.0])
     min = np.min(eigenvalues_s[eigenvalues_s > 0.0])
     i, vb = np.where(eigenvalues_s==max)
     i, cb = np.where(eigenvalues_s==min)
     return vb[0], max, cb[0], min
 
-def isosurfaces_wf(input, kpt, band, spin):
-    calc = TotalEnergy.read(input)
-    output = input.rsplit('.', 1)[0]+'_'+str(kpt)+'_'+str(band)+'_'+str(spin)+'.vasp'
-    pbc = [1, 1, 1]
-    positions = calc.system.atoms.positions
-    cell = calc.system.cell.avec
-    elements_symbols = calc.system.atoms.get_labels()
-    stp = ats(elements_symbols,positions=positions,cell=cell,pbc=pbc)
-    grid = calc.system.cell.grid
-    write(output, stp, direct=True, vasp5=True)
+# rescuiso
+
+def isosurfaces_wf(input, output, kpt, band, spin):
+    if not output:
+        output = input+'_'+str(kpt)+'_'+str(band)+'_'+str(spin)+'.vasp'
     if calc.system.hamiltonian.ispin == 1:
         att = f"wavefunctions/{kpt + 1}/field"
     else:
         if spin == 1:
             att = f"wavefunctions/spin-up/{kpt + 1}/field"
         else:
             att = f"wavefunctions/spin-down/{kpt + 1}/field"
-    filename = input.rsplit('.', 1)[0]+'.h5'
+    filename = input+'.h5'
     h = h5py.File(filename, mode="r")
     fld = h[att][0:]
     fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
     fld = np.asfortranarray(fld)
     fld = fld / ureg.bohr**1.5
     fld = fld[::2, :] + 1j * fld[1::2, :]
     fld.ito("angstrom ** -1.5")
-    fld = fld[..., band].magnitude
+    if band < fld.shape[-1]:
+        fld = fld[..., band].magnitude
+    else:
+        raise Exception("The band is out of range in *.h5 file.")
     f_abs = np.abs(fld)
     f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
     f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
+    calc = TotalEnergy.read(input+'.json')
+    pbc = [1, 1, 1]
+    positions = calc.system.atoms.positions
+    cell = calc.system.cell.avec
+    elements_symbols = calc.system.atoms.get_labels()
+    stp = ats(elements_symbols,positions=positions,cell=cell,pbc=pbc)
+    grid = calc.system.cell.grid
+    write(output, stp, direct=True, vasp5=True)
     with open(output, "a") as f:
         f.writelines(['\n']+[str(i)+' ' for i in grid]+['\n'])
         np.savetxt(f, f_div)
```

## rescupybs/wrapper.py

```diff
@@ -7,40 +7,37 @@
 
 plt.rcParams['xtick.direction'] = 'in'
 plt.rcParams['ytick.direction'] = 'in'
 plt.rcParams['ytick.minor.visible'] = True
 plt.rcParams["mathtext.fontset"] = 'cm'
 
 def main():
-    parser = argparse.ArgumentParser(description='Plot the band structure from rescuplus calculation result *.json file',
+    parser = argparse.ArgumentParser(description='Plot the band structure from rescuplus calculation result *.json or *.dat file.',
                                      epilog='''
 Example:
-rescupybs -y -0.5 0.5 -b
+rescubs -y -0.5 0.5 -b
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",      version="rescupybs "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
     parser.add_argument('-s', "--size",       type=float, nargs=2,   help='figure size: width, height')
     parser.add_argument('-b', "--divided",    action='store_true',   help="plot the up and down spin in divided subplot")
     parser.add_argument('-y', "--vertical",   type=float, nargs=2,   help="vertical axis")
-    parser.add_argument('-g', "--legend",     type=str,  nargs=1,    help="legend labels")
+    parser.add_argument('-g', "--legend",     type=str,   nargs=1,   help="legend labels")
     parser.add_argument('-a', "--location",   type=str.lower,        default='best',
                                                                      choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                      help="arrange the legend location, default best")
     parser.add_argument('-k', "--linestyle",  type=str, nargs='+',   default=['-'],
                                                                      help="linestyle: solid, dashed, dashdot, dotted or tuple; default solid")
-    parser.add_argument('-W', "--linewidth",  type=str, nargs='+',   default=['0.8'], help="linewidth, default 0.8")
+    parser.add_argument('-w', "--linewidth",  type=str, nargs='+',   default=['0.8'], help="linewidth, default 0.8")
     parser.add_argument('-c', "--color",      type=str,              nargs='+', default=[],
                                                                      help="plot colors: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
     parser.add_argument('-m', "--modify",     type=int, nargs=2,     help='modify the bands overlap, the up or nonispin bands to exchange values')
     parser.add_argument('-n', "--nbands",     type=int, nargs=2,     help='the down bands to exchange values')
     parser.add_argument('-i', "--input",      type=str,              nargs='+', default=[], help="plot figure from .json or .dat file")
     parser.add_argument('-o', "--output",     type=str,              default="BAND.png", help="plot figure filename")
-    parser.add_argument('-K', "--kpt",        type=int,              default=0, help="The kpoint in wavefunctions")
-    parser.add_argument('-B', "--band",       type=int,              default=0, help="The band in wavefunctions")
-    parser.add_argument('-S', "--spin",       type=int,              default=1, help="The up or down spin in wavefunctions")
     parser.add_argument('-l', "--labels",     type=str.upper,        nargs='+', default=[], help='labels for high-symmetry points')
     parser.add_argument('-f', "--font",       type=str,              default='STIXGeneral', help="font to use")
 
     args = parser.parse_args()
 
     labels_f = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     linestyle = []
@@ -78,19 +75,21 @@
     pltname = os.path.split(os.getcwd())[-1]
     if not args.input:
         input = ['nano_bs_out.json']
         if not os.path.exists(input[0]):
             raise Exception("The input file does not exist.")
     else:
         input = [f for i in args.input for f in glob.glob(i)]
+        input = [os.path.join(i,'nano_bs_out.json') if os.path.isdir(i) else i for i in input]
+        input = [i for i in input if os.path.exists(i)]
         if not input:
             raise Exception("The input file does not exist.")
 
     if len(input) == 1:
-        if input[0].rsplit('.', 1)[-1].lower() == 'json':
+        if input[0].lower().endswith('.json'):
             if 'bs' in input[0].split('_'):
                 bs_file = input[0]
                 eigenvalues, chpts, labels = functions.bs_json_read(bs_file)
                 if labels_f:
                     labels = labels_f
                 legend = args.legend
                 if not legend:
@@ -101,18 +100,16 @@
                     labels = labels[:len(chpts)]
                 if len(eigenvalues) == 1:
                     plots.Nispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
                 elif len(eigenvalues) == 2 and not args.divided:
                     plots.Ispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
                 elif len(eigenvalues) == 2 and args.divided:
                     plots.Dispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
-            elif 'wvf' in input[0].split('_'):
-                functions.isosurfaces_wf(input[0], args.kpt, args.band, args.spin)
 
-        elif input[0].rsplit('.', 1)[-1].lower() == 'dat':
+        elif input[0].lower().endswith('.dat'):
             eigenvalues = functions.bs_dat_read(input)
             chpts, labels, vbm_cbm = functions.labels_read("LABELS")
             if labels_f:
                 labels = labels_f
             legend = args.legend
             if not legend:
                 legend = [pltname]
@@ -172,8 +169,43 @@
                 elif len(eigenvalues) == 2 and not args.divided:
                     plots.Ispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
                 elif len(eigenvalues) == 2 and args.divided:
                     plots.Dispin(args.output, args.size, vertical, eigenvalues, chpts, labels, linestyle, linewidth, legend, args.location, color)
         else:
             raise Exception("The input files mismatch.")
 
+def surface():
+    parser = argparse.ArgumentParser(description='Export the wavefunction isosurface for VESTA from rescuplus calculation result *.json and *.h5 files.',
+                                     epilog='''
+Example:
+rescuiso -b 1 -k 0
+''',
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser.add_argument('-v', "--version", action="version", version="rescupybs "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
+    parser.add_argument('-i', "--input",   type=str,         nargs='+', default=[], help="export the wavefunction isosurface from .json and .h5 files")
+    parser.add_argument('-o', "--output",  type=str,         help="wavefunction isosurface for VESTA format")
+    parser.add_argument('-k', "--kpt",     type=int,         default=0, help="The kpoint in wavefunctions")
+    parser.add_argument('-b', "--band",    type=int,         default=0, help="The band in wavefunctions")
+    parser.add_argument('-s', "--spin",    type=int,         default=1, help="The up or down spin in wavefunctions")
+
+    args = parser.parse_args()
+
+    if not args.input:
+        input = ['nano_wvf_out']
+        if not os.path.exists(input[0]+'.json') and not os.path.exists(input[0]+'.h5'):
+            raise Exception("The input file does not exist.")
+    else:
+        input = [f.rsplit('_in',1)[0]+'_out.json' if f.rsplit('.',1)[0].endswith('in') else f for i in args.input for f in glob.glob(i)]
+        input = [os.path.join(i,'nano_wvf_out.json') if os.path.isdir(i) else i for i in input]
+        input = [i.rsplit('.',1)[0] for i in input]
+        input = [i for i in input if os.path.exists(i+'.json') and os.path.exists(i+'.h5')]
+        if not input:
+            raise Exception("The input file does not exist.")
+
+    if len(input) == 1:
+        if 'wvf' in input[0].split('_'):
+            functions.isosurfaces_wf(input[0], args.output, args.kpt, args.band, args.spin)
+    else:
+        if all('wvf' in f.split('_') for f in input):
+            for i in range(len(input)):
+                functions.isosurfaces_wf(input[i], args.output, args.kpt, args.band, args.spin)
```

## Comparing `rescupybs-0.0.1.3.2.dist-info/LICENSE` & `rescupybs-0.0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rescupybs-0.0.1.3.2.dist-info/RECORD` & `rescupybs-0.0.1.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-rescupybs/__init__.py,sha256=cTmFF1WqPMbeqRNUHztB-QeJOqsFzpIP7dbrWJwHEPE,31
-rescupybs/functions.py,sha256=70LXS_a3LjzIfxYNgFokskikZOIIdm_FIPsyr0rJIfk,8230
+rescupybs/__init__.py,sha256=EwUBrbjqfFSu5mrlRfgjbaVl39_D-q5WlKKDhiOSkRI,29
+rescupybs/functions.py,sha256=Ume1P3SYVE2iOuK5Tq4taN8PEDgRldr8NSMnr11RNVI,8451
 rescupybs/plots.py,sha256=5_7__zep7lgbxNqw-UZ_Nm2h4uSbtjCbeqB9g3FHLoM,6786
-rescupybs/wrapper.py,sha256=275oEos1nyUX-A9PgTXw6ruOmXELpaF7w-qSEKOzweE,10461
-rescupybs-0.0.1.3.2.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
-rescupybs-0.0.1.3.2.dist-info/METADATA,sha256=tY37RnJLnI7GdMvebMgT1wnrNqp2zNcxCz8UqHU4TvE,1858
-rescupybs-0.0.1.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rescupybs-0.0.1.3.2.dist-info/entry_points.txt,sha256=DUGWHtRnZ-6RuS6H2KaXmmQzv_teO2Ddmrq5Nq20e3g,53
-rescupybs-0.0.1.3.2.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
-rescupybs-0.0.1.3.2.dist-info/RECORD,,
+rescupybs/wrapper.py,sha256=znQ51PrhuD9I7_gd35m8eAIxZ3hdgzMFAckAC4W2kdE,12318
+rescupybs-0.0.1.4.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
+rescupybs-0.0.1.4.dist-info/METADATA,sha256=OAE3ReboQQG2B5UDDlGsx2OIheb1Y4KieFSgJwPmHwY,2963
+rescupybs-0.0.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+rescupybs-0.0.1.4.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
+rescupybs-0.0.1.4.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
+rescupybs-0.0.1.4.dist-info/RECORD,,
```

