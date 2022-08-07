In static routing, routers only know about directly connected routes. Every other network must be manually configued. R1 can be configured with following routes
- 192.168.100.196 255.255.255.252 192.168.100.193
- 192.168.100.64 255.255.255.192 192.168.100.193
- 192.168.100.196 255.255.255.252 192.168.100.193

Since every route has the same next hop, its not required to setup routes one by one. Instead we can set default route to make it simple as
- 0.0.0.0 0.0.0.0 192.168.100.193

This is a one usecase of default static routing. Same thing goes with R3
