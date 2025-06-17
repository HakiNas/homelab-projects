# Step 6 – Group Policy Configuration (GPOs)

In this step, I configured Group Policy Objects (GPOs) to enforce company-wide user settings and security standards within the lab.local domain. These policies help ensure consistency, improve security, and restrict unnecessary user access.

### ✅ Key GPOs Created and Applied:

1. **Password Policy**
   - Enforced minimum password length of **8 characters**
   - Set **maximum password age** to **30 days**
   - Set **minimum password age** to **29 days**

2. **Desktop Wallpaper Policy**
   - Forced all users’ desktops to use a standard wallpaper
   - Configured using:
     ```
     C:\windows\web\wallpaper\Windows\img0.jpg
     ```
   - Wallpaper style: **Fill**
   - Prevented users from changing the background

3. **Control Panel Restriction**
   - Disabled access to both Control Panel and PC Settings
   - Applied via the setting:  
     `Prohibit access to Control Panel and PC settings`

### 📸 Included Screenshots:
- `GroupPolicyForest.png` – Group Policy Management Console open on lab.local domain
- `GPO_PSWDPOLICY.png` – Password policy GPO with defined age and length settings
- `GPO_WALLPAPER_POLICY.png` – Wallpaper policy with path and enforcement
- `GPO_DISABLECONTROLPANEL.png` – GPO disabling Control Panel and PC settings

