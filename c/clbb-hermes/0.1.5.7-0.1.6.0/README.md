# Comparing `tmp/clbb-hermes-0.1.5.7.tar.gz` & `tmp/clbb_hermes-0.1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clbb-hermes-0.1.5.7.tar", last modified: Thu Apr 11 20:31:52 2024, max compression
+gzip compressed data, was "clbb_hermes-0.1.6.0.tar", last modified: Thu May  2 13:50:15 2024, max compression
```

## Comparing `clbb-hermes-0.1.5.7.tar` & `clbb_hermes-0.1.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 20:31:52.243672 clbb-hermes-0.1.5.7/
--rw-rw-rw-   0        0        0      321 2024-04-11 20:31:52.241671 clbb-hermes-0.1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-03-07 13:43:35.000000 clbb-hermes-0.1.5.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 20:31:52.239673 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/
--rw-rw-rw-   0        0        0      321 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 20:31:52.237671 clbb-hermes-0.1.5.7/hermes/
--rw-rw-rw-   0        0        0       48 2024-03-08 14:31:46.000000 clbb-hermes-0.1.5.7/hermes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-06 20:27:32.000000 clbb-hermes-0.1.5.7/hermes/functions.py
--rw-rw-rw-   0        0        0     4372 2024-04-11 16:38:51.000000 clbb-hermes-0.1.5.7/hermes/handler.py
--rw-rw-rw-   0        0        0       42 2024-04-11 20:31:52.244322 clbb-hermes-0.1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      384 2024-04-11 20:23:30.000000 clbb-hermes-0.1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:50:15.315558 clbb_hermes-0.1.6.0/
+-rw-rw-rw-   0        0        0      321 2024-05-02 13:50:15.314831 clbb_hermes-0.1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-03-07 13:43:35.000000 clbb_hermes-0.1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 13:50:15.313752 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/
+-rw-rw-rw-   0        0        0      321 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 13:50:15.312473 clbb_hermes-0.1.6.0/hermes/
+-rw-rw-rw-   0        0        0       48 2024-03-08 14:31:46.000000 clbb_hermes-0.1.6.0/hermes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 20:27:32.000000 clbb_hermes-0.1.6.0/hermes/functions.py
+-rw-rw-rw-   0        0        0     5486 2024-04-30 21:07:15.000000 clbb_hermes-0.1.6.0/hermes/handler.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 13:50:15.316578 clbb_hermes-0.1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      384 2024-04-30 21:21:54.000000 clbb_hermes-0.1.6.0/setup.py
```

### Comparing `clbb-hermes-0.1.5.7/hermes/handler.py` & `clbb_hermes-0.1.6.0/hermes/handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 from shapely import wkt
 from shapely.geometry import Point, LineString, Polygon
 
 
 class Handler:
     def __init__(self):
         self.server_address = os.getenv('server_address', 'http://localhost:8000')
-        self.request_data_endpoint = os.getenv('request_data_endpoint', 'api')
-        self.id_network = os.getenv('id_roadnetwork', 1)
         self.project_name = os.getenv('project_name', '')
+        self.set_project_id()
     
     @staticmethod
     def generate_unique_code(strings):
         text = ''.join(strings)
         return hashlib.sha256(text.encode()).hexdigest()
+    
+    def set_project_id(self):
+        url = f'{self.server_address}/interactive/project/get-project-id-by-name/?name={self.project_name}'
+        r = requests.get(url)
+        self.project_id = r.json()['project_id']
+        pass
 
     def post_data(self, endpoint='', data=None, headers={'Content-Type': 'application/json'}):
         endpoint = endpoint if endpoint else f'{self.server_address}/urban-indicators/indicatordata/upload_to_table/'
 
         json_data = json.dumps(data)
 
         response = requests.post(endpoint, headers=headers, data=json_data)
@@ -60,51 +65,68 @@
             "indicator_hash": indicator_hash,
         }
         data = self.get_data(endpoint, params, as_dataframe)
         data.drop(columns=['hash'], inplace=True)
         return data
 
     # Methods to load data from API
+    # http://192.168.31.120:8001/interactive/project/1/get-data/{which_one?}/
     
-    def load_amenities(self):
-        amenities = None
-        endpoint = f'{self.server_address}/{self.request_data_endpoint}/amenity/'
-        response = requests.get(endpoint)
-        data = response.json()
-        
+    def geojson_to_geodataframe(self, data_json):
         geometries = []
         properties = []
-        for feature in data['features']:
+        for feature in data_json['features']:
             geometries.append(wkt.loads(feature['geometry'].split(';')[-1]))
             properties.append(feature['properties'])
+        return gpd.GeoDataFrame(properties, geometry=geometries)
 
-        amenities = gpd.GeoDataFrame(properties, geometry=geometries)
+    def load_amenities(self):
+        amenities = None
+        endpoint = f'{self.server_address}/interactive/project/{self.project_id}/get-data/amenities/'
+        response = requests.get(endpoint)
+        data_json = response.json()
+        amenities = self.geojson_to_geodataframe(data_json=data_json)
         amenities.drop(columns=['tags'], inplace=True)
         return amenities
 
     def load_area_of_interest(self, id=1):
         area_of_interest = None
-        endpoint = f'{self.server_address}/{self.request_data_endpoint}/areaofinterest/{id}/'
+        endpoint = f'{self.server_address}/interactive/project/{self.project_id}/area-of-interest/'
         response = requests.get(endpoint)
         data = response.json()
         geometries= [wkt.loads(data['geometry'].split(';')[-1])]
         properties= [data['properties']]
-
         area_of_interest = gpd.GeoDataFrame(properties, geometry=geometries)
         area_of_interest = area_of_interest.set_crs(4326)
         return area_of_interest
-
+    
+    def load_aggregation_polys(self, dist_type=None, level=None):
+        endpoint = f'{self.server_address}/interactive/project/{self.project_id}/discrete-distributions/?dist_type={dist_type}&level={level}'
+        response = requests.get(endpoint)
+        data_json = response.json()
+        unit = self.geojson_to_geodataframe(data_json=data_json)
+        unit.set_crs(4326, inplace=True)
+        return unit
+    
+    def load_green_areas(self):
+        endpoint = f'{self.server_address}/interactive/project/{self.project_id}/get-data/green_areas/'
+        response = requests.get(endpoint)
+        data_json = response.json()
+        green_areas = self.geojson_to_geodataframe(data_json=data_json)
+        green_areas.set_crs(4326, inplace=True)
+        return green_areas
+        
     def load_network(self, id_network=None):
         if id_network is None:
             id_network = self.id_network
         download_path = '/app/tmp'
         os.makedirs(download_path, exist_ok=True)
         filename = os.path.join(download_path, f'net_{id_network}.h5')
         if not os.path.exists(filename):
-            endpoint = f'{self.server_address}/{self.request_data_endpoint}/roadnetwork/{id_network}/serve_h5_file/'
+            endpoint = f'{self.server_address}/api/roadnetwork/{id_network}/serve_h5_file/'
             print(endpoint)
             response = requests.get(endpoint)
             if response.status_code == 200:
                 with open(filename, 'wb') as f:
                     f.write(response.content)
                 print("¡Archivo h5 descargado exitosamente!")
             else:
```

