# Step 3 – Static IP Configuration & Server Rename

In this step, I configured a **static IP address** and renamed the server to `DC01` as part of the domain setup process.

### Key Steps Completed:
- Manually assigned the following IP settings:
  - **IPv4 Address:** 192.168.1.10
  - **Subnet Mask:** 255.255.255.0
  - **Default Gateway:** 192.168.1.1
  - **Preferred DNS Server:** 192.168.1.10
- Verified the static IP assignment in both:
  - **Control Panel > Network Settings**
  - **Command Prompt using `ipconfig`**
- Renamed the system from the default name to **DC01**

### Included Screenshots:
- `VMCMDStaticIPConfirmed.png` – IP confirmed via `ipconfig`.
- `ControlPanelStaticIPConfirm.png` – IP settings shown in Control Panel.
- `IPv4DefaultSettings.png` – Static IP settings entry screen.
- `LocalServerDefaultName.png` – Default computer name before renaming.
- `LocalServerNewName.png` – Computer name after renaming to `DC01`.
