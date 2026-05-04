<p align="center">
  <img src="os ticket.jpg" alt="osTicket Logo" width="200">
</p>

# osTicket — Prerequisites and Installation  
*A simple, beginner‑friendly walkthrough with screenshots*

This guide shows you how to install the open‑source help desk system **osTicket** on a Windows 10 Virtual Machine in Microsoft Azure.  
You will install all required software, configure IIS, set up PHP, create a database, and finish the osTicket installation.

---

# 🎥 Video Demonstration
- **YouTube:** How To Install osTicket with Prerequisites  
  *(Insert your link here)*

---

# 🧰 Technologies Used
- Microsoft Azure (Virtual Machines)
- Remote Desktop (RDP)
- Internet Information Services (IIS)
- PHP + required extensions
- MySQL Server
- osTicket Installer

---

# 🖥 Operating System Used
- **Windows 10 (21H2)**

---

# 🟦 Part 1 — Create Your Azure Virtual Machine

## ✔️ 1. Create a Windows 10 VM in Azure
- Go to https://portal.azure.com  
- Create a **Resource Group**
- Create a **Windows 10 VM**
- Allow Azure to create:
  - A **Virtual Network (VNet)**
  - A **Subnet**
- Connect to the VM using **Remote Desktop**

<p align="center">
  <img src="vm-creation.png" width="80%">
</p>

---

# 🟩 Part 2 — Install Required Software

## ✔️ 2. Install IIS (Internet Information Services)

### Steps:
1. Open **Control Panel**
2. Go to **Programs → Turn Windows features on or off**
3. Enable:
   - Internet Information Services
   - IIS Management Console
   - CGI
   - Common HTTP Features
4. Click **OK** and let Windows install IIS

<p align="center">
  <img src="iis-install.png" width="80%">
</p>

---

## ✔️ 3. Install PHP and Required Extensions

### Steps:
1. Download PHP (version 7.3 or 7.4 works best with osTicket 1.15.x)
2. Extract PHP to:
