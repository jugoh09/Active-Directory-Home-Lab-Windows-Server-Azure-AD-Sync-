# 🖥️ Active Directory Home Lab (Windows Server + Azure AD Hybrid)

## 📌 Project Overview
This project simulates a real-world enterprise IT environment by deploying a Windows Server 2022 Domain Controller, configuring Active Directory, and integrating it with Azure AD using Azure AD Connect.

The goal was to replicate production-level identity and access management workflows, including user provisioning, Group Policy enforcement, and hybrid cloud synchronization.

---

## 🏗️ Environment Setup

**Virtualization Platform:**
- VirtualBox

**Systems Deployed:**
- Windows Server 2022 (Domain Controller)
- Windows 11 Enterprise (Domain-Joined Client)

**Cloud Integration:**
- Azure AD (Free Tier)
- Microsoft Entra

---

## 🧩 Architecture Overview
- On-premises Active Directory Domain (`victorgoh.lab`)
- Domain Controller managing users, groups, and policies
- Windows 11 client joined to domain
- Azure AD Connect syncing identities to Azure AD

---

## ⚙️ Key Configurations

### 🧑‍💼 Active Directory Setup
- Installed and configured **Active Directory Domain Services (AD DS)**
- Promoted Windows Server to Domain Controller
- Created domain: `victorgoh.lab`

---

### 🗂️ Organizational Units (OUs)
- IT  
- HR  
- Finance  

Each OU includes:
- 5 test users  
- 2 security groups  

---

### 🔐 Group Policy Objects (GPOs)
Configured and applied multiple GPOs to simulate enterprise controls:

- Enforced desktop wallpaper policy  
- Configured network drive mapping  
- Disabled USB storage devices for security  

---

### ☁️ Azure AD Integration
- Installed and configured **Azure AD Connect**
- Synced on-prem AD users to Azure AD tenant
- Validated hybrid identity functionality

---

## 🖼️ Screenshots

Include screenshots of:
- Active Directory Users and Computers (OU structure)  
- Group Policy Management Console  
- Domain-joined Windows 11 system  
- Azure AD synced users  

> 📁 Store images in `/screenshots` and embed below:

```md
![AD Structure](screenshots/ad-structure.png)
![GPO Settings](screenshots/gpo.png)
