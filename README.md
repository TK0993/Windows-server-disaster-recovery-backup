# Windows Server 2022 Disaster Recovery & System State Backup Lab

This repository documents the practical installation, scheduling, and configuration of enterprise disaster recovery mechanisms using **Windows Server Backup (WSB)** on **Windows Server 2022**.

Ensuring absolute business continuity and maintaining active, scheduled protection of directory infrastructure databases is a fundamental night-shift engineering responsibility within modern Managed Service Provider (MSP) and corporate environments.

---

## 🛠️ Infrastructure Core Components
* **Operating System:** Windows Server 2022 Datacenter Edition
* **Management Console:** Windows Server Backup Tool (`wbadmin.msc`)
* **Automation Framework:** Windows PowerShell 5.1
* **Strategy Target:** System State Backup (Active Directory Domain Architecture)

---

## 🏗️ Technical Execution & Framework Walkthrough

### 1. Feature Deployment via PowerShell
To bypass manual installations, the native server backup architecture features were provisioned using administrative automation blocks.
```powershell
# Command utilized to initialize backup binaries
Install-WindowsFeature -Name Windows-Server-Backup
