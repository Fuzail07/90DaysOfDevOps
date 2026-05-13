Map the OSI vs TCP/IP models :

OSI Model (Open System Interconnection ) THis is a theoratical concept.

Application - where you can communicate with other node.
Presentation - end to end encryption
Session - maintains a session to connect
Transport - tcp protocol
Network - routing and addresses
Data Link - physical addresses
Physical - connect using cables and routers

TCP/IP Model : Practical implementation of the OSI model

combination of Application, Presentation and session layer is called application layer and datalink and physical is called network access in TCP/IP model

Application layer 
Transport layer 
Internet layer
Network access layer


Hands-on Checklist 
Identity: hostname -I (172.31.30.224)

Reachability: ping 8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=117 time=1.04 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=117 time=1.06 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=117 time=1.06 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=117 time=1.06 ms
64 bytes from 8.8.8.8: icmp_seq=5 ttl=117 time=1.07 ms

Path: traceroute www.google.com -- it hops 30 times with 0.5ms it seems normal no spikes at all.

Ports: ss -tulpn -- listenening all tcp and udp ports one of it is 323.

Name resolution: nslookup www.google.com 
Server:         127.0.0.53
Address:        127.0.0.53#53

HTTP check: curl -I www.trainwithshubham.com

HTTP/1.1 301 Moved Permanently
Server: openresty
Date: Wed, 13 May 2026 19:42:14 GMT
Content-Type: text/html
Content-Length: 166
Connection: keep-alive
Location: https://www.trainwithshubham.com/
Strict-Transport-Security: max-age=31536000; includeSubDomains;
Permissions-Policy: geolocation=(self), microphone=*, camera=*
Referrer-Policy: strict-origin-when-cross-origin
X-Content-Type-Options: nosniff
X-Frame-Options: ALLOW-FROM *

<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>openresty</center>
</body>
</html>

Connections snapshot: netstat -an | head 


