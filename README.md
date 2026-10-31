# NETWORKWALKS-MEHAK-B084-WK1-CYBERSECURITY-LAB-S

WEEK 1 : LAB ENVIRONMENT SETUP 

**Creating a cybersecurity environment for pen testing and ethical hacking.**

## OVERVIEW:

This project involves creating a virtual cybersecurity lab using VirtualBox and Kali Linux. The lab will be used to practice cybersecurity tasks such as scanning networks, finding devices, checking for security weaknesses, and testing security tools.

The lab will run on a private virtual network to keep testing separate from normal networks. More virtual machines can be added later to act as target systems for practicing penetration testing safely and legally.

---

## OBJECTIVES:

-Install VirtualBox and set up Kali Linux as a virtual machine on oracle VirtualBox.
-Create a private NAT Network and configure Kali’s network settings with a fixed IP address.
-Test the internet connection and DNS to make sure the network is working.
-Save a VM snapshot so the system can be restored if something goes wrong.
-Document the setup and prepare the lab for future cybersecurity testing and tasks.

---

## PURPOSE:

-Network reconnaissance
-Port scanning
-Vulnerability assessment
-Packet analysis
-Web security testing
-Exploitation practice
-Security-tool experimentation

---

## ARCHITECTURE:

<img width="960" height="509" alt="Capture ss" src="https://github.com/user-attachments/assets/273b03a7-d4f4-4138-b1d1-b343423b5463" />

---

## LAB CONFIGS:

|    Component       |   Configuration    |
| ------------------ | ------------------ |
|    Host OS         | Windows 10         |
|    Host RAM        | 8 GB               |
|    Processor       | Intel Core i7 8th  |
|    Hypervisor      | VirtualBox 7.2.20  |
|    Security OS     | Kali Linux 2026.2  |
|    Kali RAM        | 2048 MB            |
|    Virtual Network | NATNetwork         |
|    Network Address | 10.0.0.0/24        |
|    Kali IP Address | 10.0.0.2/24        |
|    Default Gateway | 10.0.0.1           |
|    DNS Server      | 8.8.8.8            |
|    Future VM Range | 10.0.0.3–10.0.0.99 |

---

## SETUP PROCEDURE: 

## Step 1: Install a file extractor.

For the first step of the procedure i used the winrar file extractor by which the kali linux files were extracted before installation.

Tool used: WINRAR

---

## Step 2: Install Oracle VirtualBox

VirtualBox 7.2.20 was installed to simulate a virtual working environment for the Linux Operating system.

Tool used: Virtualbox 7.2.20

---

## Step 3: NAT Network Creation


Configuration:
Network Name: NatNetwork
IPv4 Prefix:  10.0.0.0/24
DHCP:         Enabled
IPv6:         Disabled

<img width="960" height="506" alt="ss3" src="https://github.com/user-attachments/assets/3493297a-d1b6-4a40-a0be-617cf96afd4a" />

A NAT Network was chosen so that multiple virtual machines connected to the same NAT Network can communicate with each other.
This will allow future attacker and target VMs to communicate within the lab.

---

## Step 4: Importing Kali Linux

The Kali Linux files were downloaded from the linux website then extracted using winrar, after that the files were then imported to the virtualbox. 

```text
Adapter 1:
Attached to:  NAT Network
Network:      NatNetwork
Adapter Type: Intel PRO/1000 MT Desktop
RAM: 2048
```

<img width="525" height="433" alt="ss4" src="https://github.com/user-attachments/assets/8f768b10-38fa-4439-9a69-f32acc62f078" />

---

## Step 5: Kali Network Configuration

The Kali Linux network was configured using a IPv4 address.

```text
IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS: 8.8.8.8
```

<img width="360" height="280" alt="ss1" src="https://github.com/user-attachments/assets/79d7bcb0-fd9b-49e7-8c0a-61ece51e353a" />



## Step 6: VM Snapshot Creation

After completing the initial configuration, a VirtualBox snapshot was created so if anything happens to the machine it can load to a saved state made by the snapshot.

Snapshot name:
```text
KALI
```

<img width="293" height="282" alt="ss2" src="https://github.com/user-attachments/assets/f671e369-9320-447c-9a81-6b70e21d0720" />

---

## Learning Outcomes:

Through this task assigned to me, I learned how to create and configure a virtual environment for cybersecurity practice using kali linux and oracle virtualbox along with IP settings.

### 1. Oracle and Linux installation

I learned how to install oracle virtual box and kali linux files in order to simulate the linux operating system virtually for my cybersecurity journey.

### 2. NAT Network

i learned about NAT network as it was chosen so that multiple virtual machines connected to the same NAT Network can communicate with each other.
This will allow future attacker and target VMs to communicate within the lab.

### 3. Virtual Machine Networking

I learned how VirtualBox network adapters connect virtual machines to networks and how network settings control communication between them.

### 4. Static IP Configuration

I learned how to setup, configure and verify IPv4 addressing, subnet masks, gateways, and DNS settings in the network section for Kali Linux.

### 5. VM Snapshots

I learned how a snapshot should be taken just in-case a crisis arises, as having a backup state helps if something happens to the machine.
This provides a known-good recovery point for future cybersecurity exercises.

### 6. Documentation

I learned that documenting commands, configuration, screenshots, problems, and solutions is an important part of a professional cybersecurity project.

---

## Tools Used:
1- winrar
2- Oracle VirtualBox
3- Kali Linux files

---

Mehak Aslam | Cybersecurity week 1 | VirtualBox Setup
