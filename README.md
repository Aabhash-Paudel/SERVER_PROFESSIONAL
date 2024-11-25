# 🖥️ Advanced Active Directory Management and Group Policy Implementation

**📜 Submitted to:**  
**L&T EduTech**

**📋 By:**  
- Aabhash Paudel  
- Chudaraj Kushwaha  
- Satyam Raut  

**🏫 Institution:**  
Sri Venkateshwara College of Engineering And Technology  

📅 **November 2024**  

---

## 📑 Table of Contents

1. [Introduction](#1-introduction)  
2. [Objectives](#2-objectives)  
3. [Methodology](#3-methodology)  
4. [Findings](#4-findings)  
5. [Documentation](#5-documentation)  
6. [Challenges and Resolutions](#6-challenges-and-resolutions)  
7. [Conclusion](#7-conclusion)  
8. [References](#8-references)  

---

## 1️⃣ Introduction  

Active Directory Domain Services (AD DS) is a core component of Windows Server, enabling centralized management and authentication for users and computers in a network.  

The primary goal of this project was to:  
- Implement an **Active Directory Domain Services (AD DS)** environment.  
- Explore advanced management features.  
- Create and configure **Group Policies** for enhanced security and operational efficiency.  

---

## 2️⃣ Objectives  

The key objectives of this project were:  

1. ✅ Configure a new Active Directory Forest and promote servers as Domain Controllers (DCs).  
2. ✅ Explore advanced Domain Controller features, such as **cloning** and **Read-Only Domain Controllers (RODCs)**.  
3. ✅ Implement advanced security configurations, including:  
   - **Password Settings Objects (PSOs)**  
   - **Authentication Policies**  
   - **Managed Service Accounts (MSA)**  
4. ✅ Configure and manage **Group Policy Objects (GPOs)** for linking, filtering, and setting precedence.  
5. ✅ Simulate and document recovery procedures for AD DS.

---

## 3️⃣ Methodology  

### 📂 3.1 Environment Setup  

**🔧 Tools Used:**  
- **Oracle VirtualBox:** Virtualization platform.  
- **Windows Server 2019:** Operating System for Domain Controllers.  
- **AD DS & GPMC:** For managing directory services and Group Policies.

**🌐 Network Setup:**  
- Virtual machines connected via the host laptop’s **mobile hotspot** using a **bridged adapter** to simulate enterprise environments.

---

### 🛠️ 3.2 Step-by-Step Implementation  

1. **Configuring AD DS for a New Forest:**  
   - Installed the AD DS role and promoted the server as a **Domain Controller** for a new forest (`example.local`).  
   - Set up the **Directory Services Restore Mode (DSRM)** password.

2. **Adding a Secondary Domain Controller:**  
   - Installed a secondary Windows Server 2019 instance.  
   - Joined and promoted it to a DC in the existing forest.

3. **Exploring Advanced DC Options:**  
   - **DC Cloning:** Configured a VM to clone an existing DC.  
   - **RODC Setup:** Deployed a Read-Only Domain Controller for secure branch office scenarios.

4. **Configuring Security Policies:**  
   - Created and applied **Password Settings Objects (PSOs)**.  
   - Configured **Authentication Policies and Silos** for sensitive resource access.  
   - Set up **Managed Service Accounts (MSA)** for secure service management.

5. **Implementing Group Policies:**  
   - Linked **GPOs** for password policies and user restrictions.  
   - Used **WMI filters** for targeted policy application.  

6. **Simulating Recovery Procedures:**  
   - Performed **system state backups** and restored using **DSRM**.  

---

## 4️⃣ Findings  

### 🔍 AD DS Configurations:  
- Successfully configured a **new forest and root domain**.  
- Added and promoted additional DCs to enhance **redundancy** and **load balancing**.

### 🔍 Advanced DC Features:  
- **Cloning:** Effective for rapid deployment but needs rigorous testing.  
- **RODCs:** Improved branch site security but required careful delegation.

### 🔍 Group Policy Management:  
- Linking GPOs at various levels provided precise control over settings.  
- **WMI filters** improved efficiency by targeting specific devices or users.

### 🔍 Recovery Procedures:  
- Highlighted the importance of **regular system state backups** for disaster recovery.

---

## 5️⃣ Documentation  

### 📸 Key Configuration Screenshots:  
Captured and documented:  
- AD DS installation and promotion.  
- **Password Settings Objects** and **Authentication Silos**.  
- GPMC configurations for GPO linking and editing.

Documentation:    
        [FILE](https://drive.google.com/file/d/1E8hBa72MyWEAEUu3k7dFK-N8OeHY38N7/view?usp=sharing)

Focused on User-Group Management and Powershell:

Documentation:   
       [FILE](https://drive.google.com/file/d/1rZwS78Ao0h5bAXebeKCW_9qHS5-oVGc9/view?usp=sharing)


---

## 6️⃣ Challenges and Resolutions  

| **Challenge**                            | **Resolution**                                                                 |
|------------------------------------------|---------------------------------------------------------------------------------|
| Networking VMs effectively.              | Switched from **NAT to Bridged Adapter** for better connectivity.               |
| DC Cloning prerequisites were complex.   | Followed Microsoft's guidelines and rigorously tested in a virtual environment. |
| Limited hardware capabilities in the VM. | Allocated **less memory per system** to improve performance.                    |

---

## 7️⃣ Conclusion  

The project successfully simulated an **Active Directory** environment using **Windows Server 2019**, exploring advanced features like:  
- **RODCs**  
- **Authentication Silos**  
- **GPOs**
- **User management**
- **Group management**
- **Domain management**

The experience provided insights into practical challenges and emphasized the importance of **planning** and **testing** in real-world scenarios.  

This comprehensive simulation serves as a valuable reference for enterprise deployments.

---

## 8️⃣ References  

- 📘 [Microsoft Documentation - Active Directory Overview](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/)  
- 📘 [Group Policy Management Overview](https://docs.microsoft.com/en-us/windows-server/administration/grouppolicy/grouppolicy-overview)  
- 💻 TechNet Forums: For troubleshooting GPO and AD DS issues.  
- 🌐 VirtualBox Networking Guides: For VM setup.
- L&T Edutech: https://learn.lntedutech.com/

---

### 🚀 **Thank You!**
