# Comparing `tmp/warmth-0.0.2.tar.gz` & `tmp/warmth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmth-0.0.2.tar", max compression
+gzip compressed data, was "warmth-0.0.3.tar", max compression
```

## Comparing `warmth-0.0.2.tar` & `warmth-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     7652 2024-04-09 10:10:23.254884 warmth-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     1286 2024-04-09 10:10:23.254884 warmth-0.0.2/README.md
--rw-r--r--   0        0        0      837 2024-04-09 10:10:52.983189 warmth-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       87 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/__init__.py
--rw-r--r--   0        0        0    33895 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/build.py
--rw-r--r--   0        0        0    44794 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/data/haq87.json
--rw-r--r--   0        0        0    39680 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/data.py
--rw-r--r--   0        0        0    78689 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/forward_modelling.py
--rw-r--r--   0        0        0      284 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/logging.py
--rw-r--r--   0        0        0    78829 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/mesh_model.py
--rw-r--r--   0        0        0     8296 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/mesh_utils.py
--rw-r--r--   0        0        0     1991 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/model.py
--rw-r--r--   0        0        0    10952 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/parameters.py
--rw-r--r--   0        0        0    19686 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/postprocessing.py
--rw-r--r--   0        0        0    25882 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/resqpy_helpers.py
--rw-r--r--   0        0        0    10027 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/simulator.py
--rw-r--r--   0        0        0     4255 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/utils.py
--rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 warmth-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-05-08 06:50:19.427116 warmth-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1286 2024-05-08 06:50:19.427116 warmth-0.0.3/README.md
+-rw-r--r--   0        0        0      854 2024-05-08 06:50:47.571419 warmth-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/__init__.py
+-rw-r--r--   0        0        0    33895 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/build.py
+-rw-r--r--   0        0        0    44794 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/data/haq87.json
+-rw-r--r--   0        0        0    39680 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/data.py
+-rw-r--r--   0        0        0    78689 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/forward_modelling.py
+-rw-r--r--   0        0        0      284 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/logging.py
+-rw-r--r--   0        0        0    80196 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/mesh_model.py
+-rw-r--r--   0        0        0     8296 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/mesh_utils.py
+-rw-r--r--   0        0        0     1991 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/model.py
+-rw-r--r--   0        0        0    10952 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/parameters.py
+-rw-r--r--   0        0        0    19686 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/postprocessing.py
+-rw-r--r--   0        0        0    30098 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/resqpy_helpers.py
+-rw-r--r--   0        0        0    10027 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/simulator.py
+-rw-r--r--   0        0        0     4255 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/utils.py
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 warmth-0.0.3/PKG-INFO
```

### Comparing `warmth-0.0.2/LICENSE.md` & `warmth-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/README.md` & `warmth-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/pyproject.toml` & `warmth-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "warmth"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Adam Cheng <52572642+adamchengtkc@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 xtgeo = "^3.4.0"
 numpy = "^1.26.0"
 pandas = "<2.0"
 scipy = "^1.11.3"
 progress = "^1.6"
 urllib3 = "^2.0.6"
 meshio = {extras = ["all"], version = "^5.3.4"}
-resqpy = "^4.12.1"
+resqpy = "^4.14.4"
 pillow = "^10.3.0"
+pyetp = "^0.0.7"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.25.2"
 notebook = "^7.0.4"
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 flake8 = "^6.1.0"
```

### Comparing `warmth-0.0.2/warmth/build.py` & `warmth-0.0.3/warmth/build.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/data/haq87.json` & `warmth-0.0.3/warmth/data/haq87.json`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/data.py` & `warmth-0.0.3/warmth/data.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/forward_modelling.py` & `warmth-0.0.3/warmth/forward_modelling.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/mesh_model.py` & `warmth-0.0.3/warmth/mesh_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Tuple
 import numpy as np
 from mpi4py import MPI
 import meshio
 import dolfinx  
 from petsc4py import PETSc
 import ufl
+import sys
 from scipy.interpolate import LinearNDInterpolator
 from progress.bar import Bar
 from warmth.build import single_node, Builder
 from .parameters import Parameters
 from warmth.logging import logger
 from .mesh_utils import  top_crust,top_sed,thick_crust,  top_lith, top_asth, top_sed_id, bottom_sed_id,interpolateNode, interpolate_all_nodes
 from .resqpy_helpers import write_tetra_grid_with_properties, write_hexa_grid_with_timeseries, write_hexa_grid_with_properties,read_mesh_resqml_hexa
@@ -250,15 +251,14 @@
             lid0 = hex_data_layerID[i]
             # 
             # discard aesth and lith (layer IDs -2, -3)
             #
             if (lid0>=-1) and (lid0<100):
                 hexa_to_keep.append(h)
                 lid_to_keep.append(lid0)
-                # cell_id_to_keep.append(self.node_index[i])
                 cell_id_to_keep.append(hex_data_nodeID[i])
                 minY = np.amin(np.array ( [x_original_order[hi,1] for hi in h] ))
                 if abs( self.node1D[hex_data_nodeID[i]].Y - minY)>1:
                     logger.warning( f"weird Y:  {minY}, {self.node1D[hex_data_nodeID[i]].Y}, {abs( self.node1D[hex_data_nodeID[i]].Y - minY)}, {i}, {hex_data_nodeID[i]}" )
                     breakpoint()
                 for hi in h:
                     p_to_keep.add(hi)
@@ -286,77 +286,82 @@
         #     lid0  = lid_to_keep[i]
 
         T_per_vertex_keep = [ T_per_vertex[i] for i in range(nv) if i in p_to_keep ]
         age_per_vertex_keep = [ self.age_per_vertex[i] for i in range(nv) if i in p_to_keep ]
 
         from os import path
         filename_hex = path.join(out_path, self.modelName+'_hexa_'+str(tti)+'.epc')
-        write_hexa_grid_with_properties(filename_hex, np.array(points_cached), hexa_renumbered, "hexamesh",
+        points_cached=np.array(points_cached)
+        write_hexa_grid_with_properties(filename_hex, points_cached, hexa_renumbered, "hexamesh",
             np.array(T_per_vertex_keep), np.array(age_per_vertex_keep), poro0_per_cell, decay_per_cell, density_per_cell,
             cond_per_cell, rhp_per_cell, lid_per_cell)
         return filename_hex
 
 
     def write_hexa_mesh_timeseries( self, out_path):
         """Prepares arrays and calls the RESQML output helper function for hexa meshes:  the lith and aesth are removed, and the remaining
            vertices and cells are renumbered;  the sediment properties are prepared for output.
 
            out_path: string: path to write the resqml model to (.epc and .h5 files)
 
            returns the filename (of the .epc file) that was written 
         """            
         hexaHedra, hex_data_layerID, hex_data_nodeID = self.buildHexahedra(keep_padding=False)
-
         hexa_to_keep = []
         p_to_keep = set()
         lid_to_keep = []
-        cond_per_cell = []
         cell_id_to_keep = []
         for i,h in enumerate(hexaHedra):
             lid0 = hex_data_layerID[i]
             # 
             # discard aesth and lith (layer IDs -2, -3)
             #
             if (lid0>=-1) and (lid0<100):
                 hexa_to_keep.append(h)
                 lid_to_keep.append(lid0)
                 cell_id_to_keep.append(hex_data_nodeID[i])
-                # k_cond_mean = []
                 for hi in h:
                     p_to_keep.add(hi)
-                #     k_cond_mean.append(self.thermalCond.x.array[hi])
-                # cond_per_cell.append( np.mean(np.array(k_cond_mean)))
 
-        # poro0_per_cell = np.array( [ self.getSedimentPropForLayerID('phi', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ] )
-        # decay_per_cell = np.array( [ self.getSedimentPropForLayerID('decay', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
-        # density_per_cell = np.array( [ self.getSedimentPropForLayerID('solidus', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
-        # cond_per_cell = np.array( [ self.getSedimentPropForLayerID('k_cond', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
-        # rhp_per_cell = np.array( [ self.getSedimentPropForLayerID('rhp', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
-        # lid_per_cell = np.array(lid_to_keep)
-
-        points_cached_series = []
-        Temp_per_vertex_series = []
-
-        for tti in self.time_indices:
-            x_original_order, T_per_vertex = self.get_node_pos_and_temp(tti)
-            T_per_vertex_filt = [ T_per_vertex[i] for i in range(x_original_order.shape[0]) if i in p_to_keep  ]
-            Temp_per_vertex_series.append(np.array(T_per_vertex_filt))
-            points_cached = []
-            point_original_to_cached = np.ones(x_original_order.shape[0], dtype = np.int32)  * (-1)
-            for i in range(x_original_order.shape[0]):
+
+        poro0_per_cell = np.array( [ self.getSedimentPropForLayerID('phi', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ] )
+        decay_per_cell = np.array( [ self.getSedimentPropForLayerID('decay', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        density_per_cell = np.array( [ self.getSedimentPropForLayerID('solidus', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        cond_per_cell = np.array( [ self.getSedimentPropForLayerID('k_cond', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        rhp_per_cell = np.array( [ self.getSedimentPropForLayerID('rhp', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        lid_per_cell = np.array(lid_to_keep)
+        
+        x_original_order, T_per_vertex = self.get_node_pos_and_temp(self.time_indices[0]) # oldest first
+        n_vertices = x_original_order.shape[0]
+        age_per_vertex_keep = np.array([ self.age_per_vertex[i] for i in range(n_vertices) if i in p_to_keep ])
+        Temp_per_vertex_series = np.empty([len(self.time_indices), len(p_to_keep)])
+        points_cached_series = np.empty([len(self.time_indices), len(p_to_keep),3])
+
+        for idx, tti in enumerate(self.time_indices): # oldest first
+            if idx > 0:
+                x_original_order, T_per_vertex = self.get_node_pos_and_temp(tti)
+            T_per_vertex_filt = [ T_per_vertex[i] for i in range(n_vertices) if i in p_to_keep  ]
+            Temp_per_vertex_series[idx,:] = T_per_vertex_filt
+            point_original_to_cached = np.full(n_vertices,-1,dtype = np.int32)
+            count = 0
+            for i in range(n_vertices):
                 if (i in p_to_keep):
-                    point_original_to_cached[i] = len(points_cached)
-                    points_cached.append(x_original_order[i,:])
-            points_cached_series.append(np.array(points_cached))
+                    points_cached_series[idx,count,:]=x_original_order[i,:]
+                    point_original_to_cached[i]= count
+                    count += 1
+            
+                    
         hexa_renumbered = [ [point_original_to_cached[i] for i in hexa] for hexa in hexa_to_keep ]
 
         from os import path
+
         filename_hex = path.join(out_path, self.modelName+'_hexa_ts_'+str(self.tti)+'.epc')
         write_hexa_grid_with_timeseries(filename_hex, points_cached_series, hexa_renumbered, "hexamesh",
-            Temp_per_vertex_series )
+            Temp_per_vertex_series,age_per_vertex_keep, poro0_per_cell, decay_per_cell, density_per_cell,
+            cond_per_cell, rhp_per_cell, lid_per_cell )
         return filename_hex
 
     def heatflow_at_crust_sed_boundary(self):
         hf_array = np.zeros([self.num_nodes_x-2*self.padX, self.num_nodes_y-2*self.padX])
         for hy in range(self.padX, self.num_nodes_y-self.padX):
             for hx in range(self.padX, self.num_nodes_x-self.padX):
                 v_per_n = int(self.mesh_vertices.shape[0]/(self.num_nodes_y*self.num_nodes_x))
@@ -1545,14 +1550,39 @@
         if transpose:
             assert res.flatten().shape[0] == x.shape[1]
         else:
             assert res.flatten().shape[0] == x.shape[0]
         return res.flatten()
 
 
+def global_except_hook(exctype, value, traceback):
+    """https://github.com/chainer/chainermn/issues/236
+    """
+    try:
+        sys.stderr.write("\n*****************************************************\n")
+        sys.stderr.write("Uncaught exception was detected on rank {}. \n".format(
+            MPI.COMM_WORLD.Get_rank()))
+        from traceback import print_exception
+        print_exception(exctype, value, traceback)
+        sys.stderr.write("*****************************************************\n\n\n")
+        sys.stderr.write("\n")
+        sys.stderr.write("Calling MPI_Abort() to shut down MPI processes...\n")
+        sys.stderr.flush()
+    finally:
+        try:       
+            MPI.COMM_WORLD.Abort(1)
+        except Exception as e:
+            sys.stderr.write("*****************************************************\n")
+            sys.stderr.write("Sorry, we failed to stop MPI, this process will hang.\n")
+            sys.stderr.write("*****************************************************\n")
+            sys.stderr.flush()
+            raise e
+
+sys.excepthook = global_except_hook
+
 def run_3d( builder:Builder, parameters:Parameters,  start_time=182, end_time=0, pad_num_nodes=0,
             out_dir = "out-mapA/",sedimentsOnly=False, writeout=True, base_flux=None):
     logger.setLevel(10)  # numeric level equals DEBUG
     comm = MPI.COMM_WORLD
     builder=interpolate_all_nodes(builder)
     nums = 4
     dt = parameters.myr2s / nums # time step is 1/4 of 1Ma
@@ -1608,13 +1638,13 @@
             comm.send(mm2.mesh.topology.index_map(0).local_to_global(list(range(mm2.mesh.geometry.x.shape[0]))) , dest=0, tag=((comm.rank-1)*10)+21)
             comm.send(mm2.mesh_reindex, dest=0, tag=((comm.rank-1)*10)+23)
             comm.send(mm2.mesh_vertices_age, dest=0, tag=((comm.rank-1)*10)+25)
             comm.send(mm2.posarr, dest=0, tag=((comm.rank-1)*10)+20)
             comm.send(mm2.Tarr, dest=0, tag=((comm.rank-1)*10)+24)
         if comm.rank==0:
             mm2.receive_mpi_messages()
-            EPCfilename = mm2.write_hexa_mesh_resqml("temp/", end_time)
-            logger.info(f"RESQML model written to: {EPCfilename}")
+            # EPCfilename = mm2.write_hexa_mesh_resqml("temp/", end_time)
+            # logger.info(f"RESQML model written to: {EPCfilename}")
             EPCfilename_ts = mm2.write_hexa_mesh_timeseries("temp/")
             logger.info(f"RESQML partial model with timeseries written to: {EPCfilename_ts}")
-            read_mesh_resqml_hexa(EPCfilename)  # test reading of the .epc file
+            read_mesh_resqml_hexa(EPCfilename_ts)  # test reading of the .epc file
     return mm2
```

### Comparing `warmth-0.0.2/warmth/mesh_utils.py` & `warmth-0.0.3/warmth/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/model.py` & `warmth-0.0.3/warmth/model.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/parameters.py` & `warmth-0.0.3/warmth/parameters.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/postprocessing.py` & `warmth-0.0.3/warmth/postprocessing.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/resqpy_helpers.py` & `warmth-0.0.3/warmth/resqpy_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import resqpy.property as rqp
 import resqpy.crs as rqc
 import resqpy.model as rq
 import resqpy.olio.uuid as bu
 import resqpy.unstructured as rug
 import resqpy.time_series as rts
-
+from warmth.logging import logger
 #
 # 
 #
 
 def read_mesh_resqml(epcfilename, meshTitle = 'tetramesh'):
     """Example code how to read the .epc file written by the write_tetra_grid_with_properties function.
        Extracts arrays of node positions and of tetrahedra indices.
@@ -257,34 +257,36 @@
     
     hexa.check_hexahedral()
 
     #
     # read properties
     #
 
-    temp_uuid = model.uuid(title = 'Temperature')
+    temp_uuid = model.uuids(title = 'Temperature')
+    temp_uuid = temp_uuid[0]
     assert temp_uuid is not None
     temp_prop = rqp.Property(model, uuid = temp_uuid)
     assert temp_prop.uom() == 'degC'
     assert temp_prop.indexable_element() == 'nodes'   # properties are defined either on nodes or on cells
     print( temp_prop.array_ref().shape, temp_prop.array_ref()[0:10] )  # .array_ref() exposes the values as numpy array
 
     layerID_uuid = model.uuid(title = 'LayerID')
     assert layerID_uuid is not None
     layerID_prop = rqp.Property(model, uuid = layerID_uuid)
     # assert layerID_prop.uom() == 'Euc'
     assert layerID_prop.is_continuous() == False
     assert layerID_prop.indexable_element() == 'cells'
     print( layerID_prop.array_ref().shape, layerID_prop.array_ref()[0:10] )  # .array_ref() exposes the values as numpy array
  
-    titles=['Temperature', 'Age', 'LayerID', 'Porosity_initial', 'Porosity_decay', 'Density_solid', 'insulance_thermal', 'Radiogenic_heat_production']
-    for title in titles:
-        prop_uuid = model.uuid(title = title)
+    titles=[ 'Age', 'LayerID', 'Porosity_initial', 'Porosity_decay', 'Density_solid', 'insulance_thermal', 'Radiogenic_heat_production']
+    titles_uuid = [model.uuid(title = title) for title in titles]
+    titles_uuid.append(temp_uuid)
+    for prop_uuid in titles_uuid:
         prop = rqp.Property(model, uuid = prop_uuid)
-        print(title, prop.indexable_element(), prop.uom(), prop.array_ref()[0:10] )
+        print(prop.title, prop.indexable_element(), prop.uom(), prop.array_ref()[0:10] )
     
 
 def write_hexa_grid_with_properties(filename, nodes, cells, modelTitle = "hexamesh",
     Temp_per_vertex=None, age_per_vertex=None, poro0_per_cell=None, decay_per_cell=None, density_per_cell=None,
     cond_per_cell=None, rhp_per_cell=None, lid_per_cell=None ):
     """Writes the given hexahedral mesh, defined by arrays of nodes and cell indices, into a RESQML .epc file
        Given SubsHeat properties are optionally written.
@@ -455,15 +457,16 @@
                                     indexable_element = 'cells',
                                     uom = 'W/m3')
 
     model.store_epc()
 
 
 def write_hexa_grid_with_timeseries(filename, nodes_series, cells, modelTitle = "hexamesh",
-    Temp_per_vertex_series=None ):
+    Temp_per_vertex_series=None, age_per_vertex=None, poro0_per_cell=None, decay_per_cell=None, density_per_cell=None,
+    cond_per_cell=None, rhp_per_cell=None, lid_per_cell=None ):
     """Writes the given hexahedral mesh, defined by arrays of nodes and cell indices, into a RESQML .epc file
        Given SubsHeat properties are optionally written.
  
        cells is an array of 8-arrays in which the nodes are ordered:     
                7------6
               /      /|
              /      / |
@@ -473,16 +476,16 @@
             | /      /
             |/      /
             0------1
 
        NOTE: writing properties that are defines per-node (have 'nodes' as indexable element) requires a patched version of resqpy!
     """
 
-    nodes = nodes_series[0]
-    node_count = len(nodes)
+    nodes_time_0 = nodes_series[-1,:,:] # present-day at last index
+    node_count = nodes_time_0.shape[0]
     faces_per_cell = []
     nodes_per_face = []
     faces_dict = {}
     faces_repeat = np.zeros(node_count*100, dtype = bool)
 
     cell_face_is_right_handed = np.zeros( len(cells)*6, dtype = bool)
     for ih,hexa in enumerate(cells):
@@ -510,16 +513,18 @@
     set_cell_count = int(len(faces_per_cell)/6)
     face_count = int(len(nodes_per_face)/4)
 
 
     model = rq.new_model(filename)
     crs = rqc.Crs(model)
     crs.create_xml()
+    # present-day is set as 1 due resqpy
+    million_years_offset = 0 
+    times_in_years = [ int(max((t+million_years_offset)*1e6, million_years_offset)) for t in list(range(nodes_series.shape[0]-1,-1,-1))]
 
-    times_in_years = [ max(int(t*1e6),1) for t in list(range(len(nodes_series)-1,-1,-1))]
     gts = rts.GeologicTimeSeries.from_year_list(model, times_in_years, title="warmth simulation")
     gts.create_xml()
     rts.timeframe_for_time_series_uuid(model, gts.uuid)
 
     # create an empty HexaGrid
     hexa = rug.HexaGrid(model, title = modelTitle)
     assert hexa.cell_shape == 'hexahedral'
@@ -539,48 +544,119 @@
     hexa.nodes_per_face_cl = np.arange(4, 4 * face_count + 1, 4, dtype = int)
     hexa.nodes_per_face = np.array(nodes_per_face)
 
     # face handedness
     hexa.cell_face_is_right_handed = cell_face_is_right_handed  # False for all faces for external cells
 
     # points
-    hexa.points_cached = nodes
+    hexa.points_cached = nodes_time_0
 
     # basic validity check
     hexa.check_hexahedral()
 
     hexa.create_xml()
     hexa.write_hdf5()
 
     if hexa.property_collection is None:
         hexa.property_collection = rqp.PropertyCollection(support = hexa)
     pc = hexa.property_collection
 
     # nodes0 = nodes.copy()
-    for time_index in range(len(nodes_series)-1,-1,-1):
-        # nodes2 = nodes0 + [0,0,time_index*10]
-        nodes2 = nodes_series[time_index].astype(np.float32)
+    for time_index in range(nodes_series.shape[0]-1,-1,-1):  #oldest first
+
+        nodes2 = nodes_series[time_index,:,:].astype(np.float32)
+
         pc.add_cached_array_to_imported_list(nodes2,
                                                 'dynamic nodes',
-                                                'points',
+                                                "points",
                                                 uom = 'm',
                                                 property_kind = 'length',
                                                 realization = 0,
                                                 time_index = time_index,
                                                 indexable_element = 'nodes',
                                                 points = True)
         # active_array = np.ones([2160], dtype = bool)
         tt = Temp_per_vertex_series[time_index].astype(np.float32)
         pc.add_cached_array_to_imported_list(tt,
                                                 'Temperature',
-                                                'Temperature',
+                                                "Temperature",
                                                 uom = 'degC',
                                                 property_kind = 'thermodynamic temperature',
                                                 realization = 0,
                                                 time_index = time_index,
                                                 indexable_element = 'nodes')
                                                 # points = True)
     pc.write_hdf5_for_imported_list()
     pc.create_xml_for_imported_list_and_add_parts_to_model(time_series_uuid = gts.uuid)
 
+
+    if age_per_vertex is not None:
+        _ = rqp.Property.from_array(model,
+                                    age_per_vertex.astype(np.float32),
+                                    source_info = 'SubsHeat',
+                                    keyword = 'Age',
+                                    support_uuid = hexa.uuid,
+                                    property_kind = 'geological age',
+                                    indexable_element = 'nodes',
+                                    uom = 'y')
+
+    if lid_per_cell is not None:
+        _ = rqp.Property.from_array(model,
+                                    lid_per_cell.astype(np.int32),
+                                    source_info = 'SubsHeat',
+                                    keyword = 'LayerID',
+                                    support_uuid = hexa.uuid,
+                                    property_kind = 'layer ID',
+                                    indexable_element = 'cells',
+                                    uom = 'Euc',
+                                    discrete=True)
+         
+    if poro0_per_cell is not None:
+        _ = rqp.Property.from_array(model,
+                                    poro0_per_cell.astype(np.float32),
+                                    source_info = 'SubsHeat',
+                                    keyword = 'Porosity_initial',
+                                    support_uuid = hexa.uuid,
+                                    property_kind = 'porosity',
+                                    indexable_element = 'cells',
+                                    uom = 'm3/m3')
+    if decay_per_cell is not None:
+        _ = rqp.Property.from_array(model,
+                                    decay_per_cell.astype(np.float32),
+                                    source_info = 'SubsHeat',
+                                    keyword = 'Porosity_decay',
+                                    support_uuid = hexa.uuid,
+                                    property_kind = 'porosity decay',
+                                    indexable_element = 'cells',
+                                    uom = 'Euc')
+    if density_per_cell is not None:
+        _ = rqp.Property.from_array(model,
+                                    density_per_cell.astype(np.float32),
+                                    source_info = 'SubsHeat',
+                                    keyword = 'Density_solid',
+                                    support_uuid = hexa.uuid,
+                                    property_kind = 'density',
+                                    indexable_element = 'cells',
+                                    uom = 'kg/m3')
+    if cond_per_cell is not None:
+        #
+        # we write thermal conductivity as its inverse, the thermal insulance
+        #
+        _ = rqp.Property.from_array(model,
+                                    np.reciprocal(cond_per_cell).astype(np.float32),
+                                    source_info = 'SubsHeat',
+                                    keyword = 'insulance_thermal',
+                                    support_uuid = hexa.uuid,
+                                    property_kind = 'thermal insulance',
+                                    indexable_element = 'cells',
+                                    uom = 'deltaK.m2/W')
+    if rhp_per_cell is not None:
+        _ = rqp.Property.from_array(model,
+                                    rhp_per_cell.astype(np.float32),
+                                    source_info = 'SubsHeat',
+                                    keyword = 'Radiogenic_heat_production',
+                                    support_uuid = hexa.uuid,
+                                    property_kind = 'heat',
+                                    indexable_element = 'cells',
+                                    uom = 'W/m3')
     model.store_epc()
```

### Comparing `warmth-0.0.2/warmth/simulator.py` & `warmth-0.0.3/warmth/simulator.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/warmth/utils.py` & `warmth-0.0.3/warmth/utils.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.2/PKG-INFO` & `warmth-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: warmth
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Adam Cheng
 Author-email: 52572642+adamchengtkc@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: meshio[all] (>=5.3.4,<6.0.0)
 Requires-Dist: numpy (>=1.26.0,<2.0.0)
 Requires-Dist: pandas (<2.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: progress (>=1.6,<2.0)
-Requires-Dist: resqpy (>=4.12.1,<5.0.0)
+Requires-Dist: pyetp (>=0.0.7,<0.0.8)
+Requires-Dist: resqpy (>=4.14.4,<5.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Requires-Dist: urllib3 (>=2.0.6,<3.0.0)
 Requires-Dist: xtgeo (>=3.4.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Warmth
 ## Forward modeling of thermal evolution through geological time
```

