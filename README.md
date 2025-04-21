# Metasploit-for-reconnaissance
## Name: Shanmuga Raj.K
## Reg num: 212223040192
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system
## OUTPUT:

![img 1](https://github.com/user-attachments/assets/6a1704b0-94c2-4445-9917-c3683804e3fe)


Invoke msfconsole:
## OUTPUT:

![img2](https://github.com/user-attachments/assets/2cee9806-dcd2-403a-8cf3-e7dbb3e44d3e)



Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

## OUTPUT:
![img3](https://github.com/user-attachments/assets/9fb1b7c1-037d-4558-8033-f017f5b94149)
![img4](https://github.com/user-attachments/assets/ed4c4a8d-11a7-4e79-a8c6-977741fec6a1)
![img5](https://github.com/user-attachments/assets/ed93f1c8-4a8d-4838-8cf4-87abbba9b7fe)
![img6](https://github.com/user-attachments/assets/69928b8a-4423-45ef-9749-b0579f122fad)
![img7](https://github.com/user-attachments/assets/f584c680-70d2-4e82-8a43-2fbf38cb88c3)

Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).
msf >  nmap -sT 192.168.228.34/24 -p1-1000
## OUTPUT:
![img8](https://github.com/user-attachments/assets/7320010e-a784-4c74-9eb9-c9a3a2251c83)


use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.
msf > db_nmap 192.168.228.34/24
## OUTPUT:
![img9](https://github.com/user-attachments/assets/61da3931-9b29-4075-ad81-69fb16466d7a)
![img10](https://github.com/user-attachments/assets/32339c45-5b51-437f-be41-3f48acd70358)

Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules.
cd /usr/share /metasploit-framework/modules/auxiliary
kali > ls -l
## OUTPUT:
![img11](https://github.com/user-attachments/assets/80b98afd-13ab-42bb-bd31-54d33d7d2a3c)


Search is a powerful command in Metasploit that you can use to find what you want to locate. 
msf >search name:Microsoft type:exploit
## OUTPUT:
![img12](https://github.com/user-attachments/assets/26fd3087-ffbf-4d9c-a19e-cfa7aadc484e)



The info command provides information regarding a module or platform,
## OUTPUT:
![img 13](https://github.com/user-attachments/assets/30e7b566-1e2f-4dd3-9378-53f4ac9ef3d3)

##MYSQL ENUMERATION
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port.
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
## OUTPUT:
![img 14](https://github.com/user-attachments/assets/ddad1035-e7c2-4c76-9532-80c68a4d6a20)
![img 15](https://github.com/user-attachments/assets/7ba32698-049c-45b3-8187-9b7be47db3a0)
![img16](https://github.com/user-attachments/assets/dfce3f8f-26cc-4c01-b5c9-80e4dd7191b9)
![img17](https://github.com/user-attachments/assets/9affd3bc-9654-4b5e-826d-39b0517df86e)


## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
