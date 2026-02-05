these scans were performed in a home lab .

![img](https://github.com/sunandasinghh/nmap-network-troubleshooting/blob/d693fc9a6748f63d5041a6849adc1de009f3293c/add/basicscan.png)


📌 SCAN 1: PORT SCANNING

COMMAND USED: nmap<targetip>

The objective of scan was to see if there were any ports open.

RESULT: There was one open port.

port no 22 tcp (service:ssh)


![img](https://github.com/sunandasinghh/nmap-network-troubleshooting/blob/d7d2f20883e1ef52633cbb368048b60f6b18d106/add/nmapbasic.png)



📌SCAN 2: SERVICE DETECTION

COMMAND USED: nmap -sV <targetip>

The objective of the scan was to see which sevice the device is running and to see possibe software version.

RESULT: There was one ssh port open and we can see the version of operating system and which operating system is running.



📌SCAN 3: FIREWALL BLOCKS

COMMAND USED: nmap -Pn <targetip>

The objecctive was to see if there is a firewall applied to the network.

RESULT: There was no firewall. and the ssh service was open.



📌SCAN 4: SCAN SPECIFIC PORTS

COMMAND USED : nmap -p 22,80,443 <targetip>

The objective of the scan was to scan specific ports as it is faster than scanning all.

RESULT: only the port 22 was open rest of the ports were closed.



📌SCAN 5 : SCAN A RANGE OF PORTS

COMMAND USED :nmap -p 1-1000 <targetip> (The 1-1000 means the range in wich we wnat the scan to happen)

the objective of the scan was to see which ports were open in the range 1-1000.

RESULT: There was one open port.

port no 22 tcp (service:ssh)



![img](https://github.com/sunandasinghh/nmap-network-troubleshooting/blob/d7d2f20883e1ef52633cbb368048b60f6b18d106/add/scansn.png)



📌SCAN 6: AGGRESIVE SCAN

COMMAND USED: nmap -A <targetip>

the objective of this scan is to perform service,traceroute, os detection.

RESULT: This scan shows what os is running, what version it  is, network distance.



📌SCAN 7: SAVE OUTPUT

COMMAND USED: nmap -oN scan-result.txt <target-ip>

The objective of this scan is to save the result of the scan in a file.

RESULT:AS we can see the result is saved in a file called scan-result.txt .















 
