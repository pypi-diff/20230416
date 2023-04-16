# Comparing `tmp/pycapacity-1.2.8.tar.gz` & `tmp/pycapacity-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycapacity-1.2.8.tar", last modified: Thu Mar 24 16:19:54 2022, max compression
+gzip compressed data, was "dist/pycapacity-1.2.9.tar", last modified: Fri May 13 14:44:54 2022, max compression
```

## Comparing `pycapacity-1.2.8.tar` & `pycapacity-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-03-24 16:19:54.000000 pycapacity-1.2.8/
--rw-rw-r--   0 antun     (1000) antun     (1000)     1126 2022-03-24 16:15:24.000000 pycapacity-1.2.8/setup.py
--rw-rw-r--   0 antun     (1000) antun     (1000)     1069 2021-08-06 12:07:42.000000 pycapacity-1.2.8/LICENSE
--rw-rw-r--   0 antun     (1000) antun     (1000)    18958 2022-03-24 16:19:54.000000 pycapacity-1.2.8/PKG-INFO
--rw-rw-r--   0 antun     (1000) antun     (1000)       38 2022-03-24 16:19:54.000000 pycapacity-1.2.8/setup.cfg
-drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-03-24 16:19:54.000000 pycapacity-1.2.8/pycapacity/
--rw-rw-r--   0 antun     (1000) antun     (1000)    18477 2022-03-24 16:19:14.000000 pycapacity-1.2.8/pycapacity/algorithms.py
--rw-rw-r--   0 antun     (1000) antun     (1000)     6934 2022-02-15 12:26:31.000000 pycapacity-1.2.8/pycapacity/human.py
--rwxrwxr-x   0 antun     (1000) antun     (1000)    13379 2022-03-24 15:38:23.000000 pycapacity-1.2.8/pycapacity/robot.py
--rw-rw-r--   0 antun     (1000) antun     (1000)        0 2021-10-27 15:41:22.000000 pycapacity-1.2.8/pycapacity/__init__.py
--rw-rw-r--   0 antun     (1000) antun     (1000)     7912 2021-12-08 11:36:30.000000 pycapacity-1.2.8/pycapacity/visual.py
--rw-rw-r--   0 antun     (1000) antun     (1000)    16247 2021-12-07 12:52:25.000000 pycapacity-1.2.8/README.md
-drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-03-24 16:19:54.000000 pycapacity-1.2.8/pycapacity.egg-info/
--rw-rw-r--   0 antun     (1000) antun     (1000)    18958 2022-03-24 16:19:53.000000 pycapacity-1.2.8/pycapacity.egg-info/PKG-INFO
--rw-rw-r--   0 antun     (1000) antun     (1000)       11 2022-03-24 16:19:53.000000 pycapacity-1.2.8/pycapacity.egg-info/top_level.txt
--rw-rw-r--   0 antun     (1000) antun     (1000)       37 2022-03-24 16:19:53.000000 pycapacity-1.2.8/pycapacity.egg-info/requires.txt
--rw-rw-r--   0 antun     (1000) antun     (1000)        1 2022-03-24 16:19:53.000000 pycapacity-1.2.8/pycapacity.egg-info/dependency_links.txt
--rw-rw-r--   0 antun     (1000) antun     (1000)      304 2022-03-24 16:19:53.000000 pycapacity-1.2.8/pycapacity.egg-info/SOURCES.txt
+drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-05-13 14:44:54.000000 pycapacity-1.2.9/
+-rwxr-xr-x   0 antun     (1000) antun     (1000)     1069 2021-08-06 14:07:42.000000 pycapacity-1.2.9/LICENSE
+-rwxr-xr-x   0 antun     (1000) antun     (1000)    16247 2021-12-07 14:52:25.000000 pycapacity-1.2.9/README.md
+drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity/
+-rwxr-xr-x   0 antun     (1000) antun     (1000)    13379 2022-03-24 17:38:23.000000 pycapacity-1.2.9/pycapacity/robot.py
+-rwxr-xr-x   0 antun     (1000) antun     (1000)    10074 2022-04-04 15:06:52.000000 pycapacity-1.2.9/pycapacity/visual.py
+-rwxr-xr-x   0 antun     (1000) antun     (1000)    19233 2022-05-13 14:40:04.000000 pycapacity-1.2.9/pycapacity/algorithms.py
+-rwxr-xr-x   0 antun     (1000) antun     (1000)     7983 2022-04-12 15:12:45.000000 pycapacity-1.2.9/pycapacity/human.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)      102 2022-04-12 14:47:05.000000 pycapacity-1.2.9/pycapacity/polytope.py
+-rwxr-xr-x   0 antun     (1000) antun     (1000)        0 2021-10-27 17:41:22.000000 pycapacity-1.2.9/pycapacity/__init__.py
+-rw-rw-r--   0 antun     (1000) antun     (1000)    16937 2022-05-13 14:44:54.000000 pycapacity-1.2.9/PKG-INFO
+-rwxr-xr-x   0 antun     (1000) antun     (1000)     1028 2022-05-13 14:44:04.000000 pycapacity-1.2.9/setup.py
+drwxrwxr-x   0 antun     (1000) antun     (1000)        0 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/
+-rw-rw-r--   0 antun     (1000) antun     (1000)      327 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/SOURCES.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)       11 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/top_level.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)        1 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/dependency_links.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)    16937 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/PKG-INFO
+-rw-rw-r--   0 antun     (1000) antun     (1000)       44 2022-05-13 14:44:54.000000 pycapacity-1.2.9/pycapacity.egg-info/requires.txt
+-rw-rw-r--   0 antun     (1000) antun     (1000)       38 2022-05-13 14:44:54.000000 pycapacity-1.2.9/setup.cfg
```

### Comparing `pycapacity-1.2.8/setup.py` & `pycapacity-1.2.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pycapacity',
-    version='1.2.8',
+    version='1.2.9',
     author='Antun Skuric',
     author_email='antun.skuric@inria.fr',
     description='A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models',
     long_description=long_description, #'A Real-time capable robot capacity calculation module', 
     long_description_content_type="text/markdown",
     url='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity',
     license='MIT',
-    #package_dir = {'pycapacity': 'pycapacity'}, 
     packages = ['pycapacity'],
-    #py_modules=['pycapacity.robot','pycapacity.human'],
-    install_requires=['numpy','scipy','cvxopt>=1.2.6','matplotlib'],
+    install_requires=['numpy','scipy','cvxopt>=1.2.6','matplotlib','plotly'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Framework :: Robot Framework",
         "Framework :: Robot Framework :: Library",
         "Framework :: Robot Framework :: Tool"
```

### Comparing `pycapacity-1.2.8/LICENSE` & `pycapacity-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycapacity-1.2.8/PKG-INFO` & `pycapacity-1.2.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,271 +1,255 @@
-Metadata-Version: 2.1
-Name: pycapacity
-Version: 1.2.8
-Summary: A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models
-Home-page: https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity
-Author: Antun Skuric
-Author-email: antun.skuric@inria.fr
-License: MIT
-Description: 
-        # Real-time capable task-space capacity calculation python module
-        
-        <img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
-        <img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
-        
-        The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
-        - Robotic serial manipulators - `pycapacity.robot`
-        - Human musculoskeletal models - `pycapacity.human`
-        
-        This package also provides a module `pycapacity.algorithms` with a set of polytope evaluation algorithms for standard polytope formulations, that can be used as a standalone library.
-        
-        Additionally, `pycapacity.visual` module provides a set of visualisaiton tools using the `matplotlib` for visualising 2d and 3d polytopes.
-        
-        See [full API documentation and docs.](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
-        
-        ## Robotic manipulator capacity metrics
-        <img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/robot.png' height='300px'>
-        
-        For the robotic manipulators the package integrates several velocity, force and acceleration capacity calculation functions based on ellipsoids:
-        - Velocity (manipulability) ellipsoid <br> `E_vel = {dx | dx = J.dq, ||dq||<1 }`
-        - Acceleration (dynamic manipulability) ellipsoid <br> `E_acc = {ddx | ddx = J.M^(-1).t, ||t||<1 }`
-        - Force ellipsoid <br> `E_for = {f | J^T.f = t, ||t||<1 }`
-        
-        And polytopes: 
-        - Velocity polytope <br> `P_vel = {dx | dx = J.dq,  dq_min < dq < dq_max}`
-        - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).t, t_min < t < t_max}`
-        - Force polytope <br> `P_for = {f | J^T.f = t, t_min < t < t_max}`
-        - Force polytopes *Minkowski sum and intersection*
-        
-        Where `J` is the robot jacobian matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities and `t` is the vector of joint torques.
-        
-        The force polytope functions have been implemented according to the paper:<br>
-        [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
-        by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
-        
-        And the velocity and acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
-        [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
-        by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
-        
-        ## Human musculoskeletal models capacity metrics
-        <img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/force.png' height='200px'>
-        
-        For the human musculoskeletal models this package implements the polytope metrics:
-        - Velocity polytope <br> `P_vel = {dx | dx = J.dq, dl = L.dq  dl_min < dl < dl_max}`
-        - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).N.F, F_min < F < F_max}`
-        - Force polytope <br> `P_for = {f | J^T.f = N.F, F_min < F < F_max}`
-        
-        Where `J` is the model's jacobian matrix, `L` si the muscle length jacobian matrix, `N= -L^T` is the moment arm matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities, `t` is the vector of joint torques, `dl` is the vector of the muscle stretching velocities and `F` is the vector of muscular forces. 
-        
-        The force and velocity polytope functions have been implemented according to the paper:<br>
-        [**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
-        by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
-        
-        And the acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
-        [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
-        by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
-        
-        ## Polytope evaluation algorithms
-        
-        There are three methods implemented in this paper to resolve all the polytope calculations:
-        - Hyper-plane shifting method
-        - Iterative convex hull method
-        - Vertex enumeration auctus
-        
-        All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md). 
-        
-        ### Hyper-plane shifting method
-        [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
-        by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
-        
-        This method finds the half-space representation of the polytope of a class:
-        ```
-        P = {x | x = By, y_min <= y <= y_max }
-        ```
-        To find the vertices of the polytope after finding the half-space representation `Hx <= d` an convex-hull algorithm is used. 
-        
-        The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-hyper_plane_shift_method). 
-        
-        ### Iterative convex-hull method
-        [**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
-        by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
-        
-        This method finds both vertex and half-space representation of the class of polytopes:
-        ```
-        P = {x | Ax = By, y_min <= y <= y_max }
-        ``` 
-        And it can be additionally extended to the case where there is an additional projection matrix `P` making a class of problems:
-        ```
-        P = {x | x= Pz, Az = By, y_min <= y <= y_max }
-        ``` 
-        
-        The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-iterative_convex_hull_method)
-        
-        ### Vertex enumeration auctus
-        [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
-        by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
-        
-        This method finds vertex representation of the class of polytopes:
-        ```
-        P = {x | Ax = y, y_min <= y <= y_max }
-        ``` 
-        To find the half-space representation (faces) of the polytope after finding the vertex representation  an convex-hull algorithm is used. 
-        
-        The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-vertex_enumeration_auctus)
-        
-        ## Installation
-        
-        All you need to do to install it is:
-        ```
-        pip install pycapacity
-        ```
-        And include it to your python project
-        ```python
-        import pycapacity.robot 
-        # and/or
-        import pycapacity.human 
-        #and/or
-        import pycapacity.algorithms 
-        #and/or
-        import pycapacity.visual 
-        ```
-        
-        Other way to install the code is by installing it directly from the git repo:
-        ```
-        pip install git+https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/
-        ```
-        
-        ## Package API docs
-        
-        See full docs at the [link](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
-        
-        ### Modules
-        
-        - [`human`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.human.html#module-pycapacity.human)
-        - [`robot`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
-        - [`algorithms`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
-        - [`visual`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
-        
-        ### Functions
-        
-        Robot metrics
-        - [`robot.acceleration_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
-        - [`robot.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
-        - [`robot.acceleration_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
-        - [`robot.force_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
-        - [`robot.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
-        - [`robot.force_polytope_intersection`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-        - [`robot.force_polytope_intersection_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-        - [`robot.force_polytope_sum_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
-        - [`robot.force_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
-        - [`robot.velocity_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
-        - [`robot.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
-        - [`robot.velocity_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
-        
-        Human metrics
-        - [`human.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
-        - [`human.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
-        - [`human.joint_torques_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
-        - [`human.torque_to_muscle_force`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
-        - [`human.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
-        
-        
-        Algorithms
-        - [`algorithms.hyper_plane_shift_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
-        - [`algorithms.iterative_convex_hull_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
-        - [`algorithms.vertex_enumeration_auctus`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
-        
-        
-        Visualisation tools
-        - [`visual.plot_polytope_faces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
-        - [`visual.plot_polytope_vertex`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
-        ---
-        
-        ## Code examples
-        
-        See [`demo_notebook.ipynb`](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
-        
-        ### Randomised serial robot example
-        ```python
-        """
-        A simple example program for 3d force polytope 
-        evaluation of a randomised 6dof robot 
-        """
-        import pycapacity.robot as capacity # robot capacity module
-        import numpy as np
-        
-        m = 3 # 3d forces
-        n = 6 # robot dof
-        
-        J = np.array(np.random.rand(m,n)) # random jacobian matrix
-        
-        t_max = np.ones(n)  # joint torque limits max and min
-        t_min = -np.ones(n)
-        
-        vertices, face_indexes = capacity.force_polytope_withfaces(J,t_min, t_max) # calculate the polytope vertices and faces
-        faces = capacity.face_index_to_vertex(vertices, face_indexes)
-        
-        print(vertices) # display the vertices
-        
-        # plotting the polytope
-        import matplotlib.pyplot as plt
-        from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
-        fig = plt.figure(4)
-        
-        # draw faces and vertices
-        ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
-        plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
-        
-        plt.tight_layout()
-        plt.legend()
-        plt.show()
-        ```
-        
-        
-        ### Randomised muslucoskeletal model example
-        ```python
-        """
-        A simple example program for 3d force polytope 
-        evaluation of a randomised 30 muscle 7dof 
-        human musculoskeletal model 
-        """
-        
-        import pycapacity.human as capacity # robot capacity module
-        import numpy as np
-        
-        L = 30 # number of muscles
-        m = 3 # 3d forces
-        n = 6 # number of joints - dof
-        
-        J = np.array(np.random.rand(m,n))*2-1 # random jacobian matrix
-        N = np.array(np.random.rand(n,L))*2-1 # random moment arm matrix
-        
-        F_max = 100*np.ones(L)  # muscle forces limits max and min
-        F_min = np.zeros(L)
-        
-        vertices, H,d, face_indexes = capacity.force_polytope(J,N, F_min, F_max, 0.1) # calculate the polytope vertices and faces
-        faces = capacity.face_index_to_vertex(vertices, face_indexes)
-        
-        print(vertices) # display the vertices
-        
-        # plotting the polytope
-        import matplotlib.pyplot as plt
-        from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
-        fig = plt.figure(4)
-        
-        # draw faces and vertices
-        ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
-        plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
-        
-        plt.tight_layout()
-        plt.legend()
-        plt.show()
-        
-        ```
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Robot Framework
-Classifier: Framework :: Robot Framework :: Library
-Classifier: Framework :: Robot Framework :: Tool
-Description-Content-Type: text/markdown
+
+# Real-time capable task-space capacity calculation python module
+
+<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
+<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
+
+The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
+- Robotic serial manipulators - `pycapacity.robot`
+- Human musculoskeletal models - `pycapacity.human`
+
+This package also provides a module `pycapacity.algorithms` with a set of polytope evaluation algorithms for standard polytope formulations, that can be used as a standalone library.
+
+Additionally, `pycapacity.visual` module provides a set of visualisaiton tools using the `matplotlib` for visualising 2d and 3d polytopes.
+
+See [full API documentation and docs.](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+
+## Robotic manipulator capacity metrics
+<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/robot.png' height='300px'>
+
+For the robotic manipulators the package integrates several velocity, force and acceleration capacity calculation functions based on ellipsoids:
+- Velocity (manipulability) ellipsoid <br> `E_vel = {dx | dx = J.dq, ||dq||<1 }`
+- Acceleration (dynamic manipulability) ellipsoid <br> `E_acc = {ddx | ddx = J.M^(-1).t, ||t||<1 }`
+- Force ellipsoid <br> `E_for = {f | J^T.f = t, ||t||<1 }`
+
+And polytopes: 
+- Velocity polytope <br> `P_vel = {dx | dx = J.dq,  dq_min < dq < dq_max}`
+- Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).t, t_min < t < t_max}`
+- Force polytope <br> `P_for = {f | J^T.f = t, t_min < t < t_max}`
+- Force polytopes *Minkowski sum and intersection*
+
+Where `J` is the robot jacobian matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities and `t` is the vector of joint torques.
+
+The force polytope functions have been implemented according to the paper:<br>
+[**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
+by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
+
+And the velocity and acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
+[**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
+by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
+
+## Human musculoskeletal models capacity metrics
+<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/force.png' height='200px'>
+
+For the human musculoskeletal models this package implements the polytope metrics:
+- Velocity polytope <br> `P_vel = {dx | dx = J.dq, dl = L.dq  dl_min < dl < dl_max}`
+- Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).N.F, F_min < F < F_max}`
+- Force polytope <br> `P_for = {f | J^T.f = N.F, F_min < F < F_max}`
+
+Where `J` is the model's jacobian matrix, `L` si the muscle length jacobian matrix, `N= -L^T` is the moment arm matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities, `t` is the vector of joint torques, `dl` is the vector of the muscle stretching velocities and `F` is the vector of muscular forces. 
+
+The force and velocity polytope functions have been implemented according to the paper:<br>
+[**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
+by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
+
+And the acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
+[**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
+by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
+
+## Polytope evaluation algorithms
+
+There are three methods implemented in this paper to resolve all the polytope calculations:
+- Hyper-plane shifting method
+- Iterative convex hull method
+- Vertex enumeration auctus
+
+All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md). 
+
+### Hyper-plane shifting method
+[**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
+by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
+
+This method finds the half-space representation of the polytope of a class:
+```
+P = {x | x = By, y_min <= y <= y_max }
+```
+To find the vertices of the polytope after finding the half-space representation `Hx <= d` an convex-hull algorithm is used. 
+
+The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-hyper_plane_shift_method). 
+
+### Iterative convex-hull method
+[**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
+by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
+
+This method finds both vertex and half-space representation of the class of polytopes:
+```
+P = {x | Ax = By, y_min <= y <= y_max }
+``` 
+And it can be additionally extended to the case where there is an additional projection matrix `P` making a class of problems:
+```
+P = {x | x= Pz, Az = By, y_min <= y <= y_max }
+``` 
+
+The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-iterative_convex_hull_method)
+
+### Vertex enumeration auctus
+[**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
+by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
+
+This method finds vertex representation of the class of polytopes:
+```
+P = {x | Ax = y, y_min <= y <= y_max }
+``` 
+To find the half-space representation (faces) of the polytope after finding the vertex representation  an convex-hull algorithm is used. 
+
+The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-vertex_enumeration_auctus)
+
+## Installation
+
+All you need to do to install it is:
+```
+pip install pycapacity
+```
+And include it to your python project
+```python
+import pycapacity.robot 
+# and/or
+import pycapacity.human 
+#and/or
+import pycapacity.algorithms 
+#and/or
+import pycapacity.visual 
+```
+
+Other way to install the code is by installing it directly from the git repo:
+```
+pip install git+https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/
+```
+
+## Package API docs
+
+See full docs at the [link](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+
+### Modules
+
+- [`human`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.human.html#module-pycapacity.human)
+- [`robot`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
+- [`algorithms`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
+- [`visual`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
+
+### Functions
+
+Robot metrics
+- [`robot.acceleration_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
+- [`robot.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
+- [`robot.acceleration_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
+- [`robot.force_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
+- [`robot.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
+- [`robot.force_polytope_intersection`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_sum_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
+- [`robot.velocity_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
+- [`robot.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
+- [`robot.velocity_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
+
+Human metrics
+- [`human.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
+- [`human.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
+- [`human.joint_torques_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
+- [`human.torque_to_muscle_force`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
+- [`human.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
+
+
+Algorithms
+- [`algorithms.hyper_plane_shift_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
+- [`algorithms.iterative_convex_hull_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
+- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
+
+
+Visualisation tools
+- [`visual.plot_polytope_faces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
+- [`visual.plot_polytope_vertex`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
+---
+
+## Code examples
+
+See [`demo_notebook.ipynb`](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
+
+### Randomised serial robot example
+```python
+"""
+A simple example program for 3d force polytope 
+evaluation of a randomised 6dof robot 
+"""
+import pycapacity.robot as capacity # robot capacity module
+import numpy as np
+
+m = 3 # 3d forces
+n = 6 # robot dof
+
+J = np.array(np.random.rand(m,n)) # random jacobian matrix
+
+t_max = np.ones(n)  # joint torque limits max and min
+t_min = -np.ones(n)
+
+vertices, face_indexes = capacity.force_polytope_withfaces(J,t_min, t_max) # calculate the polytope vertices and faces
+faces = capacity.face_index_to_vertex(vertices, face_indexes)
+
+print(vertices) # display the vertices
+
+# plotting the polytope
+import matplotlib.pyplot as plt
+from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
+fig = plt.figure(4)
+
+# draw faces and vertices
+ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
+plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
+
+plt.tight_layout()
+plt.legend()
+plt.show()
+```
+
+
+### Randomised muslucoskeletal model example
+```python
+"""
+A simple example program for 3d force polytope 
+evaluation of a randomised 30 muscle 7dof 
+human musculoskeletal model 
+"""
+
+import pycapacity.human as capacity # robot capacity module
+import numpy as np
+
+L = 30 # number of muscles
+m = 3 # 3d forces
+n = 6 # number of joints - dof
+
+J = np.array(np.random.rand(m,n))*2-1 # random jacobian matrix
+N = np.array(np.random.rand(n,L))*2-1 # random moment arm matrix
+
+F_max = 100*np.ones(L)  # muscle forces limits max and min
+F_min = np.zeros(L)
+
+vertices, H,d, face_indexes = capacity.force_polytope(J,N, F_min, F_max, 0.1) # calculate the polytope vertices and faces
+faces = capacity.face_index_to_vertex(vertices, face_indexes)
+
+print(vertices) # display the vertices
+
+# plotting the polytope
+import matplotlib.pyplot as plt
+from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
+fig = plt.figure(4)
+
+# draw faces and vertices
+ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
+plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
+
+plt.tight_layout()
+plt.legend()
+plt.show()
+
+```
```

### Comparing `pycapacity-1.2.8/pycapacity/algorithms.py` & `pycapacity-1.2.9/pycapacity/algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from math import sin, cos 
 import numpy as np
 import numpy.matlib 
 import itertools
 from scipy.spatial import ConvexHull, HalfspaceIntersection
 from cvxopt import matrix
 import cvxopt.glpk
+from scipy.optimize import linprog
 
 
 def iterative_convex_hull_method(A, B, y_min, y_max, tol, P = None, bias = None,  G_in = None, h_in = None, G_eq = None, h_eq = None):
     """
     A function calculating the polytopes of achievable x for equations form:
 
     .. math:: z = By, \quad Ax = z
@@ -26,18 +27,20 @@
 
     (optionally - additional bias)
 
     .. math:: Az = By + bias
     .. math:: y_{min} \leq y \leq y_{max}
 
     (optionally - additional inequality constaints)
-    .. math:: G{in} x \leq h_{in}    
+
+    .. math:: G_{in} x \leq h_{in}    
     
     (optionally - additional equality constaints)
-    .. math:: G{eq} x = h_{eq}
+
+    .. math:: G_{eq} x = h_{eq}
 
     Note:
         On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method
         A.Skuric,V.Padois,N.Rezzoug,D.Daney 
 
     Args:
         A: matrix
@@ -126,37 +129,37 @@
     if P is not None:
         # check the size
         nP, mP = P.shape
         if mP != m or nP > mP:
             raise ValueError('Matrix P dimensions error - (rows,cols) = P.shape should be: rows > cols and cols = {:d}. In your case P.shape = {}.'.format(m,P.shape))
         M = P.dot(M)
         x_bias = P.dot(x_bias)
-        u = P.dot(u)     
+        u = P.dot(u)  
 
     if G_in is not None:
         # check the size
         nG, mG = G_in.shape
         if mG != L:
-            raise ValueError('Matrix G_in dimensions error - (rows,cols) = G_in.shape should be: col = {:d}. In your case P.shape = {}.'.format(m,G_in.shape))
+            raise ValueError('Matrix G_in dimensions error - (rows,cols) = G_in.shape should be: col = {:d}. In your case G_in.shape = {}.'.format(L,G_in.shape))
         if nG != len(h_in):
-            raise ValueError('Vector h_in dimensions error - should have {:d} entries. In your case P.shape = {}.'.format(nG,len(h_in)))    
+            raise ValueError('Vector h_in dimensions error - should have {:d} entries. In your case h_in.shape = {}.'.format(nG,len(h_in)))    
 
         G = matrix(np.vstack((-np.identity(L),np.identity(L),G_in)))
         h = matrix(np.hstack((list(-np.array(y_min)),y_max, h_in)))
     else:
         G = matrix(np.vstack((-np.identity(L),np.identity(L))))
         h = matrix(np.hstack((list(-np.array(y_min)),y_max)))
 
     if G_eq is not None:
-        # # check the size
-        # nG, mG = G_in.shape
-        # if mG != L:
-        #     raise ValueError('Matrix G_in dimensions error - (rows,cols) = G_in.shape should be: col = {:d}. In your case P.shape = {}.'.format(m,G_in.shape))
-        # if nG != len(h_in):
-        #     raise ValueError('Vector h_in dimensions error - should have {:d} entries. In your case P.shape = {}.'.format(nG,len(h_in)))    
+        # check the size
+        nG, mG = G_eq.shape
+        if mG != L:
+            raise ValueError('Matrix G_in dimensions error - (rows,cols) = G_in.shape should be: col = {:d}. In your case Geq.shape = {}.'.format(L,G_eq.shape))
+        if nG != len(h_eq):
+            raise ValueError('Vector h_in dimensions error - should have {:d} entries. In your case h_eq.shape = {}.'.format(nG,len(h_eq)))    
         if Aeq is not None:
             Aeq = matrix(np.vstack((Aeq,G_eq)))
             beq = matrix(np.hstack((beq,h_eq)))
         else:
             Aeq = matrix(G_eq)
             beq = matrix(h_eq)
 
@@ -167,17 +170,19 @@
 
     solvers_opt={'tm_lim': 100000, 'msg_lev': 'GLP_MSG_OFF', 'it_lim':10000}
 
     y_vert, x_p = [],[]
     for i in range(m):
         c = matrix((u[:,i].T).dot(M))
         res = cvxopt.glpk.lp(c=-c,  A=Aeq, b=beq, G=G,h=h, options=solvers_opt)
-        y_vert = stack(y_vert, res[1],'h')
+        if res[1]:
+            y_vert = stack(y_vert, res[1],'h')
         res = cvxopt.glpk.lp(c=c,  A=Aeq, b=beq, G=G,h=h, options=solvers_opt)
-        y_vert = stack(y_vert, res[1],'h')
+        if res[1]:
+            y_vert = stack(y_vert, res[1],'h')
     x_p  = M.dot(y_vert) + x_bias
     z_vert = B.dot(y_vert) + bias
 
     # if one directin only
     if m == 1:
         return x_p, np.array([[1],[-1]]), np.array([[np.max(x_p)],[-np.max(x_p)]]), [], y_vert, z_vert
 
@@ -194,15 +199,15 @@
 
     n_faces, n_faces_old,  = len(hull.simplices), 0
     face_final, cnt = {}, 2*m
 
     while n_faces > n_faces_old:
         n_faces_old = n_faces
         
-        x_center = np.mean(x_p)
+        x_center = np.mean(x_p,axis=1)
         
         y_vert_new = []
 
         for face, equation in zip(hull.simplices,hull.equations):
             
             # create a string index of the face 
             # this value is used as a hash map index
@@ -245,17 +250,18 @@
                 hull = ConvexHull(x_p.T, incremental=True, qhull_options="QJ")
             
             y_vert = stack(y_vert, y_vert_new,'h')
             x_p  = stack(x_p, x_p_new,'h')
 
             z_new = B.dot(y_vert_new) + bias
             z_vert = stack(z_vert, z_new,'h')
-            
+ 
         n_faces = len(hull.simplices)
-    
+  
+
     return x_p, hull.equations[:,:-1], hull.equations[:,-1], hull.simplices, y_vert, z_vert
 
 
 def hyper_plane_shift_method(A, x_min, x_max, tol = 1e-15):
     """
     Hyper plane shifting method implementation used to solve problems of a form:
 
@@ -456,15 +462,30 @@
         vertices(list)  : vertices of the polytope
         face_indexes(list) : indexes of verteices forming triangulated faces of the polytope
 
     """
     if len(H):
         # calculate the certices
         hd_mat = np.hstack((np.array(H),-np.array(d)))
-        hd = HalfspaceIntersection(hd_mat,np.zeros(H.shape[1]),'QJ')
+
+        # calculating chebyshev center
+        # https://pageperso.lis-lab.fr/~francois.denis/IAAM1/scipy-html-1.0.0/generated/scipy.spatial.HalfspaceIntersection.html
+        norm_vector = np.reshape(np.linalg.norm(H[:, :-1], axis=1), (H.shape[0], 1))
+        c = np.zeros((hd_mat.shape[1],))
+        c[-1] = -1
+        A = np.hstack((hd_mat[:, :-1], norm_vector))
+        b = - hd_mat[:, -1:]
+        G = matrix(A)
+        h = matrix(b)
+        solvers_opt={'tm_lim': 100000, 'msg_lev': 'GLP_MSG_OFF', 'it_lim':10000}
+        res = cvxopt.glpk.lp(c=c,  G=G, h=h, options=solvers_opt)
+        feasible_point = np.array(res[1][:-1]).reshape((-1,))
+
+        # calculate the convex hull
+        hd = HalfspaceIntersection(hd_mat,feasible_point,'QJ')
         hull = ConvexHull(hd.intersections)
         return hd.intersections.T, hull.simplices
 
 def vertex_to_faces(vertex):
     if vertex.shape[0] == 1:
         faces = [0, 1]
     else:
```

### Comparing `pycapacity-1.2.8/pycapacity/human.py` & `pycapacity-1.2.9/pycapacity/human.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 from cvxopt import matrix
 import cvxopt.glpk
 
 # import the algos
 from pycapacity.algorithms import iterative_convex_hull_method, hyper_plane_shift_method
-from pycapacity.algorithms import stack, face_index_to_vertex,hsapce_to_vertex
+from pycapacity.algorithms import stack, face_index_to_vertex, hsapce_to_vertex
 
 
-def joint_torques_polytope(N, F_min, F_max, tol=1e-15):
+def joint_torques_polytope(N, F_min, F_max, options = None):
     """
     A function calculating the polytopes of achievable joint torques
     based on the moment arm matrix `N` :
     
     .. math:: t = NF
     .. math:: F_{min} \leq F \leq F_{max}
 
@@ -29,21 +29,45 @@
         t_vert(array):  
             list of torque vertices
         H(array):  
             half-space rep matrix H -  :math:`Ht < d`
         d(array):  
             half-space rep vector d
         faces: 
-            indexes of verteices forming the polytope faces
+            indexes of vertices forming the polytope faces
     """
-    H, d = hyper_plane_shift_method(N, F_min, F_max)
-    vert, faces = hsapce_to_vertex(H,d)
-    return vert, H, d, faces
+    p = Polytope
+
+    if options is not None and options['algorithm'] is not None:
+        if "ichm" in options['algorithm']:
+            if options['precision'] is None:
+                options['precision'] = 1e-1
+            t_vert, H, d, face_indexes, F_vert, _t_vert = iterative_convex_hull_method(np.eye(N.shape[0]), N, F_min, F_max, options['precision'])
+            p.vertices = t_vert
+            p.H = h
+            p.d = d
+            p.face_indexes = face_indexes
+        elif "hpsm" in options['algorithm']:
+            H, d = hyper_plane_shift_method(N, F_min, F_max) 
+            p.H = h
+            p.d = d
+        else:
+            raise ValueError('Algorihtm - {} not supported. Supported algos are: "ichm" and "hpsm". '.format(options['algorithm']))
+    else: 
+        H, d = hyper_plane_shift_method(N, F_min, F_max)
+        p.H = h
+        p.d = d
+        if options['calc_vertices'] not None and options['calc_vertices'] == True:
+            vert, faces = hsapce_to_vertex(H,d)
+            p.face_indexes = faces            
+            p.vertices = vert
+            
+    return p
     
-def acceleration_polytope(J, N, M, F_min, F_max, tol=1e-15):
+def acceleration_polytope(J, N, M, F_min, F_max, tol=1e-15, options = None):
     """
     A function calculating the polytopes of achievable accelerations
     based on the jacobian matrix `J`, moment arm matrix `N` and mass matrix `M`
 
     .. math:: a = \ddot{x}   = JM^{-1}NF
     .. math:: F_{min} \leq F \leq F_{max}
 
@@ -69,15 +93,15 @@
         faces: 
             indexes of verteices forming the polytope faces
     """
     H,d = hyper_plane_shift_method(J.dot(np.linalg.inv(M).dot(N)),F_min,F_max)
     vert, faces = hsapce_to_vertex(H,d)
     return vert, H, d, faces
 
-def force_polytope(J, N, F_min, F_max, tol, torque_bias=None):
+def force_polytope(J, N, F_min, F_max, tol, torque_bias=None, options = None):
     """
     A function calculating the polytopes of achievable foreces based 
     on the jacobian matrix `J` and moment arm matrix `N`
 
     .. math:: J^Tf = NF \quad(+\, t_{bias})
     .. math::  F_{min} \leq F \leq F_{max}
         
@@ -101,15 +125,15 @@
             half-space rep vectors d
         faces(list):   
             list of vertex indexes forming polytope faces  
     """
     f_vert, H, d, faces , F_vert, t_vert = iterative_convex_hull_method(J.T, N, F_min, F_max, tol, bias=torque_bias)
     return f_vert, H, d, faces
 
-def velocity_polytope(J, N, dl_min , dl_max, tol):
+def velocity_polytope(J, N, dl_min , dl_max, tol, options = None):
     """
     A function calculating the polytopes of achievable velocity based 
     on the jacobian matrix `J` and moment arm matrix `N`
 
     .. math:: L\dot{q} = \dot{l}, \quad J\dot{q} = \dot{x} = v
     .. math:: \dot{l}_{min} \leq \dot{l} \leq \dot{l}_{max}
     
@@ -132,15 +156,15 @@
             half-space rep vectors d
         faces(list):   
             list of vertex indexes forming velocity polytope faces  
     """
     v_vert, H, d, faces , dl_vert, dq_vert = iterative_convex_hull_method(A=-N.T, B=np.eye(dl_min.shape[0]), P = J, y_min=dl_min, y_max=dl_max, tol=tol)
     return v_vert, H, d, faces
 
-def torque_to_muscle_force(N, F_min, F_max, tau, options="lp"):
+def torque_to_muscle_force(N, F_min, F_max, tau, options="lp", options = None):
     """
     A function calculating muscle forces needed to create the joint torques tau.
     It uses eaither the linear programming or quadratic programming, set with the ``options`` parameter.
 
     Args:
         N: moment arm matrix
         F_min: minimal muscular forces (passive forces or 0)
```

### Comparing `pycapacity-1.2.8/pycapacity/robot.py` & `pycapacity-1.2.9/pycapacity/robot.py`

 * *Files identical despite different names*

### Comparing `pycapacity-1.2.8/pycapacity/visual.py` & `pycapacity-1.2.9/pycapacity/visual.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,87 @@
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 from matplotlib.patches import Ellipse
+
+import pycapacity.algorithms as algos
+
+import plotly.graph_objects as go
 import numpy as np
 
+def init_plotly():
+    fig = go.Figure()
+    return fig
+
+def plotly_polytope(vert, face_index, fig, color=None, edge_color=None, vertex_color=None, alpha=None,label=None, center=None):
+    dim = min(np.array(vert).shape)
+
+    if dim == 2:
+        plotly_polytope_2d(vert, face_index, fig, color, edge_color, vertex_color, alpha,label, center)
+    elif dim == 3:
+        plotly_polytope_3d(vert, face_index, fig, color, edge_color, vertex_color, alpha,label, center)
+    else:
+        print("cannot visualise data with dimension: "+str(dim))
+
+def plotly_polytope_2d(vert, face_index, fig, color=None, edge_color=None, vertex_color=None, alpha=None,label=None, center=None):
+    # extract the vertices
+    x,y = algos.face_index_to_vertex(vert, face_index)
+    x = np.hstack((x,x[0]))
+    y = np.hstack((y,y[0]))
+    fig.add_trace(
+        go.Scatter(
+            x=x, 
+            y=y, 
+            fill="toself",
+            fillcolor=color,
+            line=dict(color=edge_color),
+            marker=dict(
+                color=vertex_color,
+                # size=2,
+            )
+        )
+    )
+
+def plotly_polytope_3d(vert, face_index, fig, color=None, edge_color=None, vertex_color=None, alpha=None,label=None, center=None):
+    # extract the vertices
+    x,y,z = vert
+    # extract the face indexes
+    i,j,k = face_index.T
+    
+    fig.add_trace(go.Mesh3d
+    (x=x, 
+     y=y, 
+     z=z,
+     i=i,
+     j=j,
+     k=k,
+     color=color,
+     name=label, 
+     showlegend=True,
+     opacity=alpha)
+    )
+
+    # create the necessary for line and pint structure
+    v = np.vstack(([vert.T[face_index[0][i%3]] for i in range(4)] , np.array([None, None, None])))
+    for T in face_index[1:]:
+        v = np.vstack((v, [vert.T[T[i%3]] for i in range(4)] , np.array([None, None, None])))
+    x,y,z = np.array(v).T
+
+    # plot the edges and vertices
+    fig.add_trace(go.Scatter3d(
+        x=x,
+        y=y,
+        z=z,
+        # mode='markers',
+        name='',
+        line=dict(color=edge_color),
+        marker=dict(
+            color=vertex_color,
+            size=2,
+        )))  
+
 def plot_polytope_faces(faces,ax=None, plt=None, face_color=None, edge_color=None, alpha=None,label=None, center=None):
     """ 
     Polytope faces plotting function in 2d and 3d. 
     
     Note:
         If provided matplotlib `plt` it will find the `ax` automatically. No need to provide the `ax`. If `ax` already defined no need to provide the `plt`.
 
@@ -123,15 +198,14 @@
             ax.scatter(vertex[0,:],vertex[1,:],vertex[2,:],color=color, label=label)
         else:
             ax.scatter(vertex[0,:],vertex[1,:],vertex[2,:],color=color)  
     else:
         print("cannot visualise data with dimension: "+str(dim))
     return ax   
 
-
 def plot_ellipsoid(radii, rotation, center=None, ax=None, plt=None, label=None, color=None, edge_color=None, alpha=1.0):
     """
     Plotting ellipsoid in 2d and 3d
 
     Note:
         If provided matplotlib `plt` it will find the `ax` automatically. No need to provide the `ax`. If `ax` already defined no need to provide the `plt`.
```

### Comparing `pycapacity-1.2.8/README.md` & `pycapacity-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pycapacity
+Version: 1.2.9
+Summary: A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models
+Home-page: https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity
+Author: Antun Skuric
+Author-email: antun.skuric@inria.fr
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Framework :: Robot Framework :: Tool
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # Real-time capable task-space capacity calculation python module
 
 <img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
 <img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
 
 The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
@@ -248,8 +266,9 @@
 ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
 plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
 
 plt.tight_layout()
 plt.legend()
 plt.show()
 
-```
+```
+
```

### Comparing `pycapacity-1.2.8/pycapacity.egg-info/PKG-INFO` & `pycapacity-1.2.9/pycapacity.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,271 +1,274 @@
 Metadata-Version: 2.1
 Name: pycapacity
-Version: 1.2.8
+Version: 1.2.9
 Summary: A real-time task space capacity calculation module for robotic manipulators and human musculoskeletal models
 Home-page: https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity
 Author: Antun Skuric
 Author-email: antun.skuric@inria.fr
 License: MIT
-Description: 
-        # Real-time capable task-space capacity calculation python module
-        
-        <img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
-        <img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
-        
-        The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
-        - Robotic serial manipulators - `pycapacity.robot`
-        - Human musculoskeletal models - `pycapacity.human`
-        
-        This package also provides a module `pycapacity.algorithms` with a set of polytope evaluation algorithms for standard polytope formulations, that can be used as a standalone library.
-        
-        Additionally, `pycapacity.visual` module provides a set of visualisaiton tools using the `matplotlib` for visualising 2d and 3d polytopes.
-        
-        See [full API documentation and docs.](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
-        
-        ## Robotic manipulator capacity metrics
-        <img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/robot.png' height='300px'>
-        
-        For the robotic manipulators the package integrates several velocity, force and acceleration capacity calculation functions based on ellipsoids:
-        - Velocity (manipulability) ellipsoid <br> `E_vel = {dx | dx = J.dq, ||dq||<1 }`
-        - Acceleration (dynamic manipulability) ellipsoid <br> `E_acc = {ddx | ddx = J.M^(-1).t, ||t||<1 }`
-        - Force ellipsoid <br> `E_for = {f | J^T.f = t, ||t||<1 }`
-        
-        And polytopes: 
-        - Velocity polytope <br> `P_vel = {dx | dx = J.dq,  dq_min < dq < dq_max}`
-        - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).t, t_min < t < t_max}`
-        - Force polytope <br> `P_for = {f | J^T.f = t, t_min < t < t_max}`
-        - Force polytopes *Minkowski sum and intersection*
-        
-        Where `J` is the robot jacobian matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities and `t` is the vector of joint torques.
-        
-        The force polytope functions have been implemented according to the paper:<br>
-        [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
-        by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
-        
-        And the velocity and acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
-        [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
-        by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
-        
-        ## Human musculoskeletal models capacity metrics
-        <img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/force.png' height='200px'>
-        
-        For the human musculoskeletal models this package implements the polytope metrics:
-        - Velocity polytope <br> `P_vel = {dx | dx = J.dq, dl = L.dq  dl_min < dl < dl_max}`
-        - Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).N.F, F_min < F < F_max}`
-        - Force polytope <br> `P_for = {f | J^T.f = N.F, F_min < F < F_max}`
-        
-        Where `J` is the model's jacobian matrix, `L` si the muscle length jacobian matrix, `N= -L^T` is the moment arm matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities, `t` is the vector of joint torques, `dl` is the vector of the muscle stretching velocities and `F` is the vector of muscular forces. 
-        
-        The force and velocity polytope functions have been implemented according to the paper:<br>
-        [**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
-        by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
-        
-        And the acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
-        [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
-        by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
-        
-        ## Polytope evaluation algorithms
-        
-        There are three methods implemented in this paper to resolve all the polytope calculations:
-        - Hyper-plane shifting method
-        - Iterative convex hull method
-        - Vertex enumeration auctus
-        
-        All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md). 
-        
-        ### Hyper-plane shifting method
-        [**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
-        by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
-        
-        This method finds the half-space representation of the polytope of a class:
-        ```
-        P = {x | x = By, y_min <= y <= y_max }
-        ```
-        To find the vertices of the polytope after finding the half-space representation `Hx <= d` an convex-hull algorithm is used. 
-        
-        The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-hyper_plane_shift_method). 
-        
-        ### Iterative convex-hull method
-        [**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
-        by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
-        
-        This method finds both vertex and half-space representation of the class of polytopes:
-        ```
-        P = {x | Ax = By, y_min <= y <= y_max }
-        ``` 
-        And it can be additionally extended to the case where there is an additional projection matrix `P` making a class of problems:
-        ```
-        P = {x | x= Pz, Az = By, y_min <= y <= y_max }
-        ``` 
-        
-        The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-iterative_convex_hull_method)
-        
-        ### Vertex enumeration auctus
-        [**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
-        by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
-        
-        This method finds vertex representation of the class of polytopes:
-        ```
-        P = {x | Ax = y, y_min <= y <= y_max }
-        ``` 
-        To find the half-space representation (faces) of the polytope after finding the vertex representation  an convex-hull algorithm is used. 
-        
-        The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-vertex_enumeration_auctus)
-        
-        ## Installation
-        
-        All you need to do to install it is:
-        ```
-        pip install pycapacity
-        ```
-        And include it to your python project
-        ```python
-        import pycapacity.robot 
-        # and/or
-        import pycapacity.human 
-        #and/or
-        import pycapacity.algorithms 
-        #and/or
-        import pycapacity.visual 
-        ```
-        
-        Other way to install the code is by installing it directly from the git repo:
-        ```
-        pip install git+https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/
-        ```
-        
-        ## Package API docs
-        
-        See full docs at the [link](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
-        
-        ### Modules
-        
-        - [`human`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.human.html#module-pycapacity.human)
-        - [`robot`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
-        - [`algorithms`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
-        - [`visual`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
-        
-        ### Functions
-        
-        Robot metrics
-        - [`robot.acceleration_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
-        - [`robot.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
-        - [`robot.acceleration_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
-        - [`robot.force_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
-        - [`robot.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
-        - [`robot.force_polytope_intersection`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-        - [`robot.force_polytope_intersection_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
-        - [`robot.force_polytope_sum_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
-        - [`robot.force_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
-        - [`robot.velocity_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
-        - [`robot.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
-        - [`robot.velocity_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
-        
-        Human metrics
-        - [`human.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
-        - [`human.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
-        - [`human.joint_torques_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
-        - [`human.torque_to_muscle_force`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
-        - [`human.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
-        
-        
-        Algorithms
-        - [`algorithms.hyper_plane_shift_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
-        - [`algorithms.iterative_convex_hull_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
-        - [`algorithms.vertex_enumeration_auctus`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
-        
-        
-        Visualisation tools
-        - [`visual.plot_polytope_faces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
-        - [`visual.plot_polytope_vertex`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
-        ---
-        
-        ## Code examples
-        
-        See [`demo_notebook.ipynb`](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
-        
-        ### Randomised serial robot example
-        ```python
-        """
-        A simple example program for 3d force polytope 
-        evaluation of a randomised 6dof robot 
-        """
-        import pycapacity.robot as capacity # robot capacity module
-        import numpy as np
-        
-        m = 3 # 3d forces
-        n = 6 # robot dof
-        
-        J = np.array(np.random.rand(m,n)) # random jacobian matrix
-        
-        t_max = np.ones(n)  # joint torque limits max and min
-        t_min = -np.ones(n)
-        
-        vertices, face_indexes = capacity.force_polytope_withfaces(J,t_min, t_max) # calculate the polytope vertices and faces
-        faces = capacity.face_index_to_vertex(vertices, face_indexes)
-        
-        print(vertices) # display the vertices
-        
-        # plotting the polytope
-        import matplotlib.pyplot as plt
-        from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
-        fig = plt.figure(4)
-        
-        # draw faces and vertices
-        ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
-        plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
-        
-        plt.tight_layout()
-        plt.legend()
-        plt.show()
-        ```
-        
-        
-        ### Randomised muslucoskeletal model example
-        ```python
-        """
-        A simple example program for 3d force polytope 
-        evaluation of a randomised 30 muscle 7dof 
-        human musculoskeletal model 
-        """
-        
-        import pycapacity.human as capacity # robot capacity module
-        import numpy as np
-        
-        L = 30 # number of muscles
-        m = 3 # 3d forces
-        n = 6 # number of joints - dof
-        
-        J = np.array(np.random.rand(m,n))*2-1 # random jacobian matrix
-        N = np.array(np.random.rand(n,L))*2-1 # random moment arm matrix
-        
-        F_max = 100*np.ones(L)  # muscle forces limits max and min
-        F_min = np.zeros(L)
-        
-        vertices, H,d, face_indexes = capacity.force_polytope(J,N, F_min, F_max, 0.1) # calculate the polytope vertices and faces
-        faces = capacity.face_index_to_vertex(vertices, face_indexes)
-        
-        print(vertices) # display the vertices
-        
-        # plotting the polytope
-        import matplotlib.pyplot as plt
-        from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
-        fig = plt.figure(4)
-        
-        # draw faces and vertices
-        ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
-        plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
-        
-        plt.tight_layout()
-        plt.legend()
-        plt.show()
-        
-        ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Framework :: Robot Framework :: Tool
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Real-time capable task-space capacity calculation python module
+
+<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/comparison.gif" height="250px">
+<img src="https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/bimanual1.png" height="150px">
+
+The `pycapacity` package provides a framework for the generic task-space capacity calculation for:
+- Robotic serial manipulators - `pycapacity.robot`
+- Human musculoskeletal models - `pycapacity.human`
+
+This package also provides a module `pycapacity.algorithms` with a set of polytope evaluation algorithms for standard polytope formulations, that can be used as a standalone library.
+
+Additionally, `pycapacity.visual` module provides a set of visualisaiton tools using the `matplotlib` for visualising 2d and 3d polytopes.
+
+See [full API documentation and docs.](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+
+## Robotic manipulator capacity metrics
+<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/robot.png' height='300px'>
+
+For the robotic manipulators the package integrates several velocity, force and acceleration capacity calculation functions based on ellipsoids:
+- Velocity (manipulability) ellipsoid <br> `E_vel = {dx | dx = J.dq, ||dq||<1 }`
+- Acceleration (dynamic manipulability) ellipsoid <br> `E_acc = {ddx | ddx = J.M^(-1).t, ||t||<1 }`
+- Force ellipsoid <br> `E_for = {f | J^T.f = t, ||t||<1 }`
+
+And polytopes: 
+- Velocity polytope <br> `P_vel = {dx | dx = J.dq,  dq_min < dq < dq_max}`
+- Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).t, t_min < t < t_max}`
+- Force polytope <br> `P_for = {f | J^T.f = t, t_min < t < t_max}`
+- Force polytopes *Minkowski sum and intersection*
+
+Where `J` is the robot jacobian matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities and `t` is the vector of joint torques.
+
+The force polytope functions have been implemented according to the paper:<br>
+[**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
+by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
+
+And the velocity and acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
+[**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
+by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
+
+## Human musculoskeletal models capacity metrics
+<img src='https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/raw/master/images/force.png' height='200px'>
+
+For the human musculoskeletal models this package implements the polytope metrics:
+- Velocity polytope <br> `P_vel = {dx | dx = J.dq, dl = L.dq  dl_min < dl < dl_max}`
+- Acceleration polytope <br> `P_acc = {ddx | ddx = J.M^(-1).N.F, F_min < F < F_max}`
+- Force polytope <br> `P_for = {f | J^T.f = N.F, F_min < F < F_max}`
+
+Where `J` is the model's jacobian matrix, `L` si the muscle length jacobian matrix, `N= -L^T` is the moment arm matrix, `f` is the vector of cartesian forces,`dx` and `ddx` are vectors fo cartesian velocities and accretions, `dq` is the vector of the joint velocities, `t` is the vector of joint torques, `dl` is the vector of the muscle stretching velocities and `F` is the vector of muscular forces. 
+
+The force and velocity polytope functions have been implemented according to the paper:<br>
+[**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
+by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
+
+And the acceleration polytopes are resolved using the *Hyper-plane shifting method*:<br>
+[**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
+by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
+
+## Polytope evaluation algorithms
+
+There are three methods implemented in this paper to resolve all the polytope calculations:
+- Hyper-plane shifting method
+- Iterative convex hull method
+- Vertex enumeration auctus
+
+All of the methods are implemented in the module `pycapacity.algorithms` and can be used as standalone functions.  See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md). 
+
+### Hyper-plane shifting method
+[**Characterization of Parallel Manipulator Available Wrench Set Facets**](http://www.lirmm.fr/krut/pdf/2010_gouttefarde_ark-0602650368/2010_gouttefarde_ark.pdf)<br>
+by Gouttefarde M., Krut S. <br>In: Lenarcic J., Stanisic M. (eds) Advances in Robot Kinematics: Motion in Man and Machine. Springer, Dordrecht (2010)
+
+This method finds the half-space representation of the polytope of a class:
+```
+P = {x | x = By, y_min <= y <= y_max }
+```
+To find the vertices of the polytope after finding the half-space representation `Hx <= d` an convex-hull algorithm is used. 
+
+The method is a part of the `pycapacity.algorithms` module `hyper_plane_shift_method`, See in [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-hyper_plane_shift_method). 
+
+### Iterative convex-hull method
+[**On-line feasible wrench polytope evaluation based on human musculoskeletal models: an iterative convex hull method**](https://hal.inria.fr/hal-03369576)<br> 
+by A.Skuric, V.Padois, N.Rezzoug and D.Daney<br> Submitted to RAL & ICRA2022 
+
+This method finds both vertex and half-space representation of the class of polytopes:
+```
+P = {x | Ax = By, y_min <= y <= y_max }
+``` 
+And it can be additionally extended to the case where there is an additional projection matrix `P` making a class of problems:
+```
+P = {x | x= Pz, Az = By, y_min <= y <= y_max }
+``` 
+
+The method is a part of the `pycapacity.algorithms` module `iterative_convex_hull_method`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-iterative_convex_hull_method)
+
+### Vertex enumeration auctus
+[**On-line force capability evaluation based on efficient polytope vertex search**](https://arxiv.org/abs/2011.05226)<br> 
+by A.Skuric, V.Padois and D.Daney<br> Published on ICRA2021
+
+This method finds vertex representation of the class of polytopes:
+```
+P = {x | Ax = y, y_min <= y <= y_max }
+``` 
+To find the half-space representation (faces) of the polytope after finding the vertex representation  an convex-hull algorithm is used. 
+
+The method is a part of the `pycapacity.algorithms` module `vertex_enumeration_auctus`. See the [docs for more info](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/docs/algorithms.md#function-vertex_enumeration_auctus)
+
+## Installation
+
+All you need to do to install it is:
+```
+pip install pycapacity
+```
+And include it to your python project
+```python
+import pycapacity.robot 
+# and/or
+import pycapacity.human 
+#and/or
+import pycapacity.algorithms 
+#and/or
+import pycapacity.visual 
+```
+
+Other way to install the code is by installing it directly from the git repo:
+```
+pip install git+https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/
+```
+
+## Package API docs
+
+See full docs at the [link](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/)
+
+### Modules
+
+- [`human`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.human.html#module-pycapacity.human)
+- [`robot`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#module-pycapacity.robot)
+- [`algorithms`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.algorithms.html#module-pycapacity.algorithms)
+- [`visual`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#module-pycapacity.visual)
+
+### Functions
+
+Robot metrics
+- [`robot.acceleration_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.robot.html#pycapacity.robot.acceleration_ellipsoid): acceleration ellipsoid calculation (dynamic manipulability ellipsoid)
+- [`robot.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope): Acceleration polytope calculating function
+- [`robot.acceleration_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.acceleration_polytope_withfaces): Acceleration polytope calculating function
+- [`robot.force_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_ellipsoid): force manipulability ellipsoid calculation
+- [`robot.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope): Force polytope representing the capacities of the two robots in a certain configuration
+- [`robot.force_polytope_intersection`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_intersection_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_intersection_withfaces): Force polytope representing the intersection of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_sum_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_sum_withfaces): Force polytope representing the minkowski sum of the capacities of the two robots in certain configurations.
+- [`robot.force_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.force_polytope_withfaces): Force polytope representing the capacities of the two robots in a certain configuration.
+- [`robot.velocity_ellipsoid`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_ellipsoid): velocity manipulability ellipsoid calculation
+- [`robot.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope): Velocity polytope calculating function
+- [`robot.velocity_polytope_withfaces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.robot\.html#pycapacity\.robot\.velocity_polytope_withfaces): Velocity polytope calculating function, with faces
+
+Human metrics
+- [`human.acceleration_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.acceleration_polytope): A function calculating the polytopes of achievable accelerations
+- [`human.force_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.force_polytope): A function calculating the polytopes of achievable foreces based 
+- [`human.joint_torques_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.joint_torques_polytope): A function calculating the polytopes of achievable joint torques
+- [`human.torque_to_muscle_force`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.torque_to_muscle_force): A function calculating muscle forces needed to create the joint torques tau
+- [`human.velocity_polytope`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.human\.html#pycapacity\.human\.velocity_polytope): A function calculating the  polytopes of achievable velocity based 
+
+
+Algorithms
+- [`algorithms.hyper_plane_shift_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.hyper_plane_shift_method): Hyper plane shifting method implementation used to solve problems of a form:
+- [`algorithms.iterative_convex_hull_method`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.iterative_convex_hull_method): A function calculating the polytopes of achievable x for equations form:
+- [`algorithms.vertex_enumeration_auctus`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity\.algorithms\.html#pycapacity\.algorithms\.vertex_enumeration_auctus): Efficient vertex enumeration algorithm for a problem of a form:
+
+
+Visualisation tools
+- [`visual.plot_polytope_faces`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#pycapacity.visual.plot_polytope_faces): Polytope faces plotting function in 2d and 3d
+- [`visual.plot_polytope_vertex`](https://auctus-team.gitlabpages.inria.fr/people/antunskuric/pycapacity/pycapacity.visual.html#fpycapacity.visual.plot_polytope_vertex): Polytope vertices plotting function in 2d and 3d
+---
+
+## Code examples
+
+See [`demo_notebook.ipynb`](https://gitlab.inria.fr/auctus-team/people/antunskuric/pycapacity/-/blob/master/demo_notebook.ipynb) for more examples of how ot use the module.
+
+### Randomised serial robot example
+```python
+"""
+A simple example program for 3d force polytope 
+evaluation of a randomised 6dof robot 
+"""
+import pycapacity.robot as capacity # robot capacity module
+import numpy as np
+
+m = 3 # 3d forces
+n = 6 # robot dof
+
+J = np.array(np.random.rand(m,n)) # random jacobian matrix
+
+t_max = np.ones(n)  # joint torque limits max and min
+t_min = -np.ones(n)
+
+vertices, face_indexes = capacity.force_polytope_withfaces(J,t_min, t_max) # calculate the polytope vertices and faces
+faces = capacity.face_index_to_vertex(vertices, face_indexes)
+
+print(vertices) # display the vertices
+
+# plotting the polytope
+import matplotlib.pyplot as plt
+from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
+fig = plt.figure(4)
+
+# draw faces and vertices
+ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
+plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
+
+plt.tight_layout()
+plt.legend()
+plt.show()
+```
+
+
+### Randomised muslucoskeletal model example
+```python
+"""
+A simple example program for 3d force polytope 
+evaluation of a randomised 30 muscle 7dof 
+human musculoskeletal model 
+"""
+
+import pycapacity.human as capacity # robot capacity module
+import numpy as np
+
+L = 30 # number of muscles
+m = 3 # 3d forces
+n = 6 # number of joints - dof
+
+J = np.array(np.random.rand(m,n))*2-1 # random jacobian matrix
+N = np.array(np.random.rand(n,L))*2-1 # random moment arm matrix
+
+F_max = 100*np.ones(L)  # muscle forces limits max and min
+F_min = np.zeros(L)
+
+vertices, H,d, face_indexes = capacity.force_polytope(J,N, F_min, F_max, 0.1) # calculate the polytope vertices and faces
+faces = capacity.face_index_to_vertex(vertices, face_indexes)
+
+print(vertices) # display the vertices
+
+# plotting the polytope
+import matplotlib.pyplot as plt
+from pycapacity.visual import plot_polytope_faces, plot_polytope_vertex # pycapacity visualisation tools
+fig = plt.figure(4)
+
+# draw faces and vertices
+ax = plot_polytope_vertex(plt=plt, vertex=vertices, label='force',color='blue')
+plot_polytope_faces(ax=ax, faces=faces, face_color='blue', edge_color='blue', alpha=0.2)
+
+plt.tight_layout()
+plt.legend()
+plt.show()
+
+```
+
```

