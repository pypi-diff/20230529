# Comparing `tmp/airfrans-0.1.3.tar.gz` & `tmp/airfrans-0.1.4.tar.gz`

## Comparing `airfrans-0.1.3.tar` & `airfrans-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 airfrans-0.1.3/.readthedocs.yaml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 airfrans-0.1.3/airfrans.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/make.bat
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/requirements.txt
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/conf.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/index.rst
--rw-r--r--   0        0        0   119172 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/_figures/boundary_layer.png
--rw-r--r--   0        0        0  2300738 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/_figures/fields.png
--rw-r--r--   0        0        0  2317524 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/_figures/sampling.png
--rw-r--r--   0        0        0    71716 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/_figures/surface.png
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/modules/dataset.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/modules/naca.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/modules/root.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/modules/sampling.rst
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/notes/dataset.rst
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/notes/installation.rst
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/notes/introduction.rst
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/notes/simulation.rst
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 airfrans-0.1.3/docs/source/notes/visualization.rst
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 airfrans-0.1.3/src/airfrans/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 airfrans-0.1.3/src/airfrans/dataset.py
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 airfrans-0.1.3/src/airfrans/naca_generator.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 airfrans-0.1.3/src/airfrans/reorganize.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 airfrans-0.1.3/src/airfrans/sampling.py
--rw-r--r--   0        0        0    22460 2020-02-02 00:00:00.000000 airfrans-0.1.3/src/airfrans/simulation.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 airfrans-0.1.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 airfrans-0.1.3/LICENSE
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 airfrans-0.1.3/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 airfrans-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 airfrans-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 airfrans-0.1.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 airfrans-0.1.4/airfrans.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/requirements.txt
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/conf.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/index.rst
+-rw-r--r--   0        0        0   119172 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/boundary_layer.png
+-rw-r--r--   0        0        0  2300738 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/fields.png
+-rw-r--r--   0        0        0  2317524 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/sampling.png
+-rw-r--r--   0        0        0    71716 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/surface.png
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/dataset.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/naca.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/root.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/sampling.rst
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/dataset.rst
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/installation.rst
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/introduction.rst
+-rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/simulation.rst
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/visualization.rst
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/__init__.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/dataset.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/naca_generator.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/reorganize.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/sampling.py
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/simulation.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 airfrans-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 airfrans-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 airfrans-0.1.4/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 airfrans-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 airfrans-0.1.4/PKG-INFO
```

### Comparing `airfrans-0.1.3/.readthedocs.yaml` & `airfrans-0.1.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/Makefile` & `airfrans-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/make.bat` & `airfrans-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/source/conf.py` & `airfrans-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/source/index.rst` & `airfrans-0.1.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/source/_figures/boundary_layer.png` & `airfrans-0.1.4/docs/source/_figures/boundary_layer.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/source/_figures/fields.png` & `airfrans-0.1.4/docs/source/_figures/fields.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/source/_figures/sampling.png` & `airfrans-0.1.4/docs/source/_figures/sampling.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/source/_figures/surface.png` & `airfrans-0.1.4/docs/source/_figures/surface.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/docs/source/notes/introduction.rst` & `airfrans-0.1.4/docs/source/notes/introduction.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Introduction
 ============
 
-The AirfRANS dataset is a collection of numerical simulations solving the incompressible Reynolds-Averaged Navier-Stokes equations over two dimensional airfoils in a subsonic flight regime. The associated `paper <https://openreview.net/forum?id=Zp8YmiQ_bDC>`_ has been accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks. In addition to this library two GitHub repositories have been proposed to reconduct the paper `experiments <https://github.com/Extrality/AirfRANS>`_ and to generate new `compressible or incompressible simulations over NACA airfoils <https://github.com/Extrality/NACA_simulation>`_. The setup to generate those simulations have been confronted to the Langley Research Center experiments available in the `Turbulence Modeling Resource <https://turbmodels.larc.nasa.gov/>`_ for the NACA 0012 and 4412.
+The AirfRANS dataset is a collection of numerical simulations solving the incompressible Reynolds-Averaged Navier-Stokes equations over two dimensional airfoils in a subsonic flight regime. The associated `paper https://arxiv.org/abs/2212.07564`_ has been accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks. In addition to this library two GitHub repositories have been proposed to reconduct the paper `experiments <https://github.com/Extrality/AirfRANS>`_ and to generate new `compressible or incompressible simulations over NACA airfoils <https://github.com/Extrality/NACA_simulation>`_. The setup to generate those simulations have been confronted to the Langley Research Center experiments available in the `Turbulence Modeling Resource <https://turbmodels.larc.nasa.gov/>`_ for the NACA 0012 and 4412.
 
 This dataset has been built to lower the potential barrier between Machine Learning and Physics research communities. It proposes data on a simple but realistic case which already includes some of the major challenges of Machine Learning for solving Fluid Dynamics, namely:
 
 - working with unstructured data coming from raw numerical simulations,
 - being able to deal with the number of nodes required in simulation meshes (from hundreds of thousands to hundreds of million in 3D cases),
 - treating cases with a realistic Reynolds number,
 - regressing the entire velocity, pressure and turbulent viscosity fields from a geometry and the boundary conditions,
```

### Comparing `airfrans-0.1.3/docs/source/notes/simulation.rst` & `airfrans-0.1.4/docs/source/notes/simulation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. note::
+	
+	Since version ``0.1.4``, the normals in the ``airfrans.Simulation`` class are inward-pointing instead ouf outward-pointing previsouly. This for consistency with the normals given in the AirfRANS dataset.
+
 Simulation
 ==========
 
 Each simulation is defined via boundary conditions (inlet velocity and angle of attack) and a geometry (NACA 4 or 5 digits). We recall that in an incompressible setup and when neglecting gravity, the only parameter of Navier-Stokes equations (and also of RANS equations) is the Reynolds number. If we fix the kinematic viscosity (`i.e.` if we fix the temperature of air one for all), the Reynolds number is completely defined by the inlet velocity (as the characteristic length of airfoil is chosen to be 1 meter). In this dataset, we chose to arbitrarily fix the temperature to 298.15K and to work with properties of air at that temperature, at a pressure of 1013.25 hPa.
 
 You can run new simulation with the help of `OpenFOAM v2112 <https://www.openfoam.com/>`_ and the `NACA simulation GitHub <https://github.com/Extrality/NACA_simulation>`_.
 
@@ -15,14 +19,18 @@
 
 .. code-block:: python
 
 	import airfrans as af
 	
 	simulation = af.Simulation(root = PATH_TO_DATASET, name = 'airFoil2D_SST_43.597_5.932_3.551_3.1_1.0_18.252', T = 298.15)
 
+.. note::
+
+	The name of a simulation gives all the information about the boundary conditions used to generate it. For example, in ``'airFoil2D_SST_43.597_5.932_3.551_3.1_1.0_18.252'``, we read that the inlet velocity magnitude is :math:`43.597 m\cdot s^{-1}`, and the angle of attack :math:`5.932^{\circ}`. The last numbers are for the parameters of the NACA arifoil, if we have 3 parameters it means that we are dealing with an airfoil from the 4-digits series, and if we have 4 parameters then this airfoil comes from the 5-digits series (this is due to the fact that the last two digits gives the thickness of the airfoil which only defines a single parameter). To keep with our example, we here deal with an airfoil of the 5-digits series with parameters given by ``(3.551, 3.1, 1.0, 18.252)`` (which are real numbers and not integers). Another example, the NACA 0012 will lead to parameters ``(0, 0, 12)`` and a name ending by ``0_0_12``.
+
 Attributes
 ----------
 
 One part of the attributes of the class is the properties of air at the given temperature:
 
 - :obj:`airfrans.Simulation.MOL` is the molar weigth of air in :math:`kg\cdot mol^{-1}`
 - :obj:`airfrans.Simulation.P_ref` is the reference pressure in :math:`Pa`
@@ -43,16 +51,16 @@
 Finally, the last part is the fields associated with the simulation under the form of NumPy ndarray. Those fields are either defined on the mesh nodes, are the airfoil patch nodes directly:
 
 - :obj:`airfrans.Simulation.input_velocity` is the inlet velocity copied on each nodes of the internal mesh in :math:`m\cdot s^{-1}`
 - :obj:`airfrans.Simulation.sdf` is the distance function on the internal mesh in :math:`m`
 - :obj:`airfrans.Simulation.surface` is a boolean on the internal mesh, it is ``True`` if the node lie on the airfoil
 - :obj:`airfrans.Simulation.position` is the position of the nodes of the internal mesh in :math:`m`
 - :obj:`airfrans.Simulation.airfoil_position` is the position of the nodes of the airfoil mesh in :math:`m`
-- :obj:`airfrans.Simulation.normals` is the outpointing normals of the surface on the internal mesh, it is set to 0 for points not lying on the airfoil
-- :obj:`airfrans.Simulation.airfoil_normals` is the outpointing normais of the surface on the airfoil mesh
+- :obj:`airfrans.Simulation.normals` is the inward-pointing normals of the surface on the internal mesh, it is set to 0 for points not lying on the airfoil
+- :obj:`airfrans.Simulation.airfoil_normals` is the inward-pointing normais of the surface on the airfoil mesh
 
 and for the targets:
 
 - :obj:`airfrans.Simulation.velocity` is the air velocity on the internal mesh in :math:`m\cdot s^{-1}`
 - :obj:`airfrans.Simulation.pressure` is the air pressure on the internal mesh (divided by the specific mass in the incompressible case)
 - :obj:`airfrans.Simulation.nu_t` is the kinematic turbulent viscosity on the internal mesh in :math:`m^2\cdot s^{-2}`
```

### Comparing `airfrans-0.1.3/docs/source/notes/visualization.rst` & `airfrans-0.1.4/docs/source/notes/visualization.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/src/airfrans/dataset.py` & `airfrans-0.1.4/src/airfrans/dataset.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/src/airfrans/naca_generator.py` & `airfrans-0.1.4/src/airfrans/naca_generator.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/src/airfrans/reorganize.py` & `airfrans-0.1.4/src/airfrans/reorganize.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/src/airfrans/sampling.py` & `airfrans-0.1.4/src/airfrans/sampling.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/src/airfrans/simulation.py` & `airfrans-0.1.4/src/airfrans/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         # Input candidates
         self.surface = np.array((self.internal.point_data['U'][:, 0] == 0))
         self.sdf = -np.array(self.internal.point_data['implicit_distance'][:, None]).astype('float64')
         self.input_velocity = (np.array([np.cos(self.angle_of_attack), np.sin(self.angle_of_attack)])*self.inlet_velocity).reshape(1, 2)*np.ones_like(self.sdf)
         
         self.position = np.array(self.internal.points[:, :2]).astype('float64')
         self.airfoil_position = np.array(self.airfoil.points[:, :2]).astype('float64')
-        self.airfoil_normals = np.array(-self.airfoil.point_data['Normals'][:, :2]).astype('float64')
+        self.airfoil_normals = np.array(self.airfoil.point_data['Normals'][:, :2]).astype('float64')
 
         self.normals = np.zeros_like(self.input_velocity).astype('float64')
         self.normals[self.surface] = reorganize(
             self.airfoil_position,
             self.position[self.surface], 
             self.airfoil_normals
             )
@@ -105,15 +105,15 @@
             sampled_line_indices = np.random.choice(self.airfoil.n_cells, size = n, replace = True, p = p)
         elif density == 'mesh_density': # Sample via mesh density
             sampled_line_indices = np.random.choice(self.airfoil.n_cells, size = n, replace = True)
 
         line_dict = np.array(self.airfoil.lines).reshape(-1, 3)[sampled_line_indices, 1:]
         line_points = np.array(self.airfoil.points)[line_dict]
 
-        normal = np.array(-self.airfoil.point_data['Normals'][line_dict, :2]) 
+        normal = np.array(self.airfoil.point_data['Normals'][line_dict, :2]) 
 
         if targets:
             line_attr = np.concatenate([
                 normal, 
                 np.array(self.airfoil.point_data['U'][line_dict, :2]), 
                 np.array(self.airfoil.point_data['p'][line_dict, None]), 
                 np.array(self.airfoil.point_data['nut'][line_dict, None])
@@ -170,15 +170,15 @@
             internal.point_data['U'] = np.concatenate([self.velocity, np.zeros_like(self.sdf)], axis = -1)
         jacobian = np.array(internal.compute_derivative(scalars = 'U', gradient = 'jacobian').point_data['jacobian'].reshape(-1, 3, 3)[self.surface, :2, :2]).astype('float64')
 
         s = .5*(jacobian + jacobian.transpose(0, 2, 1))
         s = s - s.trace(axis1 = -2, axis2 = -1).reshape(-1, 1, 1)*np.eye(2)[None]/3
 
         wss_ = 2*self.NU.reshape(-1, 1, 1)*s
-        wss_ = (wss_*self.normals[self.surface, :2].reshape(-1, 1, 2)).sum(axis = 2)
+        wss_ = -(wss_*self.normals[self.surface, :2].reshape(-1, 1, 2)).sum(axis = 2)
 
         if over_airfoil:
             wss = reorganize(self.position[self.surface], self.airfoil_position, wss_)
         else:
             wss = np.zeros_like(self.velocity).astype('float64')
             wss[self.surface] = wss_
 
@@ -219,25 +219,25 @@
         else:
             force_p = np.array(-wp_int)*self.RHO
             force_v = np.array(wss_int)*self.RHO
         force = force_p + force_v
 
         return force, force_p, force_v
 
-    def force_coefficient(self, reference = False):
+    def force_coefficient(self, compressible = False, reference = False):
         """
         Compute the force coefficients for the simulation. The output is a tuple of the form `((cd, cdp, cdv), (cl, clp, clv))`,
         where `cd` is the drag coefficient, `cdp` the pressure contribution of the drag coefficient and `cdv` the viscous
         contribution of the drag coefficient. Same for the lift coefficient `cl`.
 
         Args:
             reference (bool, optional): If ``True``, return the force coefficients computed with the reference fields.
                 If ``False``, compute the force coefficients with the fields attribute of the class. Default: ``False``   
         """
-        f, fp, fv = self.force(reference = reference)
+        f, fp, fv = self.force(compressible = compressible, reference = reference)
 
         basis = np.array([[np.cos(self.angle_of_attack), np.sin(self.angle_of_attack)], [-np.sin(self.angle_of_attack), np.cos(self.angle_of_attack)]])
         fp_rot, fv_rot = np.matmul(basis, fp), np.matmul(basis, fv)
         cp, cv = fp_rot/(.5*self.RHO*self.inlet_velocity**2), fv_rot/(.5*self.RHO*self.inlet_velocity**2)
         cdp, cdv = cp[0], cv[0]
         clp, clv = cp[1], cv[1]
         cd, cl = cdp + cdv, clp + clv
@@ -330,18 +330,18 @@
 
         if x < 1:
             digits = np.array(list(map(float, self.name.split('_')[4:-1]))).astype('float64')
             camber = camber_line(digits, self.airfoil_position[:, 0])[0]
             idx_extrado = self.airfoil_position[:, 1] > camber
 
             if extrado:
-                arg = np.argmin(np.abs(self.airfoil_position[idx_extrado, 0] - x))
+                arg = np.argmin(np.abs(self.airfoil_position[idx_extrado, 0] - x)) + 1
                 arg = np.argwhere(idx_extrado.cumsum(axis = 0) == arg)[0][0]
             else:
-                arg = np.argmin(np.abs(self.airfoil_position[~idx_extrado, 0] - x))
+                arg = np.argmin(np.abs(self.airfoil_position[~idx_extrado, 0] - x)) + 1
                 arg = np.argwhere((~idx_extrado).cumsum(axis = 0) == arg)[0][0]
 
             if direction == 'normals':
                 normals = np.concatenate([self.airfoil_normals[arg], np.zeros(1)])
             
             elif direction == 'vertical':
                 normals = np.array([0, 2*int(extrado) - 1, 0]).astype('float64')
```

### Comparing `airfrans-0.1.3/.gitignore` & `airfrans-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/LICENSE` & `airfrans-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/README.md` & `airfrans-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.3/pyproject.toml` & `airfrans-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "airfrans"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Florent Bonnet", email="bonnet@isir.upmc.fr" },
 ]
 description = "A package to facilitate the manipulation of the AirfRANS dataset simulations."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airfrans-0.1.3/PKG-INFO` & `airfrans-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airfrans
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to facilitate the manipulation of the AirfRANS dataset simulations.
 Project-URL: Homepage, https://github.com/Extrality/airfrans_lib
 Project-URL: Bug Tracker, https://github.com/Extrality/airfrans_lib/issues
 Author-email: Florent Bonnet <bonnet@isir.upmc.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

