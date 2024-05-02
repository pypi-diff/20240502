# Comparing `tmp/w2rpy-0.1.1.tar.gz` & `tmp/w2rpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2rpy-0.1.1.tar", last modified: Wed May  1 21:17:26 2024, max compression
+gzip compressed data, was "w2rpy-0.1.2.tar", last modified: Thu May  2 14:44:21 2024, max compression
```

## Comparing `w2rpy-0.1.1.tar` & `w2rpy-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 21:17:26.635889 w2rpy-0.1.1/
--rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      416 2024-05-01 21:17:26.635889 w2rpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.1/README.md
--rw-rw-rw-   0        0        0       86 2024-05-01 21:17:26.636903 w2rpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      702 2024-05-01 21:17:02.000000 w2rpy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:17:26.628890 w2rpy-0.1.1/w2rpy/
--rw-rw-rw-   0        0        0      114 2024-05-01 21:04:56.000000 w2rpy-0.1.1/w2rpy/__init__.py
--rw-rw-rw-   0        0        0    26127 2024-05-01 20:18:20.000000 w2rpy-0.1.1/w2rpy/w2rpy.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:17:26.634890 w2rpy-0.1.1/w2rpy.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-01 21:17:26.000000 w2rpy-0.1.1/w2rpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-01 21:17:26.000000 w2rpy-0.1.1/w2rpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 21:17:26.000000 w2rpy-0.1.1/w2rpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-01 21:17:26.000000 w2rpy-0.1.1/w2rpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-01 21:17:26.000000 w2rpy-0.1.1/w2rpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 14:44:21.554791 w2rpy-0.1.2/
+-rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-05-02 14:44:21.554791 w2rpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-02 14:44:21.555512 w2rpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      702 2024-05-02 14:44:16.000000 w2rpy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:44:21.550463 w2rpy-0.1.2/w2rpy/
+-rw-rw-rw-   0        0        0      114 2024-05-01 21:04:56.000000 w2rpy-0.1.2/w2rpy/__init__.py
+-rw-rw-rw-   0        0        0    26091 2024-05-02 02:33:12.000000 w2rpy-0.1.2/w2rpy/w2rpy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:44:21.554069 w2rpy-0.1.2/w2rpy.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/top_level.txt
```

### Comparing `w2rpy-0.1.1/LICENSE` & `w2rpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `w2rpy-0.1.1/w2rpy/w2rpy.py` & `w2rpy-0.1.2/w2rpy/w2rpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Created on Wed May  1 10:36:37 2024
 
 @author: lrussell
 """
 
 import pandas as pd
 import numpy as np
-from shapely.geometry import Point,LineString,Polygon,MultiPolygon,shape
+from shapely.geometry import Point,LineString,Polygon,MultiPolygon,shape,box
 import geopandas as gpd
 import rasterio as rio
 from rasterio.mask import mask
 from rasterio.merge import merge
 from rasterio import features
 from rasterio.warp import Resampling
 from rasterio.warp import reproject,calculate_default_transform
@@ -52,15 +52,15 @@
     acc = acc
     print('Flow accumulation computed')
     
     terrain = Terrain(grid,dem,fdir,acc,crs)
     
     return terrain
 
-def streamlines(terrain, pour_point, threshold=None, snap_threshold=None,save=None):
+def streamlines(terrain, pour_point, threshold=None, snap_threshold=None, save=None):
     
     grid = copy.deepcopy(terrain.grid)
     
     if threshold is None:
         threshold = grid.size/100
     if snap_threshold is None:
         snap_threshold = grid.size/10
@@ -84,15 +84,17 @@
     # Clip the grid to the catchment
     grid.clip_to(catch)
 
     # Extract river network to geodataframe 
     branches = grid.extract_river_network(terrain.fdir, terrain.acc > threshold)
     file = str(branches)
     
-    lines = gpd.read_file(file,crs=terrain.crs)
+    lines = gpd.read_file(file)
+    lines.crs = terrain.crs
+    
     if save:
         lines.to_file(save)
         print('Stream network extracted')
     else:
         print('Stream network extracted')
         return lines
     
@@ -121,14 +123,15 @@
     # Clip the grid to the catchment
     grid.clip_to(catch)
     
     #get shapefile of catchment
     shapes = grid.polygonize()
     for shape in shapes:
         coords = np.asarray(shape[0]['coordinates'][0])
+        
     cm = gpd.GeoDataFrame([],geometry=[Polygon(coords)],crs=terrain.crs)  
       
     if save:
         cm.to_file(save)
         print('Catchment delineated')
     else:
         print('Catchment delineated')
@@ -164,17 +167,15 @@
             xs_lines.loc[len(xs_lines)] = [idx,xs*spacing,line]
     
     xs_lines = gpd.GeoDataFrame(xs_lines,geometry=xs_lines.geometry,crs=xs_lines.crs)
     xs_lines.set_crs(cl.crs, inplace=True)
     
     if save:
         xs_lines.to_file(save)
-        print('Cross-sections created')
     else:
-        print('Cross-sections created')
         return xs_lines
 
 def get_points(lines,spacing,ep=True,save=None):
     if isinstance(lines,str):
         lines = gpd.read_file(lines)
         
     def _get_points_ep(row):
@@ -200,17 +201,15 @@
     else:
         lines['points'] = lines.apply(lambda row: _get_points(row), axis=1)
         
     points = pd.concat(lines.points.values)
     
     if save:
         points.to_file(save)
-        print('Points created')
     else:
-        print('Points created')
         return points
 
 def inundate(raster,rel_wse_list,largest_only=False,invert=False,remove_holes=False,save=None):
     
     with rio.open(raster) as src:
 
         array = src.read(1)
@@ -258,15 +257,15 @@
             if poly.geom_type=='MultiPolygon':
                 polys = []
                 for geom in poly.geoms:
                     polys.append(Polygon(geom.exterior.coords))
                 new_poly = MultiPolygon(polys)
             return new_poly
         
-        inundate.geometry = inundate.geometry.apply(lambda poly: _remove_holes(poly))
+        inundated.geometry = inundated.geometry.apply(lambda poly: _remove_holes(poly))
     
     if save:
         inundated.to_file(save)
     else:
         return inundated
 
 def edit_raster(raster,output,crs=None,resample=None,resample_method='bilinear',clip=None,nodata=None):        
@@ -583,23 +582,18 @@
             if multiband:
                 sampled_data = [x.tolist() for x in src.sample(zip(points.geometry.x,points.geometry.y),masked=True)]
             else:
                 sampled_data = [x.tolist()[0] for x in src.sample(zip(points.geometry.x,points.geometry.y),masked=True)]
     
     return sampled_data
 
-def create_REM(dem,vcl,xs,output,sample_dist=3,smooth_window=5,buffer=2500,limits=[-50,50],method='min',vb=None,ret_xs=False,wse_path=None):
+def create_REM(dem,xs,output,sample_dist=3,smooth_window=5,buffer=1000,limits=[-50,50],method='min',vb=None,ret_xs=False,wse_path=None):
     with rio.open(dem) as src:
         crs = src.crs
     
-    if isinstance(vcl,str):
-        cl = gpd.read_file(vcl).to_crs(crs)
-    else:
-        cl = vcl.to_crs(crs)
-    
     # load cross-sections and clip to the valley bottom polygon (if provided)
     if isinstance(xs,str):
         xs = gpd.read_file(xs).to_crs(crs)
     else:
         xs = xs.to_crs(crs)
     
     if vb:
@@ -615,135 +609,135 @@
         xs['Z'] = xsp.groupby('CSID')['Z'].min()
         xs['Z'] = xs['Z'].rolling(smooth_window,center=True,min_periods=1).mean()
     elif method =='mean':
         xs['Z'] = xsp.groupby('CSID')['Z'].mean()
         xs['Z'] = xs['Z'].rolling(smooth_window,center=True,min_periods=1).mean()
     
     # create points to be used for interpolation
-    int_points = get_points(xs,xs.length.mean/2)
-    int_points['elevation'] = int_points.CSID.map(dict(zip(xs.index,xs.Z)))
+    int_points = get_points(xs,xs.length.mean()/2)
+    int_points['Z'] = int_points.CSID.map(dict(zip(xs.index,xs.Z)))
     int_points = int_points.dropna()
+    int_points.index = range(len(int_points))
+    int_points = int_points.iloc[int_points.round(1).drop_duplicates(subset=['CSID','Station']).index,:]
 
-    # before we go any further lets clip the raster to the buffer of the centerline
+    # before we go any further lets clip the raster to the buffer of the XSs
     with rio.open(dem,'r') as src:
-        cl = cl.to_crs(src.crs) 
-        bounds = src.bounds
-        extent = Polygon([(bounds.left,bounds.top),(bounds.right,bounds.top),(bounds.right,bounds.bottom),(bounds.left,bounds.bottom)])
-        cl = cl.intersection(extent)
-        
-        buffer_gdf = gpd.GeoDataFrame([],geometry=[cl.geometry.unary_union],crs=src.crs)
-        buffer_gdf.geometry = buffer_gdf.geometry.buffer(buffer)
-        masked_array, masked_transform = mask(src, shapes=buffer_gdf.geometry, crop=True, nodata=-9999)
+        masked_array, masked_transform = mask(src, shapes=[box(*xs.total_bounds).buffer(buffer)], crop=True, nodata=-9999, indexes=1)
+        nd_mask = (masked_array==-9999)
         
         # get masked raster geo data
         masked_profile = src.meta.copy()
         masked_profile.update({
             "driver": "GTiff",
-            "height": masked_array.shape[1],
-            "width": masked_array.shape[2],
+            "height": masked_array.shape[0],
+            "width": masked_array.shape[1],
             "transform": masked_transform,
             "nodata": -9999})
            
     #create linear Rbf interpolator
     int_r,int_c = rio.transform.rowcol(masked_transform, int_points.geometry.x, int_points.geometry.y)
-    rbfi = RBFInterpolator(np.vstack([int_c,int_r]).T, int_points.geometry.Z, kernel='linear')
+    rbfi = RBFInterpolator(np.vstack([int_c,int_r]).T, int_points.Z, kernel='linear')
     
     # interpolate REM zero elevation (wse) over cells within buffered mask
     ci,ri = np.meshgrid(np.arange(masked_array.shape[1]), np.arange(masked_array.shape[0]))
-    ci = ci[~masked_array.mask]
-    ri = ri[~masked_array.mask]
+    ci = ci[~nd_mask]
+    ri = ri[~nd_mask]
     
     int_wse = rbfi(np.stack([ci,ri]).T)
     wse = masked_array.copy()
-    wse[~masked_array.mask] = int_wse
+    wse[~nd_mask] = int_wse
     
     rem = masked_array - wse
     
     if limits:
         rem = np.where((rem>limits[1]) | (rem<limits[0]),-9999,rem)
+        
+    rem[nd_mask] = -9999
     
     with rio.open(output,'w',**masked_profile) as dst:
         dst.write(rem,indexes=1)
             
     if wse_path:
         with rio.open(wse_path,'w',**masked_profile) as wse_dst:
             wse_dst.write(wse,indexes=1)
             
     print('\nREM created at {0}'.format(output))
 
-def htab(station,elevation,slope,roughness,max_depth=10,errors='strict',save=None):
+def htab(station,elevation,slope,D50,max_depth=10,breaks=None,save=None):
+    station = np.array(station)
+    elevation = np.array(elevation)
     
     twg = np.min(elevation)
     
-    htab = pd.DataFrame([],columns=['d','wse','Q','u','n','S','A','P','R'])
+    htab = pd.DataFrame([],columns=['d','wse','Q','u','n','S','A','P','R','n_chan'])
     
     for d in np.linspace(0.1,max_depth,25):
         wse = twg + d
         
         boo = (elevation<wse)
         
         if boo.all():
             print('Error - Unconfined XS at {0}'.format(round(wse,2)))
             continue
         
         indices = np.nonzero(boo[1:] != boo[:-1])[0] + 1
-        indices = np.array([i-1 if np.where(indices==i)[0]%2==0 else i+1 for i in indices])
+        #indices = np.array([i-1 if np.where(indices==i)[0]%2==0 else i+1 for i in indices])
+        indices = np.array([i-1 if np.where(indices==i)[0]%2==0 else i for i in indices])
+        
+        chan_ind = np.array([np.argmin(abs(station-bound)) for bound in breaks])
+        chan_ind = np.delete(chan_ind,elevation[chan_ind]>wse)
+        indices = np.sort(np.unique(np.concatenate([indices,chan_ind]).flatten()))
         
         sta = np.split(station, indices)
-        sta = sta[0::2] if boo[0] else sta[1::2]
+        sta = [s for s in sta if (elevation[np.searchsorted(station,s)]<wse).any()]
+        sta = [np.append(s,station[np.argwhere(station==max(s))+1]) for s in sta]
         
         elev = np.split(elevation, indices)
-        elev = elev[0::2] if boo[0] else elev[1::2]
+        elev = [e for e in elev if (e<wse).any()]
+        elev = [np.append(e,max(elevation[np.argwhere(elevation==e[-1])+1])) for e in elev]
         
         channels = [np.array([sta[i],elev[i]]).astype(float) for i in range(len(sta))]
         channels = [chan for chan in channels if chan.size>0]
         
         aas = []
         ps = []
         rs = []
         qs = []
         us = []
+        ns = []
         for chan in channels:
             boo = (chan[1]<wse)
-            try:
-                if (boo[0]==True or boo[-1]==True):
-                    if errors == 'strict':
-                        print('Error - XS Unconfined at {0}'.format(round(wse,2)))
-                        break
-                    elif errors == 'ignore':
-                        continue
-                    else:
-                        print('Unknown Error Handling')
-                        return
-            except:
-                print(boo)
-                print(chan)
-                print(channels)
-                print(indices)
             
-            chan[0,0] = interp1d(chan[1,:2],chan[0,:2])(wse)
-            chan[0,-1] = interp1d(chan[1,-2:],chan[0,-2:])(wse)
+            if wse<chan[1,0]:
+                chan[0,0] = interp1d(chan[1,:2],chan[0,:2])(wse)
+            if wse<chan[1,-1]:
+                chan[0,-1] = interp1d(chan[1,-2:],chan[0,-2:])(wse)
                 
             chan[1,[0,-1]] = wse
     
             a = trapezoid(wse - chan[1],chan[0])
             p = np.sqrt(np.sum((chan.T[1:] - chan.T[:-1])**2, -1)).sum()
             
             r = a/p
             
-            u = (1.49/roughness)* r**(2/3) * slope**(0.5)
+            f = 8/(5.62*np.log10(a/(max(chan[0])-min(chan[0]))/D50)+4)**2
+            n = (1.49/(8*32.17*r*slope/f)**(1/2))*r**(2/3)*slope**(1/2)
+            if n > 0.2:
+                n = 0.2
+            
+            u = (1.49/n)* r**(2/3) * slope**(0.5)
             q = a*u
             
             aas.append(a)
             ps.append(p)
-            rs.append(r)
+            rs.append(r*q)
             qs.append(q)
-            us.append(u)
+            us.append(u*q)
+            ns.append(n*q)
             
-        htab.loc[len(htab)] = [d,wse,sum(qs),sum(us),roughness,slope,sum(aas),sum(ps),sum(rs)]
+        htab.loc[len(htab)] = [d,wse,sum(qs),sum(us)/sum(qs),sum(ns)/sum(qs),slope,sum(aas),sum(ps),sum(rs)/sum(qs),len(channels)]
+
         
     if save:
         htab.to_excel(save)
     else:
-        return htab
-
-
+        return htab
```

