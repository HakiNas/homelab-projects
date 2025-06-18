# Step 9 – Enable Remote Desktop & File Sharing

In this step, I enabled Remote Desktop access and confirmed that file sharing and network discovery services were active on the domain controller (DC01).

---

### ✅ Key Tasks Completed:

- Enabled **Remote Desktop** via Settings > System > Remote Desktop.
- Verified Remote Desktop was accessible using the PC name: `DC01.lab.local`.
- Used **PowerShell** to:
  - Enable **Network Discovery** and **File & Printer Sharing** with:
    ```powershell
    Set-NetFirewallRule -DisplayGroup "Network Discovery" -Enable True -Profile Domain,Private,Public
    Set-NetFirewallRule -DisplayGroup "File and Printer Sharing" -Enable True -Profile Domain,Private,Public
    ```
  - Confirm connectivity with `Test-Connection DC01`
  - Verified the **Server service** (responsible for file sharing) was running with:
    ```powershell
    Get-Service -Name lanmanserver
    ```

---

### 📸 Included Screenshots:
- `Step9_RDP.png` – Remote Desktop enabled and connection instructions visible.
- `Step9_Confirmation.png` – PowerShell output showing ping results and network discovery/firewall rules.
- `Step9_Running.png` – Verified "Server" service (lanmanserver) is running, confirming file sharing is active.

