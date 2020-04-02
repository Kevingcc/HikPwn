# HikPwn
HikPwn, a simple scanner for Hikvision devices with basic vulnerability scanning capabilities written in Python 3.8.
This project was born out of curiosity while I was capturing and watching network traffic generated by some Hikvision's software and devices.

### Setup instructions:
```
git clone https://github.com/4n4nk3/HikPwn.git
cd HikPwn
pip install -r requirements.txt
```

### Tested on:
 - [x] Python 3.8 on Linux 4.19 x86_64

### Functions and characteristics:
 - [x] Passive discovery of Hikvision devices.
 - [x] Active discovery and enumeration of Hikvision devices via UDP probing.

 > Work in progress... stay tuned!
 
#### TODO:

* Add detection and exploitation capabilities for ICSA-17-124-01.

### Help:
```
usage: hikpwn.py [-h] --interface INTERFACE --address ADDRESS [--active]

HikPwn, a simple scanner for Hikvision devices with basic vulnerability scanning capabilities written in Python 3.8. by Ananke: https://github.com/4n4nk3.

optional arguments:
  -h, --help            show this help message and exit
  --interface INTERFACE the network interface to use
  --address ADDRESS     the ip address of the selected network interface
  --active              enable "active" discovery
```

### Censored preview:
```
Using eth0 as network interface and XXX.XXX.XXX.XXX as its IP address...

[*] Started 30 seconds of both passive and active discovery...

[*] Active discovery's results:

DEVICE #1:
	LABEL                     DATA      
	--------------------------------------------------
	Serial Number             xxxxxxxxxxxxxxxxxxxxx
	Description               DS-2DE4220IW-D
	MAC                       XX-XX-XX-XX-XX-XX
	IP                        XXX.XXX.XXX.XX
	DHCP in use               false     
	Software Version          V5.4.3build 160810
	DSP Version               V7.3 build 160801
	Boot Time                 2019-03-01 00:05:33
	Activation Status         true      
	Password Reset Ability    true      


[*] Passive discovery didn't find any device.
```

**_This project is for educational purposes only. Don't use it for illegal activities. I don't support nor condone illegal or unethical actions and I can't be held responsible for possible misuse of this software._**