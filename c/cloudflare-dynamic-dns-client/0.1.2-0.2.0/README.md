# Comparing `tmp/cloudflare-dynamic-dns-client-0.1.2.tar.gz` & `tmp/cloudflare-dynamic-dns-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare-dynamic-dns-client-0.1.2.tar", last modified: Tue Apr 30 23:27:30 2024, max compression
+gzip compressed data, was "cloudflare-dynamic-dns-client-0.2.0.tar", last modified: Wed May  1 22:01:40 2024, max compression
```

## Comparing `cloudflare-dynamic-dns-client-0.1.2.tar` & `cloudflare-dynamic-dns-client-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 23:27:30.613798 cloudflare-dynamic-dns-client-0.1.2/
--rw-rw-rw-   0        0        0      237 2024-04-30 23:27:30.612790 cloudflare-dynamic-dns-client-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-04-30 21:50:57.000000 cloudflare-dynamic-dns-client-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 23:27:30.598215 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/
--rw-rw-rw-   0        0        0       64 2024-04-30 22:38:15.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/__init__.py
--rw-rw-rw-   0        0        0     3253 2024-04-30 22:59:20.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 23:27:30.611285 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/
--rw-rw-rw-   0        0        0      237 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 23:27:30.614796 cloudflare-dynamic-dns-client-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      446 2024-04-30 23:27:25.000000 cloudflare-dynamic-dns-client-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:01:40.779195 cloudflare-dynamic-dns-client-0.2.0/
+-rw-rw-rw-   0        0        0     1066 2024-05-01 21:41:51.000000 cloudflare-dynamic-dns-client-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1905 2024-05-01 22:01:40.778196 cloudflare-dynamic-dns-client-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1600 2024-05-01 21:58:36.000000 cloudflare-dynamic-dns-client-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 22:01:40.761664 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/
+-rw-rw-rw-   0        0        0       39 2024-05-01 21:59:54.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/__init__.py
+-rw-rw-rw-   0        0        0     4154 2024-05-01 21:53:39.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:01:40.777191 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/
+-rw-rw-rw-   0        0        0     1905 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 22:01:40.779195 cloudflare-dynamic-dns-client-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      506 2024-05-01 22:01:27.000000 cloudflare-dynamic-dns-client-0.2.0/setup.py
```

### Comparing `cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/__main__.py` & `cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,151 @@
 import os
-import CloudFlare
 import json
-from datetime import datetime
 import time
 import requests
+import logging
+import CloudFlare, CloudFlare.exceptions
+import sys
+
+dirpath = os.path.dirname(os.path.realpath(__file__))
+
+FORMAT = "%(asctime)s:%(levelname)s:%(name)s:%(message)s"
+logging.basicConfig(filename=os.path.join(dirpath, "latest.log"), encoding="utf-8", level=logging.INFO, format=FORMAT)
+logger = logging.getLogger("main")
+strmHndlr = logging.StreamHandler()
+strmHndlr.setFormatter(logging.Formatter(FORMAT))
+logger.addHandler(strmHndlr)
+
+def intput(text: str) -> int:
+	textvalue = input(text)
+	try:
+		return int(textvalue)
+	except ValueError:
+		return 0
 
-def intput(text):
-  textvalue = input(text)
-  try:
-    return int(textvalue)
-  except ValueError:
-    return 0
-
-def menu(text,items):
-	for i in range(len(items)):
-		print(f"{i + 1}) {items[i]}")
-     
-	value = 0
-	while value < 1 or value > len(items):
-		value = intput(text)
-	print()
-	return value - 1
-
-
-def multi_menu(text,items):
+def multi_menu(text: str, items: list[str]) -> list[int]:
 	items.append("Finish")
 	exit_number = len(items)
 
-	for i in range(len(items)):
-		print(f"{i + 1}) {items[i]}")
- 
-	all_selected = []
+	for i, elem in enumerate(items, start=1):
+		print(f"{i}) {elem}")
+
+	all_selected: list[int] = []
 
 	while True:
 		value = 0
 		while value < 1 or value > len(items):
 			value = intput(text)
-   
+
 		if value == exit_number:
 			break
 
 		all_selected.append(value - 1)
-	
-	return all_selected
 
-def log(text):
-	time = datetime.now()
-	info = time.strftime("%Y-%m-%d %H:%M:%S") + "\t" + text
-	print(info)
-	with open("log.txt","a") as f:
-		f.write(info + "\n")
+	return all_selected
 
-def main():
-	use_config = os.path.exists("cfd-config.json")
+def get_external_ip() -> str:
+	response = requests.get("https://4.ident.me")
+	if response.status_code == 200:
+		return response.text
+	response = requests.get("https://4.tnedi.me/")
+	if response.status_code == 200:
+		return response.text
+	return ""
+
+def main() -> None:
+	if len(sys.argv) > 1 and sys.argv[1] == "logs":
+		print(dirpath)
+		return
 
-	if not use_config:
+	if not os.path.exists(os.path.join(dirpath, "config.json")) or (len(sys.argv) > 1 and  sys.argv[1] == "config"):
 		token = input("API Token: ")
 		try:
 			cf = CloudFlare.CloudFlare(token=token)
 			zones = cf.zones.get()
 		except:
 			print("Invalid API Token")
 			return
-		
+
 		dns_records = []
-  
+
 		for zone in zones:
 			try:
 				temp_dns_records = cf.zones.dns_records.get(zone["id"])
 			except CloudFlare.exceptions.CloudFlareAPIError as e:
-				exit('/zones/dns_records.get %d %s - api call failed' % (e, e))
+				logger.error("/zones/dns_records.get %d %s - api call failed" % (e, e))
+				exit("/zones/dns_records.get %d %s - api call failed" % (e, e))
 
 			temp_dns_records = [i for i in temp_dns_records if i["type"] == "A"]
-   
+
 			for i in range(len(temp_dns_records)):
 				temp_dns_records[i]["zone"] = zone["id"]
-    
+	
 			dns_records += temp_dns_records
-    
-		max_name_length = max([len(i["name"]) for i in dns_records])
+
+		max_name_length = max(map(lambda x: len(x["name"]), dns_records))
 		selected = multi_menu("Select an option: ",[i["name"] + (" " * (max_name_length - len(i["name"]))) + "\t" + i["content"] for i in dns_records])
-		
+
 		selected_dns_records = [dns_records[i] for i in selected]
-  
+
 		zones = []
-  
+
 		for i in selected_dns_records:
 			if not i["zone"] in zones:
 				zones.append(i["zone"])
 
 		delay = intput("Delay between checks in seconds: ")
-    
-		with open("cfd-config.json","w") as f:
-			json.dump({"token": token, "zones": zones, "dns_records": [i["id"] for i in selected_dns_records], "delay": delay}, f)
+
+		selected_dns_records = [i["id"] for i in selected_dns_records]
+
+		with open(os.path.join(dirpath, "config.json"),"w") as f:
+			json.dump({"token": token, "zones": zones, "dns_records": selected_dns_records, "delay": delay}, f)
 
 	else:
-		with open("cfd-config.json","r") as f:
-			config = json.load(f)
-			token = config["token"]
-			zones = config["zones"]
-			selected_dns_records = config["dns_records"]
-			delay = config["delay"]
+		with open(os.path.join(dirpath, "config.json"),"r") as f:
+			CONFIG = json.load(f)
+			token = CONFIG["token"]
+			zones = CONFIG["zones"]
+			selected_dns_records = CONFIG["dns_records"]
+			delay = CONFIG["delay"]
 			cf = CloudFlare.CloudFlare(token=token)
 
 	if delay < 1:
 		delay = 1
 
-	log("")
-	log("[INFO] Program started")
+	logger.info("Program started")
 
-	ip = "Unknown"
+	ip = ""
+	first = True
 	while True:
-		new_ip = requests.get("https://4.ident.me").text
+		new_ip = get_external_ip()
+		if new_ip == "":
+			logger.error("Failed to get external ip, check internet connection")
+			time.sleep(delay * 5)
+			continue
 
 		if ip != new_ip:
-			log(f"[INFO] IP changed from {ip} to {new_ip}")
+			if first:
+				logger.info(f"IP address is {new_ip}")
+				first = False
+			else:
+				logger.info(f"IP changed from {ip} to {new_ip}")
 			ip = new_ip
 
 			for zoneId in zones:
 				try:
 					temp_dns_records = cf.zones.dns_records.get(zoneId)
 				except CloudFlare.exceptions.CloudFlareAPIError as e:
-					log(f"[ERROR] Failed to fetch dns records for {zoneId}")
+					string = f"Failed to fetch dns records for {zoneId}\n" + "/zones/dns_records.get %d %s - api call failed" % (e, e)
+					logger.error(string)
+					continue
 				
 				for dns_record in temp_dns_records:
 					if dns_record["id"] in selected_dns_records and dns_record["content"] != ip:
 						dns_record["content"] = ip
 						cf.zones.dns_records.put(zoneId, dns_record["id"], data=dns_record)
-						log(f"[INFO] Updated record for {dns_record['name']}")
+						logger.info(f"Updated record for {dns_record['name']}")
 
 		time.sleep(delay)
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
 	main()
```

