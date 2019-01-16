
## MCSC 2019 Binary Exploitation Challenges
>thinbashane < @art0flunam00n >

**1.pwn50**

Description 
 - get the flag ! pwn50.c is here

Flag
 - `MCSC_2019{v4riabl3_0v3rwrite3_b0f}`

Setting up
 - `cd pwn50` - change directory to the challenge
 - `docker build -t pwn50 .` - build from Dockerfile
 - `docker run -p 1337:1337 pwn50` - run docker containter
 - `nc <server_ip> 1337` - Challenge Access 

Writeup
 - releases after competition
---
**2.pwn100a**

Description
 - Read the fl4g file
 - ssh credentials ( username = luna & password = luna )

Flag
 - `MCSC_2019{r4c3_c0nditi0n_15_fuN}`

Setting up
 - `cd pwn100a` - change directory to the challenge
 - `docker build -t pwn100a .` - build from Dockerfile
 - `docker run -p 22:22 pwn100a` - run docker containter
 - `ssh luna@<server_ip>` & `password = luna` - Challenge Access SSH

Writeup
 - releases after competition

---


