# 🔒 NETWORKWALKS-B082-WK1-CYBERSECURITY-LAB-SETUP

> Building an isolated virtual lab for penetration testing and ethical hacking practice.

![Skill: Cybersecurity](https://img.shields.io/badge/Skill-Cybersecurity-red)
![Virtualbox](https://img.shields.io/badge/Virtualbox-v7.7.22-blue)
![Kali Linux](https://img.shields.io/badge/Kali_Linux-v2026.3-orange)
![Network](https://img.shields.io/badge/Network-10.0.0.0%2F24-teal)

---

## 📌 Project Overview

This project documents setting up an isolated virtual lab using VirtualBox and Kali Linux for safe cybersecurity testing[cite: 1]. The process involves downloading VirtualBox and Kali Linux[cite: 2], installing VirtualBox[cite: 2], creating a dedicated NATNetwork[cite: 2], importing the Kali Linux VM[cite: 2], verifying its IP settings[cite: 2], and saving a clean snapshot backup for easy restoration[cite: 2].

---

## 🛠️ Lab Setup Steps (Week 1 Task)

The configuration of this lab environment is broken down into the following core steps[cite: 2]:

### STEP 1: Download Virtualbox & Kali Linux Setup Files
* Download and install Oracle VM VirtualBox (v7.7.22).
* Download the official Kali Linux (v2026.3) pre-built image or installer ISO.

### STEP 2: Install Virtualbox
* Run the VirtualBox installer on your host machine with default settings.
* Install the VirtualBox Extension Pack for full device support.

### STEP 3: Add NATNetworks
* Open VirtualBox **Preferences** -> **Network**.
* Create an isolated `NATNetwork` (e.g., `10.0.0.0/24`) to separate lab traffic from your host network[cite: 1, 2].

### STEP 4: Import Kali Linux in Virtualbox
* Import the Kali Linux appliance file into VirtualBox.
* Allocate system resources (RAM/CPU) and attach the network adapter to your created `NATNetwork`.

### STEP 5: Configure IP Settings Inside Kali Linux
* Boot up the Kali Linux virtual machine.
* Open the terminal and verify network adapter configuration to ensure proper connectivity within the subnet.
  ```bash
  ip a
