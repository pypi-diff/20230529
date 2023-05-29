# Comparing `tmp/rescupybs-0.1.1-py3-none-any.whl.zip` & `tmp/rescupybs-0.1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,11 @@
-Zip file size: 9526 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       27 b- defN 23-May-03 05:02 rescupybs/__init__.py
--rw-rw-r--  2.0 unx    13813 b- defN 23-May-03 05:02 rescupybs/functions.py
--rw-rw-r--  2.0 unx     7061 b- defN 23-May-03 05:02 rescupybs/plots.py
--rw-rw-r--  2.0 unx    11652 b- defN 23-May-03 05:02 rescupybs/wrapper.py
--rwxrwxr-x  2.0 unx     1060 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2961 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       88 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      802 b- defN 23-May-03 05:02 rescupybs-0.1.1.dist-info/RECORD
-10 files, 37566 bytes uncompressed, 8160 bytes compressed:  78.3%
+Zip file size: 9697 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       29 b- defN 23-May-29 02:30 rescupybs/__init__.py
+-rw-rw-r--  2.0 unx    16032 b- defN 23-May-29 02:30 rescupybs/functions.py
+-rw-rw-r--  2.0 unx     7674 b- defN 23-May-29 02:30 rescupybs/plots.py
+-rw-rw-r--  2.0 unx    13777 b- defN 23-May-29 02:30 rescupybs/wrapper.py
+-rw-rw-r--  2.0 unx     3044 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       88 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      722 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/RECORD
+9 files, 41468 bytes uncompressed, 8453 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -6,26 +6,23 @@
 
 Filename: rescupybs/plots.py
 Comment: 
 
 Filename: rescupybs/wrapper.py
 Comment: 
 
-Filename: rescupybs-0.1.1.dist-info/LICENSE
+Filename: rescupybs-0.1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: rescupybs-0.1.1.dist-info/METADATA
+Filename: rescupybs-0.1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rescupybs-0.1.1.dist-info/WHEEL
+Filename: rescupybs-0.1.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rescupybs-0.1.1.dist-info/entry_points.txt
+Filename: rescupybs-0.1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rescupybs-0.1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: rescupybs-0.1.1.dist-info/RECORD
+Filename: rescupybs-0.1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rescupybs/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.1"
+__version__ = "0.1.1.1"
```

## rescupybs/functions.py

```diff
@@ -148,14 +148,43 @@
 def get_vbm_cbm(eigenvalues_s):
     max = np.max(eigenvalues_s[eigenvalues_s < 0.0])
     min = np.min(eigenvalues_s[eigenvalues_s > 0.0])
     i, vb = np.where(eigenvalues_s==max)
     i, cb = np.where(eigenvalues_s==min)
     return vb[0], max, cb[0], min
 
+def dos(filename):
+    from rescupy import DensityOfStates as DOS
+    from rescupy.jsonio import json_read
+    calc = DOS.from_totalenergy(filename)
+    calc.set_units('atomic')
+    cal  = json_read(filename)
+    calc.dos.dos = np.array([cal['dos']['dos']]).T
+    calc.dos.energy = np.array(cal['dos']['energy'])
+    calc.dos.efermi = cal['dos']['efermi']
+    if cal['dos']['pdos_return']:
+        calc.dos.orbA = cal['dos']['orbA']
+        calc.dos.orbL = cal['dos']['orbL']
+        calc.dos.orbM = cal['dos']['orbM']
+        h5name = filename.rsplit('.json')[0] + '.h5'
+        h = h5py.File(h5name, mode="r")
+        fld = h['dos']['pdos']['total'][0:]
+        fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
+        calc.dos.pdos = fld
+        calc.dos.pdos_return = cal['dos']['pdos_return']
+    calc.set_units('si')
+    return calc
+
+def tdos(dosfiles):
+    calc = dos(dosfiles)
+    arr = calc.dos.energy
+    efe = calc.dos.efermi
+    ele = calc.dos.dos
+    return arr - efe, ele
+
 # rescuiso
 
 def isosurfaces_wf(input, output, kpt, band, spin):
     calc = TotalEnergy.read(input+'.json')
     kpt_l = len(kpt)
     band_l = len(band)
     if kpt_l == 1 and band_l == 1:
@@ -311,7 +340,37 @@
     grid = calc.system.cell.grid
     print("Saving data to disk ...")
     write(output, stp, direct=True, vasp5=True)
     with open(output, "a") as f:
         f.writelines(['\n']+[str(i)+' ' for i in grid]+['\n'])
         np.savetxt(f, f_div)
 
+def isosurfaces_dos(input, output):
+    calc = TotalEnergy.read(input+'.json')
+    if not output:
+        output = input+'.vasp'
+    att = f"density/total"
+    print("Reading *.h5 file ...")
+    filename = input+'.h5'
+    h = h5py.File(filename, mode="r")
+    print("Processing data ...")
+    fld = h[att][0:]
+    fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
+    fld = np.asfortranarray(fld)
+    fld = fld / ureg.bohr**3
+    fld.ito("angstrom ** -3")
+    fld = fld.magnitude
+    f_abs = np.abs(fld)
+    f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
+    f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
+    print("Reading structure ...")
+    pbc = [1, 1, 1]
+    positions = calc.system.atoms.positions
+    cell = calc.system.cell.avec
+    elements_symbols = calc.system.atoms.get_labels()
+    stp = ats(elements_symbols,positions=positions,cell=cell,pbc=pbc)
+    grid = calc.system.cell.grid
+    print("Saving data to disk ...")
+    write(output, stp, direct=True, vasp5=True)
+    with open(output, "a") as f:
+        f.writelines(['\n']+[str(i)+' ' for i in grid]+['\n'])
+        np.savetxt(f, f_div)
```

## rescupybs/plots.py

```diff
@@ -131,7 +131,24 @@
     if len(chpts) > 2:
         for i in chpts[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
+
+def tdos(arr, ele, fig_p):
+    plt.figure(figsize=fig_p.size)
+    plt.minorticks_on()
+    plt.tick_params(axis='both', which='minor', color='gray')
+    plt.plot(arr, ele)
+    plt.xlim(fig_p.vertical)
+    plt.ylim(fig_p.horizontal)
+    plt.xlabel('Energy (eV)')
+    plt.ylabel('Density of states, electrons/eV')
+    plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
+    plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
+#    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
+    
+    
+
```

## rescupybs/wrapper.py

```diff
@@ -21,80 +21,96 @@
 def main():
     parser = argparse.ArgumentParser(description='Plot the band structure from rescuplus calculation result *.json or *.dat file.',
                                      epilog='''
 Example:
 rescubs -y -0.5 0.5 -b
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument('-v', "--version",    action="version",      version="rescupybs "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
-    parser.add_argument('-s', "--size",       type=float, nargs=2,   help='figure size: width, height')
-    parser.add_argument('-b', "--divided",    action='store_true',   help="plot the up and down spin in divided subplot")
-    parser.add_argument('-y', "--vertical",   type=float, nargs=2,   help="vertical axis")
-    parser.add_argument('-g', "--legend",     type=str,   nargs=1,   help="legend labels")
-    parser.add_argument('-a', "--location",   type=str.lower,        default='best',
-                                                                     choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
-                                                                     help="arrange the legend location, default best")
-    parser.add_argument('-k', "--linestyle",  type=str, nargs='+',   default=[],
-                                                                     help="linestyle: solid, dashed, dashdot, dotted or tuple; default solid")
-    parser.add_argument('-w', "--linewidth",  type=str, nargs='+',   default=[], help="linewidth, default 0.8")
-    parser.add_argument('-c', "--color",      type=str,              nargs='+', default=[],
-                                                                     help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow; k, black; w, white")
-    parser.add_argument('-m', "--modify",     type=int, nargs=2,     help='modify the bands overlap, the up or nonispin bands to exchange values')
-    parser.add_argument('-n', "--nbands",     type=int, nargs=2,     help='the down bands to exchange values')
-    parser.add_argument('-i', "--input",      type=str,              nargs='+', default=[], help="plot figure from .json or .dat file")
-    parser.add_argument('-o', "--output",     type=str,              default="BAND.png", help="filename of the figure, default: BAND.png")
-    parser.add_argument('-q', "--dpi",        type=int,              default=500, help="dpi of the figure, default: 500")
-    parser.add_argument('-l', "--labels",     type=str.upper,        nargs='+', default=[], help='labels for high-symmetry points')
-    parser.add_argument('-f', "--font",       type=str,              default='STIXGeneral', help="font to use")
+    parser.add_argument('-v', "--version",    action="version",     version="rescupybs "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
+    parser.add_argument('-s', "--size",       type=float, nargs=2,  help='figure size: width, height')
+    parser.add_argument('-b', "--divided",    action='store_true',  help="plot the up and down spin in divided subplot")
+    parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="vertical axis")
+    parser.add_argument('-g', "--legend",     type=str,   nargs=1,  help="legend labels")
+    parser.add_argument('-L', "--location",   type=str.lower,       default='best',
+                                                                    choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center'],
+                                                                    help="arrange the legend location, default best")
+    parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
+                                                                                    "k, black; w, white", default=[])
+    parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
+                                                                                    default=[])
+    parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
+    parser.add_argument('-m', "--modify",     type=int, nargs=2,    help='modify the bands overlap, the up or nonispin bands to exchange values')
+    parser.add_argument('-n', "--nbands",     type=int, nargs=2,    help='the down bands to exchange values')
+    parser.add_argument('-i', "--input",      type=str,             nargs='+', default=[], help="plot figure from .json or .dat file")
+    parser.add_argument('-o', "--output",     type=str,             default="BAND.png", help="filename of the figure, default: BAND.png")
+    parser.add_argument('-q', "--dpi",        type=int,             default=500, help="dpi of the figure, default: 500")
+    parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points')
+    parser.add_argument('-d', "--dos",        type=str,             nargs='?', default='', help="plot DOS from .json file, default: nano_dos_out.json")
+    parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
+    parser.add_argument('-a', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
+    parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d')
+    parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
+    parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot')
+    parser.add_argument('-z', "--fill",       type=float,           nargs='*', help='fill a shaded region between PDOS and axis, default: 0.2', default=None)
+    parser.add_argument('-f', "--font",       type=str,             default='STIXGeneral', help="font to use")
 
     args = parser.parse_args()
 
     labels_f = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
-    linestyle = []
-    for i in args.linestyle:
-        if len(i) > 2 and i[0] == '(' and i[-1] == ')':
-            linestyle.append(eval(i))
-        elif len(i.split('*')) == 2:
-            j = i.split('*')
-            linestyle = linestyle + [j[0]] * int(j[1])
-        else:
-            linestyle.append(i)
-
-    linewidth = []
-    for i in args.linewidth:
-        if len(i.split('*')) == 2:
-            j = i.split('*')
-            linewidth = linewidth + [float(j[0])] * int(j[1])
-        else:
-            linewidth.append(float(i))
+    elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
+    if args.dos != '':
+        dosfiles = args.dos or 'nano_dos_out.json'
+        if dosfiles.rsplit('.',1)[0].endswith('_in'):
+            dosfiles = dosfiles.rsplit('_in',1)[0]+'_out.json'
+        if os.path.isdir(dosfiles):
+            dosfiles = os.path.join(dosfiles, 'nano_dos_out.json')
+        dosfiles = dosfiles if os.path.exists(dosfiles) else None
+    else:
+        dosfiles = None
 
     color = []
     for i in args.color:
         j = i.split('*')
         if len(j) == 2:
-            color = color + [j[0]] * int(j[1])
+            color += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
         else:
-            color.append(i)
+            color += [ast.literal_eval(i)] if '(' in i and ')' in i else [i]
 
-    vertical = args.vertical or [-5.0, 5.0]
+    linestyle = []
+    for i in args.linestyle:
+        j = i.split('*')
+        if len(j) == 2:
+            linestyle += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
+        else:
+            linestyle += [ast.literal_eval(i)] if '(' in i and ')' in i else [i]
+
+    linewidth = []
+    for i in args.linewidth:
+        j = i.split('*')
+        linewidth += [float(j[0])] * int(j[1]) if len(j) == 2 else [float(i)]
 
     plt.rcParams['font.family'] = '%s'%args.font
 
     pltname = os.path.split(os.getcwd())[-1]
 
     input = args.input or ['nano_bs_out.json']
     input = [f for i in input for f in glob.glob(i)]
     input = [os.path.join(i,'nano_bs_out.json') if os.path.isdir(i) else i for i in input]
     input = [i for i in input if os.path.exists(i)]
-    if not input:
-        raise Exception("The input file does not exist.")
 
-    fig_p = cla_fig(output=args.output, size=args.size, vertical=vertical,
-                    linestyle=linestyle, linewidth=linewidth, location=args.location, color=color, dpi=args.dpi)
-    if len(input) == 1:
+    width_ratios = args.wratios or (0.3 if args.divided else 0.5)
+
+    fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi)
+
+    len_bandfile = len(input)
+# plot Band Structure
+    if len_bandfile == 1:
+        if not fig_p.vertical:
+            fig_p.vertical = [-5.0, 5.0]
         if input[0].lower().endswith('.json'):
             if 'bs' in input[0].split('_'):
                 bs_file = input[0]
                 eigenvalues, chpts, labels = functions.bs_json_read(bs_file)
                 if labels_f:
                     labels = labels_f
                 legend = args.legend or [pltname]
@@ -123,15 +139,17 @@
                 if args.modify[0] != args.modify[1]:
                     functions.exchange(eigenvalues[0,:,args.modify[0]], eigenvalues[0,:,args.modify[1]])
                     np.savetxt(input[0], eigenvalues[0])
                 plots.Mnispin(eigenvalues, chpts, labels, vbm_cbm, fig_p)
             else:
                 plots.Nispin(eigenvalues, chpts, labels, legend, fig_p)
 
-    else:
+    elif len_bandfile == 2:
+        if not fig_p.vertical:
+            fig_p.vertical = [-5.0, 5.0]
         Extension = [f.rsplit('.', 1)[-1].lower() for f in input]
         if all(x == Extension[0] for x in Extension):
             if len(input) == 2 and Extension[0] == 'dat':
                 eigenvalues = functions.bs_dat_read(input)
                 chpts, labels, vbm_cbm = functions.labels_read("LABELS")
                 if labels_f:
                     labels = labels_f
@@ -166,14 +184,25 @@
                     plots.Nispin(eigenvalues, chpts, labels, legend, fig_p)
                 elif len(eigenvalues) == 2 and not args.divided:
                     plots.Ispin(eigenvalues, chpts, labels, legend, fig_p)
                 elif len(eigenvalues) == 2 and args.divided:
                     plots.Dispin(eigenvalues, chpts, labels, legend, fig_p)
         else:
             raise Exception("The input files mismatch.")
+# plot DOS
+    elif len_bandfile == 0:
+        if dosfiles:
+            if fig_p.output == "BAND.png":
+                fig_p.output = "DOS.png"
+            arr, ele = functions.tdos(dosfiles)
+            plots.tdos(arr, ele, fig_p)
+        else:
+            print("ERROR: No *dos_out.json file.")
+    else:
+        print("Input file mismatch.")
 
 def surface():
     parser = argparse.ArgumentParser(description='Export the wavefunction isosurface for VESTA from rescuplus calculation result *.json and *.h5 files.',
                                      epilog='''
 Example:
 rescuiso -b 1 -k 0
 ''',
@@ -197,12 +226,14 @@
     input = [i for i in input if os.path.exists(i+'.json') and os.path.exists(i+'.h5')]
     if not input:
         raise Exception("The input file does not exist.")
 
     if len(input) == 1:
         if 'wvf' in input[0].split('_'):
             functions.isosurfaces_wf(input[0], args.output, args.kpt, args.band, args.spin)
+        elif 'dos' in input[0].split('_'):
+            functions.isosurfaces_dos(input[0], args.output)
     else:
         if all('wvf' in f.split('_') for f in input):
             for i in range(len(input)):
                 functions.isosurfaces_wf(input[i], args.output, args.kpt, args.band, args.spin)
```

## Comparing `rescupybs-0.1.1.dist-info/METADATA` & `rescupybs-0.1.1.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: rescupybs
-Version: 0.1.1
-Summary: Band structure plot from rescuplus json file.
+Version: 0.1.1.1
+Summary: Band structure plot and wavefunction export from rescuplus *.json and *.h5 file.
 Home-page: https://github.com/lkccrr/rescupybs
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
-Keywords: DFT rescuplus band plot
+Keywords: DFT rescuplus band plot wavefunction
 Platform: Unix
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: numpy (<1.24,>=1.22.0)
 Requires-Dist: matplotlib (>=3.4.0)
 Requires-Dist: pint (>=0.10)
 Requires-Dist: rescupy (>=1.0.0)
 
 [![rescupybs](https://img.shields.io/pypi/v/rescupybs?style=flat-square)](https://pypi.org/project/rescupybs/)
 [![rescupybs](https://img.shields.io/pypi/pyversions/rescupybs?style=flat-square)](https://pypi.org/project/rescupybs/)
@@ -47,10 +47,10 @@
 ```
 ***
 <b style="color:blue;"><i>rescuiso</b></i>
 * To execute <b style="color:blue;"><i>rescuiso</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 rescuiso -h
-rescuiso -i nano_wvf_out.json -k 2 -b 2
+rescuiso -i nano_wvf_out.json -k 1 4 -b 0 3
 ```
```

## Comparing `rescupybs-0.1.1.dist-info/RECORD` & `rescupybs-0.1.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-rescupybs/__init__.py,sha256=GThDTBxUYSx7Tbtuwxo2HyiVDw6EMvBnKJkJof2YsWQ,27
-rescupybs/functions.py,sha256=ywVvQ8WkiNb156SG4pUV1aGDQkYQlgBIFKWAkPgbNJw,13813
-rescupybs/plots.py,sha256=Ql2VasG6SzXOgKRE43ROwiu15P8sPQHDukKwG1fuyUA,7061
-rescupybs/wrapper.py,sha256=mgGPiJKWW9U9Akvr-LV5-IFWf2fEopfO9d0IgxK7WSA,11652
-rescupybs-0.1.1.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
-rescupybs-0.1.1.dist-info/METADATA,sha256=L8iuuO6fZYDCNkIz6XtdjZyV0ygyackkBZn71WHveu8,2961
-rescupybs-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rescupybs-0.1.1.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
-rescupybs-0.1.1.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
-rescupybs-0.1.1.dist-info/RECORD,,
+rescupybs/__init__.py,sha256=L8ZZeqV3ZossHfeL37DRT_aUNvdxySXK8tzaxVkJAIg,29
+rescupybs/functions.py,sha256=LOArp6CRkUeb2Ed8auX-Ko8_HrMiWPS0Cqd_iJLidXI,16032
+rescupybs/plots.py,sha256=Slev0FrsUu0NY25qw0CJ_E4fY4oOmCgOUVkKDgSTnSM,7674
+rescupybs/wrapper.py,sha256=Ppabz1R-gw8xTgDUEDhX7u5xBTGP--5fv51YJSwvzEk,13777
+rescupybs-0.1.1.1.dist-info/METADATA,sha256=aveYvCzPgLEcs34dh2R8LLWKzIYmB55FwL38Zp6_h48,3044
+rescupybs-0.1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+rescupybs-0.1.1.1.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
+rescupybs-0.1.1.1.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
+rescupybs-0.1.1.1.dist-info/RECORD,,
```

