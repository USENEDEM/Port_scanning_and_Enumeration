# Port_scanning_and_Enumeration
___
### Preview
___

This project is a life simulation of port scanning and Enumeration using NMAP to identify open ports and services available on a network host. Showcasing the process of extracting machine names, network resources(Enumeration) etc as part of reconaissance procedures used in computer/system audit.

### Skills (*Learned*)
___

*Bullet point*

1. Port scanning using NMAP
2. Reconaissance
3. system/computer auditing

### Tools
___

1. Metasploitable 2 - Vulnerable machine [Download Here](Https://www.vulhub.com)
2. NMAP - Network scanner
3. HIIT plc - website/Webpage
N/B: Seek permission from the webpage/website owner for this exercise like i did.

### Procedure 
___

1. Start up NMAP on Kali linux by selecting NMAP from the application list or running the command
```zsh
sudo nmap
```



<img width="1280" alt="Screenshot 2024-06-13 at 12 19 22" src="https://github.com/USENEDEM/Port_scanning_and_Enumeration/assets/169564406/0a8aac7a-09d4-46a8-ae4c-8186206ebabc">


*Ref 1.* (starting up NMAP)

on the terminal 

2. I ran a syn stealth scan command on my linux terminal 
```zsh
nmap -sS <domain name>
```
and same command using metasploitable 2 <*ip address*> to locate open port.


<img width="1280" alt="Screenshot 2024-06-13 at 12 24 13" src="https://github.com/USENEDEM/Port_scanning_and_Enumeration/assets/169564406/a631c54b-7b5f-412f-80ed-fa9788310c06">



<img width="1280" alt="Screenshot 2024-06-13 at 23 35 09" src="https://github.com/USENEDEM/Port_scanning_and_Enumeration/assets/169564406/290df83a-63a7-492d-8763-cdb4861e8478">




*Ref 2.* (NMAP syn stealth scan on webpage(1) metasploitable 2 *IP* (2). 

3. I used a fragmented scan
```zsh
 nmap -f<domain name>
```
to probe packet in small *ip* fragment. This split the TCP header over several packets to make it harder to be detected by firewall in order to bypass packet filters.



<img width="1280" alt="Screenshot 2024-06-13 at 12 33 34" src="https://github.com/USENEDEM/Port_scanning_and_Enumeration/assets/169564406/9e259b41-5a30-4128-abdf-9fa8f1573fad">




*Ref.* 3 (nmap fragmented scan) 

4. Ran a *ICMP* Echo request to specified host to be certain host are up.



<img width="1280" alt="Screenshot 2024-06-13 at 14 29 22" src="https://github.com/USENEDEM/Port_scanning_and_Enumeration/assets/169564406/6b11d733-63d4-4281-89c6-e6f97689805d">


*Ref.* 4 (ICMP Echo request using NMAP) 

5. Ran a version detection scan to collect information about specific service running on a open port.



<img width="1280" alt="Screenshot 2024-06-13 at 14 32 33" src="https://github.com/USENEDEM/Port_scanning_and_Enumeration/assets/169564406/f1b3b0f2-2bdb-4ee9-8496-16c535743706">



*Ref.* 5 (Version detection scan)

6. I ran an OS fingerprinting scan using nmap on verbose mode to get more detailed information about the scan.
command for scan
```zsh
nmap -o <domain name>
```


<img width="1280" alt="Screenshot 2024-06-13 at 14 35 40" src="https://github.com/USENEDEM/Port_scanning_and_Enumeration/assets/169564406/d73df1c4-71b1-4385-92fb-6fb2ee778df9">


*Ref.* 6 (NMAP fingerprinting scan)
