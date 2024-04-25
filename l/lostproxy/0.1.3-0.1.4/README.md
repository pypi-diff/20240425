# Comparing `tmp/lostproxy-0.1.3.tar.gz` & `tmp/lostproxy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lostproxy-0.1.3.tar", last modified: Sun Mar 31 13:29:32 2024, max compression
+gzip compressed data, was "lostproxy-0.1.4.tar", last modified: Thu Apr 25 16:47:12 2024, max compression
```

## Comparing `lostproxy-0.1.3.tar` & `lostproxy-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 13:29:32.182992 lostproxy-0.1.3/
--rw-rw-rw-   0        0        0     1466 2024-03-31 13:29:32.181992 lostproxy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1096 2024-03-30 15:33:14.000000 lostproxy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 13:29:32.171992 lostproxy-0.1.3/lostproxy/
--rw-rw-rw-   0        0        0       21 2024-03-31 13:26:36.000000 lostproxy-0.1.3/lostproxy/__init__.py
--rw-rw-rw-   0        0        0    14763 2024-03-31 13:25:35.000000 lostproxy-0.1.3/lostproxy/lostproxy.py
-drwxrwxrwx   0        0        0        0 2024-03-31 13:29:32.180992 lostproxy-0.1.3/lostproxy.egg-info/
--rw-rw-rw-   0        0        0     1466 2024-03-31 13:29:31.000000 lostproxy-0.1.3/lostproxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-03-31 13:29:32.000000 lostproxy-0.1.3/lostproxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 13:29:31.000000 lostproxy-0.1.3/lostproxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-03-31 13:29:31.000000 lostproxy-0.1.3/lostproxy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-03-31 13:29:31.000000 lostproxy-0.1.3/lostproxy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 13:29:32.183993 lostproxy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      746 2024-03-31 13:26:27.000000 lostproxy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:47:12.279602 lostproxy-0.1.4/
+-rw-rw-rw-   0        0        0     1572 2024-04-25 16:47:12.278603 lostproxy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1202 2024-04-25 16:44:29.000000 lostproxy-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:47:12.269601 lostproxy-0.1.4/lostproxy/
+-rw-rw-rw-   0        0        0       21 2024-04-25 16:46:42.000000 lostproxy-0.1.4/lostproxy/__init__.py
+-rw-rw-rw-   0        0        0    20089 2024-04-25 16:42:01.000000 lostproxy-0.1.4/lostproxy/lostproxy.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:47:12.277602 lostproxy-0.1.4/lostproxy.egg-info/
+-rw-rw-rw-   0        0        0     1572 2024-04-25 16:47:12.000000 lostproxy-0.1.4/lostproxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-04-25 16:47:12.000000 lostproxy-0.1.4/lostproxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:47:12.000000 lostproxy-0.1.4/lostproxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-25 16:47:12.000000 lostproxy-0.1.4/lostproxy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 16:47:12.000000 lostproxy-0.1.4/lostproxy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:47:12.279602 lostproxy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      746 2024-04-25 16:46:39.000000 lostproxy-0.1.4/setup.py
```

### Comparing `lostproxy-0.1.3/PKG-INFO` & `lostproxy-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: lostproxy
-Version: 0.1.3
-Summary: A multifunctional python proxy
-Author: Joseph
-Author-email: josephdove@proton.me
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # LostProxy
 
 LostProxy is a multi functional proxy for the HTTP, Socks4/4a and Socks5/5h protocols all in one port.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install lostproxy.
@@ -21,29 +9,30 @@
 ```bash
 pip install lostproxy
 ```
 
 ## Usage
 
 ```bash
-usage: lostproxy [-h] [-l LISTENER] [-u USER] [-p PASSWORD] [-a]
+usage: lostproxy [-h] [-l LISTENER] [-u USER] [-p PASSWORD] [-a] [-v]
 
 A multi functional proxy for HTTP, Socks4/4a and Socks5/5h all in one port.
 
 options:
   -h, --help            show this help message and exit
   -l LISTENER, --listener LISTENER
                         Listening address, example: 0.0.0.0:8080
   -u USER, --user USER  (OPTIONAL) Username for auth, example: Jack
   -p PASSWORD, --password PASSWORD
                         (OPTIONAL) Password for auth, example: Password123
   -a, --allow_localhost
                         (OPTIONAL) Allows localhost and other internal IP ranges.
+  -v, --verbose         (OPTIONAL) Displays information about connections and what site they visit.
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 ## License
 
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `lostproxy-0.1.3/lostproxy/lostproxy.py` & `lostproxy-0.1.4/lostproxy/lostproxy.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Initialize libraries
 parser = argparse.ArgumentParser(description = "A multi functional proxy for HTTP, Socks4/4a and Socks5/5h all in one port.")
 
 parser.add_argument("-l", "--listener", help = "Listening address, example: 0.0.0.0:8080")
 parser.add_argument("-u", "--user", help = "(OPTIONAL) Username for auth, example: Jack")
 parser.add_argument("-p", "--password", help = "(OPTIONAL) Password for auth, example: Password123")
 parser.add_argument("-a", "--allow_localhost", help="(OPTIONAL) Allows localhost and other internal IP ranges.", action="store_true")
+parser.add_argument("-v", "--verbose", help="(OPTIONAL) Displays information about connections and what site they visit.", action="store_true")
 
 args = parser.parse_args()
 
 # Static variables
 PACKET_BUFFER = 65537
 BAD_HEADERS = [
 	b"proxy-authenticate",
@@ -60,15 +61,15 @@
 		(parts[0] == 192 and parts[1] == 168) or
 		(parts[0] == 127)):
 		return True
 
 	return False
 
 class HTTPConnection():
-	def __init__(self, server_config, init_packet, client_socket):
+	def __init__(self, server_config, init_packet, client_socket, client_address):
 		# Parse the initial packet
 
 		split_packet = init_packet.split(b"\r\n\r\n")
 
 		self.data = split_packet[1]
 
 		packet_lines = split_packet[0].split(b"\r\n")
@@ -97,68 +98,113 @@
 			# Can't connect because the host header wasn't found, close the socket
 			client_socket.send(b"HTTP/1.1 502 Bad Gateway\r\n\r\n")
 			client_socket.close()
 			return
 
 		# Handle authentication
 		if server_config.should_authenticate:
+			self.has_authenticated = False
 			for header in self.headers:
 				if header.lower() == b"proxy-authorization":
 					# Only support BASIC authentication
 					if not self.headers[header].startswith(b"Basic "):
 						client_socket.send(b"HTTP/1.1 405 Method Not Allowed\r\n\r\n")
 						client_socket.close()
+
+						# Log authentication failure
+						if server_config.is_verbose:
+							print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+"'s request failed due to a disallowed authentication method.")
+
 						return
 
 					# Decode the authentication token and compare it to username and password
 					authentication_token = self.headers[header].split(b" ")[1]
 
 					self.username, self.password = base64.b64decode(authentication_token).decode("utf-8").split(":")
 
 					if (self.username, self.password) != server_config.authentication_parameters:
 						client_socket.send(b"HTTP/1.1 401 Unauthorized\r\n\r\n")
 						client_socket.close()
+
+						# Log authentication failure
+						if server_config.is_verbose:
+							print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+'\'s request failed due to wrong authentication (passed in "'+self.username+":"+self.password+'").')
+
 						return
+					else:
+						self.has_authenticated = True
+
+			if not self.has_authenticated:
+				client_socket.send(b"HTTP/1.1 401 Unauthorized\r\n\r\n")
+				client_socket.close()
+
+				# Log authentication failure
+				if server_config.is_verbose:
+					print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+"'s request failed due to wrong authentication (no authentication header passed in).")
+
+				return
 
 		if self.method == b"CONNECT":
 			# Handle HTTPS/TCPIP requests
 
 			host_address_split = self.host_address.split(b":")
 
 			self.host_address = host_address_split[0].decode("utf-8")
 			self.requested_port = int(host_address_split[1])
 
+			# Log connection request
+			if server_config.is_verbose:
+				print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+" requested connection to "+self.host_address+":"+str(self.requested_port))
+
 			# Resolve domain
 			self.ip_address = socket.gethostbyname(self.host_address)
 			self.ip_bytes = socket.inet_aton(self.ip_address)
 
 			# Do not allow localhost connections unless specified
 			if not server_config.allow_localhost and is_ip_local(self.ip_address):
 				client_socket.send(b"HTTP/1.1 502 Bad Gateway\r\n\r\n")
 				client_socket.close()
+
+				# Log connection failure
+				if server_config.is_verbose:
+					print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.url+" failed due to local domain disallowance.")
+
 				return
 
 			# Create socket to server
 			try:
 				server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 				server_socket.connect((self.ip_address, self.requested_port))
 			except:
 				# Connection failed
 				client_socket.send(b"HTTP/1.1 502 Bad Gateway\r\n\r\n")
 				client_socket.close()
+
+				# Log connection failure due to localhost check
+				if server_config.is_verbose:
+					print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.url+" failed due to local domain disallowance.")
+
 				return
 
 			# Send a successful response
 			client_socket.send(b"HTTP/1.1 200 Connection established\r\nConnection: keep-alive\r\n\r\n")
 
+			# Log connection acceptance
+			if server_config.is_verbose:
+				print("[HTTP] Accepted "+client_address[0]+":"+str(client_address[1])+"'s connection request to "+self.host_address+":"+str(self.requested_port))
+
 			# Relay the connection
 			relay_connection(client_socket, server_socket)
 		else:
 			# Handle HTTP requests
 
+			host_address_split = self.host_address.split(b":")
+
+			self.host_address = host_address_split[0].decode("utf-8")
+
 			# Get the protocol, if there isn't any, default to HTTP
 			url_position = self.url.find(b"://")
 			if (url_position == -1):
 				url_no_protocol = self.url
 			else:
 				url_no_protocol = self.url[(url_position+3):]
 			
@@ -177,34 +223,52 @@
 			self.filtered_headers = self.headers.copy()
 
 			for bad_header in BAD_HEADERS:
 				for header in self.headers:
 					if header.lower() == bad_header:
 						del self.filtered_headers[header]
 
+			# Log connection request
+			if server_config.is_verbose:
+				print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+" requested "+self.url.decode("utf-8"))
+
 			# Resolve domain
 			self.ip_address = socket.gethostbyname(self.host_address)
 			self.ip_bytes = socket.inet_aton(self.ip_address)
 
 			# Do not allow localhost connections unless specified
 			if not server_config.allow_localhost and is_ip_local(self.ip_address):
 				client_socket.send(b"HTTP/1.1 502 Bad Gateway\r\n\r\n")
 				client_socket.close()
+
+				# Log connection failure due to localhost check
+				if server_config.is_verbose:
+					print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.url.decode("utf-8")+" failed due to local domain disallowance.")
+
 				return
 
 			# Create socket to server
 			try:
 				server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 				server_socket.connect((self.host_address, self.requested_port))
 			except:
 				# Connection failed
 				client_socket.send(b"HTTP/1.1 502 Bad Gateway\r\n\r\n")
 				client_socket.close()
+
+				# Log connection failure
+				if server_config.is_verbose:
+					print("[HTTP] Client "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.url.decode("utf-8")+" failed due to connection rejection from server.")
+
 				return
 
+			# Log connection acceptance
+			if server_config.is_verbose:
+				print("[HTTP] Accepted "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.url.decode("utf-8"))
+
 			# Send method, url location and version
 			server_socket.send(b" ".join([self.method, self.url_location, self.http_version]) + b"\r\n")
 
 			# Send filtered headers
 			for header in self.filtered_headers:
 				server_socket.send(header + b": " + self.filtered_headers[header] + b"\r\n")
 
@@ -212,15 +276,15 @@
 			server_socket.send(b"\r\n" + self.data)
 
 			# Relay the connection
 			relay_connection(client_socket, server_socket)
 
 
 class Socks4Connection():
-	def __init__(self, server_config, init_packet, client_socket):
+	def __init__(self, server_config, init_packet, client_socket, client_address):
 		# Parse the initial packet
 
 		self.version = init_packet[0]
 		self.command = init_packet[1]
 		self.requested_port = init_packet[2] * 256 + init_packet[3]
 		self.requested_port_bytes = init_packet[2:4]
 		self.user_id = init_packet[8:].split(b'\x00', 1)[0].decode("utf-8")
@@ -234,53 +298,75 @@
 
 			# Resolve domain
 			self.ip_address = socket.gethostbyname(self.domain_name)
 			self.ip_bytes = socket.inet_aton(self.ip_address)
 
 		# Handle authentication
 		if server_config.should_authenticate and self.user_id.split("***") != list(server_config.authentication_parameters):
+			# Log authentication failure
+			if server_config.is_verbose:
+				print("[SOCKS4] Client "+client_address[0]+":"+str(client_address[1])+'\'s request failed due to wrong authentication (passed in "'+self.user_id+'").')
+
 			client_socket.send(b"\x00\x5D")
 			client_socket.close()
 			return
 
 		# Handle local IP blocking
 		if not server_config.allow_localhost and is_ip_local(self.ip_address):
+			# Log connection failure due to localhost check
+			if server_config.is_verbose:
+				print("[SOCKS4] Client "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.ip_address+":"+str(self.requested_port)+" failed due to local domain disallowance.")
+			
 			client_socket.send(b"\x00\x5B")
 			client_socket.close()
 			return
 
 		# Create socket to server
 		try:
 			server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 			server_socket.connect((self.ip_address, self.requested_port))
 		except:
 			# Connection failed
 			client_socket.send(b"\x00\x5B")
 			client_socket.close()
+
+			# Log connection failure
+			if server_config.is_verbose:
+				print("[SOCKS4] Client "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.ip_address+":"+str(self.requested_port)+" failed due to connection rejection from server.")
+
 			return
 
 		# Send success response and start relaying the connection
 		client_socket.send(b"\x00\x5A" + self.requested_port_bytes + self.ip_bytes)
 
+		# Log connection acceptance
+		if server_config.is_verbose:
+			print("[SOCKS4] Accepted "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.__dict__.get("domain_name", self.ip_address)+":"+str(self.requested_port))
+
 		relay_connection(client_socket, server_socket)
 
 class Socks5Connection():
-	def __init__(self, server_config, init_packet, client_socket):
+	def __init__(self, server_config, init_packet, client_socket, client_address):
 		# Parse the initial packet
 
 		self.version = init_packet[0]
 		self.number_of_authentication_methods = init_packet[1]
 		self.authentication_methods = init_packet[2:2+self.number_of_authentication_methods]
 
 		# Handle authentication
 		if server_config.should_authenticate:
 			# If client doesn't support authentication through user and password, reject the connection
 			if 0x02 not in self.authentication_methods:
 				client_socket.sendall(b'\x05\xff')
 				client_socket.close()
+
+				# Log authentication failure
+				if server_config.is_verbose:
+					print("[SOCKS5] Client "+client_address[0]+":"+str(client_address[1])+'\'s request failed due to no authentication methods.')
+
 				return
 
 			# Continue with authentication
 			client_socket.sendall(b'\x05\x02')
 
 			self.authentication_packet = client_socket.recv(PACKET_BUFFER)
 
@@ -295,14 +381,19 @@
 			self.username = self.authentication_packet[2:2+username_length].decode("utf-8")
 			self.password = self.authentication_packet[3+username_length:3+username_length+password_length].decode("utf-8")
 
 			if (self.username, self.password) != server_config.authentication_parameters:
 				# Authentication failed
 				client_socket.sendall(b'\x01\x01')  # 0x01 version of the subnegotiation, 0x01 authentication failure
 				client_socket.close()
+
+				# Log authentication failure
+				if server_config.is_verbose:
+					print("[SOCKS5] Client "+client_address[0]+":"+str(client_address[1])+'\'s request failed due to wrong authentication (passed in "'+self.username+":"+self.password+'").')
+
 				return
 
 			# Authentication successful
 			client_socket.sendall(b'\x01\x00')
 		else:
 			# No authentication
 			client_socket.sendall(b'\x05\x00')
@@ -325,28 +416,37 @@
 			self.ip_bytes = self.address_packet[4:8]
 			self.ip_address = socket.inet_ntoa(self.ip_bytes)
 			self.requested_port_bytes = self.address_packet[-2:]
 			self.requested_port = self.address_packet[-2] * 256 + self.address_packet[-1]
 		elif self.address_type == 3:
 			# Address is a domain name, get it
 			domain_size = self.address_packet[4]
-			self.domain_name = self.address_packet[5:5+domain_size]
+			self.domain_name = self.address_packet[5:5+domain_size].decode("utf-8")
 
 			# And finally, resolve it
 			self.ip_address = socket.gethostbyname(self.domain_name)
 			self.ip_bytes = socket.inet_aton(self.ip_address)
 			self.requested_port_bytes = self.address_packet[-2:]	
 			self.requested_port = self.address_packet[-2] * 256 + self.address_packet[-1]
 		else:
 			# Address type is not support (IPV6, etc), close connection
+
+			# Log protocol failure
+			if server_config.is_verbose:
+				print("[SOCKS5] Client "+client_address[0]+":"+str(client_address[1])+'\'s request failed due to request not being supported.')
+
 			client_socket.close()
 			return
 
 		# Do not allow localhost connections unless specified
 		if not server_config.allow_localhost and is_ip_local(self.ip_address):
+			# Log connection failure due to localhost check
+			if server_config.is_verbose:
+				print("[SOCKS5] Client "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.ip_address+":"+str(self.requested_port)+" failed due to local domain disallowance.")
+
 			client_socket.close()
 			return
 
 		# Create socket to server
 		try:
 			server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 			server_socket.connect((self.ip_address, self.requested_port))
@@ -354,14 +454,18 @@
 			# Connection failed
 			client_socket.close()
 			return
 
 		# Send success response and start relaying the connection
 		client_socket.send(b"\x05\x00\x00\x01" + self.ip_bytes + self.requested_port_bytes)
 
+		# Log connection acceptance
+		if server_config.is_verbose:
+			print("[SOCKS5] Accepted "+client_address[0]+":"+str(client_address[1])+"'s request to "+self.__dict__.get("domain_name", self.ip_address)+":"+str(self.requested_port))
+
 		relay_connection(client_socket, server_socket)
 
 class MultiProxyServer:
 	http_methods_bytes = [
 		b"GET",
 		b"HEAD",
 		b"POST",
@@ -369,41 +473,46 @@
 		b"DELETE",
 		b"CONNECT",
 		b"OPTIONS",
 		b"TRACE",
 		b"PATCH"
 	]
 
-	def __init__(self, allow_localhost, authentication_parameters=None):
+	def __init__(self, allow_localhost, is_verbose, authentication_parameters=None):
 		self.allow_localhost = allow_localhost
+		self.is_verbose = is_verbose
 		self.should_authenticate = authentication_parameters != (None, None)
 		self.authentication_parameters = authentication_parameters
 
 	def connection_thread(self, conn, addr):
+		if self.is_verbose:
+			print("[INFO] New connection from "+addr[0]+":"+str(addr[1]))
+
 		try:
 			# Get the first packet and analyze what type of proxy it is
 
 			firstPacket = conn.recv(PACKET_BUFFER)
 
 			if firstPacket.split(b" ",1)[0] in self.http_methods_bytes:
 				# Handle HTTP
 
-				HTTPConnection(self, firstPacket, conn)
+				HTTPConnection(self, firstPacket, conn, addr)
 			elif firstPacket[0] == 0x04:
 				# Handle Socks4/4a
 
-				Socks4Connection(self, firstPacket, conn)
+				Socks4Connection(self, firstPacket, conn, addr)
 			elif firstPacket[0] == 0x05:
 				# Handle Socks5/5h
 
-				Socks5Connection(self, firstPacket, conn)
+				Socks5Connection(self, firstPacket, conn, addr)
 			else:
 				# We don't know the protocol used, raise an exception
 				raise Exception("No known protocol used.")
-		except:
+		except Exception as e:
+			print(e)
 			# Suppress errors
 			pass
 
 	def start(self, host, port):
 		sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 		sock.bind((host, port))
 		sock.listen()
@@ -447,11 +556,11 @@
 	if args.user != None and args.password != None:
 		print("[WARNING] Socks4/4a doesn't support USER:PASS authentication, the username and password will be split by \"***\", so for example you would connect as socks4://username***password@IP:PORT.")
 
 	# Start the CTRL+C handler
 	threading.Thread(target=controlc_handler).start()
 
 	# Start the server
-	MultiProxyServer(args.allow_localhost, authentication_parameters=(args.user, args.password)).start(host, port)
+	MultiProxyServer(args.allow_localhost, args.verbose, authentication_parameters=(args.user, args.password)).start(host, port)
 
 if __name__ == '__main__':
 	run()
```

### Comparing `lostproxy-0.1.3/lostproxy.egg-info/PKG-INFO` & `lostproxy-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lostproxy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A multifunctional python proxy
 Author: Joseph
 Author-email: josephdove@proton.me
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -21,27 +21,28 @@
 ```bash
 pip install lostproxy
 ```
 
 ## Usage
 
 ```bash
-usage: lostproxy [-h] [-l LISTENER] [-u USER] [-p PASSWORD] [-a]
+usage: lostproxy [-h] [-l LISTENER] [-u USER] [-p PASSWORD] [-a] [-v]
 
 A multi functional proxy for HTTP, Socks4/4a and Socks5/5h all in one port.
 
 options:
   -h, --help            show this help message and exit
   -l LISTENER, --listener LISTENER
                         Listening address, example: 0.0.0.0:8080
   -u USER, --user USER  (OPTIONAL) Username for auth, example: Jack
   -p PASSWORD, --password PASSWORD
                         (OPTIONAL) Password for auth, example: Password123
   -a, --allow_localhost
                         (OPTIONAL) Allows localhost and other internal IP ranges.
+  -v, --verbose         (OPTIONAL) Displays information about connections and what site they visit.
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 ## License
```

### Comparing `lostproxy-0.1.3/setup.py` & `lostproxy-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
 	name='lostproxy',
-	version='0.1.3',
+	version='0.1.4',
 	author='Joseph',
 	author_email='josephdove@proton.me',
 	description='A multifunctional python proxy',
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
 	classifiers=[
 		'Programming Language :: Python :: 3.10',
```

