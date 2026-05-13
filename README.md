# ARP-Attack-and-Network-Sniffing
# Explore Network Sniffing and ARP Attacks

# AIM:

To explore network sniffing and ARP Attacks

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## ARP Attacks:  
ARP spoofing: A hacker sends fake ARP packets that link an attacker's MAC address with an IP of a computer already on the LAN. 
Boot kali and Windows7 virtual machines.
In windows 7 give the command arp -a
## OUTPUT:

<img width="1080" height="605" alt="image" src="https://github.com/user-attachments/assets/96d2ddb5-6c25-4943-bc4b-451047d88df7" />



From kali linux issue the command :
sudo arpspoof -i eth0 -t <target system> <gateway>
## OUTPUT:

<img width="964" height="494" alt="Screenshot 2025-09-21 150622" src="https://github.com/user-attachments/assets/8c8c100e-7a7e-4f5e-8c9c-4ff27c36395a" />


Invoke the wireshark and examine the various menus  and controls of the tool:

<img width="1919" height="1106" alt="Screenshot 2025-09-21 144742" src="https://github.com/user-attachments/assets/5f382e8d-e2f9-4f3a-90cf-f443c85cb68f" />



## RESULT:
The kali linux tools for ARP Attack and Network Sniffing were identified successfully
