https://docs.packetriot.com/

step 0   => set envirnment path

step 1   => pktriot.exe

step 3   =>  pktriot.exe configure

step 4   => select [option] = 1;

step 5   => login in with pktriot web id and pwd.


Choose the region for the edge server to connect to:
+------------------------+
| #   | Region           |
+------------------------+
| 1   | us-west          |
+------------------------+
| 2   | us-east          |
+------------------------+
| 3   | asia-southeast   |
+------------------------+
| 4   | australia        |
+------------------------+
| 5   | us-south         |
+------------------------+
| 6   | asia-south       |
+------------------------+
| 7   | africa-south     |
+------------------------+

select =>  (4):



Tunnel configuration:
  Hostname: vigilant-wind-64541.pktriot.net
  Server: australia-32312.packetriot.net
  IPv4: 139.180.171.110
  IPv6: <nil>

Start the tunnel and visit URL to check its working:
  pktriot --config C:\Users\surya\.pktriot\config.json start
  https://vigilant-wind-64541.pktriot.net

Detailed help and step-by-step tutorials:
  https://docs.packetriot.com
  https://packetriot.com/tutorials.

Need more support?
  Email: support@packetriot.com
  Twitter: @packetriot (please follow us, we like new friends :)
  
  
  
 _________________________________________________________________________
 
 CHANGING TUNNEL NAME :+
 C:\Users\surya>pktriot.exe edit --name "surya_tunnel"
Tunnel name updated

xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx


C:\Users\surya>pktriot.exe tunnel http add --domain  vigilant-wind-64541.pktriot.net --destination localhost --http 80 l
etsencrypt

HTTP/S traffic rule added

C:\Users\surya>pktriot.exe info
Client:
        Hostname: vigilant-wind-64541.pktriot.net
        Server: australia-32312.packetriot.net
        IPv4: 139.180.171.110
        IPv6: <nil>

HTTP services:
+---------------------------------------------------------------------------------------------------------+
| Domain                            | Destination   | HTTP   | TLS   | Secure   | Protect   | Site Root   |
+---------------------------------------------------------------------------------------------------------+
| vigilant-wind-64541.pktriot.net   | localhost     | 80     | 0     | true     |           | --          |
+---------------------------------------------------------------------------------------------------------+

