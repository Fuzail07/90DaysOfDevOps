 what happens when you type google.com in a browser?
 the browser finds ip address linked with the DNS google.com after finding it send syncronization packets and after recieving acknowledgement from the server browser displays its webpage.

 Types of records:
 A record : links with the IPV4
 AAAA record : links with IPV6
 CName record : links with another dns like www.google.com to google.com
 MX record : it redirects to a specified mail server.
 NS record : tells the internet where to find your website.

 What is an IPv4 address? How is it structured?
 It is a protocol which is assigned to every device which is connected to the network
 It is a 32-bit address each dot derived as octate Eg: 192.168.0.1 

 Difference between public and private IPs ?
 with the help of public ip you can access to the internet. eg  92.242.225.44
 with private ip you can only communicate within the connected nodes not internet. eg: 172.168.52.22

 CIDR & Subnetting 
 What does /24 mean in 192.168.1.0/24?
 it is a cidr notation which means first 24bit wont change.

 How many usable hosts in a /24? A /16? A /28?
 /24 -- 256 usable
 /16 -- 65000 
 /28 -- 16

 why do we subnet?
 Because public ip is less for whole world so we use subnet to overcome with the limitation.
