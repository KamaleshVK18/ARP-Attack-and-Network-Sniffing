# ARP-Attack-and-Network-Sniffing using Ettercap

# Explore Network Sniffing and ARP Attacks using Ettercap

# AIM:

To explore network sniffing and ARP attacks using the Ettercap tool in Kali Linux.

---

# STEPS:

## Step 1:

Install Kali Linux either in partition, VirtualBox, VMware, or live mode.

## Step 2:

Investigate the various categories of penetration testing and network analysis tools available in Kali Linux.

## Step 3:

Open the terminal and execute basic Kali Linux commands to verify network connectivity and interface details.

Example commands:

```bash
ifconfig
ip a
ping google.com
```

---

# ARP Attacks using Ettercap

ARP spoofing is a technique where an attacker sends forged ARP packets to associate the attacker’s MAC address with the IP address of another device on the LAN. This allows interception of network traffic between systems.

---

## Procedure:

### Step 1:

Boot both Kali Linux and Windows 7 virtual machines in the same network.

### Step 2:

In Windows 7, open Command Prompt and execute:

```bash
arp -a
```

## OUTPUT:

*(Insert screenshot of ARP table here)*

---

### Step 3:

In Kali Linux, identify the network interface using:

```bash
ifconfig
```

or

```bash
ip a
```

---

### Step 4:

Launch Ettercap in graphical mode using the command:

```bash
sudo ettercap -G
```

## OUTPUT:

*(Insert screenshot of Ettercap GUI opening here)*

---

### Step 5:

In Ettercap:

1. Click on **Sniff → Unified Sniffing**
2. Select the active network interface (example: `eth0` or `wlan0`)
3. Click **Hosts → Scan for Hosts**
4. After scanning, click **Hosts → Hosts List**
5. Select the target system and gateway/router
6. Click **Add to Target 1** and **Add to Target 2**

---

### Step 6:

Start the ARP spoofing attack by navigating to:

```text
Mitm → ARP Poisoning
```

Enable:

```text
✓ Sniff remote connections
```

Click **OK**.

---

### Step 7:

Start packet sniffing by clicking:

```text
Start → Start Sniffing
```

Ettercap will now begin intercepting packets between the target system and the gateway.

## OUTPUT:

*(Insert screenshot of Ettercap ARP poisoning/sniffing here)*

---

# Wireshark Analysis

Open Wireshark in Kali Linux and capture packets on the same interface.

Observe:

* ARP packets
* Source and destination MAC addresses
* TCP/IP traffic
* Protocol analysis

## OUTPUT:

*(Insert screenshot of Wireshark packet capture here)*

---

# RESULT:

The Kali Linux tools for ARP attacks and network sniffing were successfully identified and implemented using Ettercap and Wireshark.
