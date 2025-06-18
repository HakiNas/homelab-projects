# 🧠 Homelab Active Directory Domain Project

This is a complete homelab project built on Hyper-V, focused on creating and managing a Windows Server 2019 Active Directory Domain environment. It demonstrates essential skills used in real-world IT help desk and system administration roles.

---

## ✅ Step 1: Create Your First VM in Hyper-V
- Created a new virtual machine named `DC01`
- Assigned memory and storage
- Mounted the Windows Server 2019 ISO

📸 *Screenshots:* VM creation wizard and summary before booting.

---

## ✅ Step 2: Install Windows Server in the VM
- Booted into the ISO
- Installed Windows Server 2019 (Desktop Experience)
- Set administrator password and logged into the GUI

📸 *Screenshots:* Windows setup process and desktop confirmation.

---

## ✅ Step 3: Rename Server and Set Static IP
- Renamed server to `DC01`
- Assigned static IP `192.168.1.10`
- Verified static IP via Control Panel and `ipconfig`

📸 *Screenshots:* Rename settings, IP configuration window, `ipconfig` output.

---

## ✅ Step 4: Install Active Directory Domain Services (AD DS)
- Used Server Manager to install AD DS
- Promoted the server to Domain Controller for domain `lab.local`
- Restarted after promotion

📸 *Screenshots:* AD DS installation confirmation and setup wizard.

---

## ✅ Step 5: Create Organizational Units (OUs) and Users
- Created OUs: `HR`, `IT`, `SALES`
- Created domain users: `hruser`, `ituser`, `salesuser`

📸 *Screenshots:* Each OU with its respective user inside.

---

## ✅ Step 6: Group Policy Configuration
- Created 3 Group Policies:
  - **Password Policy:** Set minimum password length and complexity
  - **Disable Control Panel**
  - **Set Desktop Wallpaper** via local image

📸 *Screenshots:* Each GPO configuration shown inside Group Policy Management.

---

## ✅ Step 7: Install and Configure DHCP  
> ⚠️ *Note:* DNS was installed automatically during AD DS setup. No further manual DNS configuration was done for this project.

- Installed the DHCP role
- Created and activated a DHCP scope (`192.168.1.100 - 192.168.1.200`)
- Verified active leases

📸 *Screenshots:* DHCP installation, success screen, active scope.

---

## ✅ Step 8: Connect a Windows 10 VM to the Domain
- Created and configured a second VM with Windows 10
- Joined it to the `lab.local` domain
- Successfully logged in as `jdoe@lab.local`

📸 *Screenshots:* Domain-joined system and login screen using domain credentials.

---

## ✅ Step 9: Enable Remote Desktop and File Sharing
- Enabled Remote Desktop from `System Properties`
- Enabled File Sharing via Control Panel
- Verified `Remote Desktop Services` was running using PowerShell

📸 *Screenshots:* RDP settings, File sharing confirmation, Services status.

---

## 📂 Screenshots
All screenshots are organized in step-specific folders (e.g., `Step1_VM_Creation`, `Step2_Windows_Server_Install`, etc.)

---

## 💼 Why This Matters

This lab simulates a real corporate environment, giving hands-on experience with:
- Windows Server 2022
- Active Directory
- Group Policy
- DHCP
- Remote Desktop & File Sharing
- Domain-joined clients

These are core technologies used in IT support and system administration jobs.

---

## 🧠 Lessons Learned

This project taught me:
- How to deploy and configure Windows Server environments
- Best practices in naming, IP configuration, and permissions
- How to troubleshoot and test domain environments in a virtual lab

---

## 👨‍💻 Contact

If you’d like to know more, feel free to reach out via my GitHub profile.
Email : hakinasir@gmail.com

---

