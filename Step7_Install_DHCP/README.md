# Step 7 – Install & Configure DHCP

In this step, I installed and configured the **Dynamic Host Configuration Protocol (DHCP)** role on the domain controller (`DC01`) to automatically assign IP addresses within my lab network.

---

### 🔧 Key Steps Completed:

- Opened **Server Manager > Add Roles and Features** and selected **DHCP Server** for installation.
- Confirmed installation settings and installed required features, including **DHCP Server Tools**.
- Completed the **Post-Install Configuration Wizard**, which:
  - Created DHCP security groups.
  - Authorized the DHCP server in Active Directory.
- Opened the **DHCP Management Console** and:
  - Created a new **IPv4 Scope** named `LabScope`.
  - Configured the scope with an IP address range of `192.168.1.100 – 192.168.1.200`.
  - Verified that the DHCP scope status is marked as **Active**.

---

### 📸 Included Screenshots:

- `DHCP_WIZARD.png` – DHCP role installation confirmation screen in Server Manager.
- `DHCP_SUCCESS.png` – Post-installation summary confirming DHCP authorization and security group creation.
- `DHCP_SCOPE_ACTIVE.png` – DHCP Manager showing the active IPv4 scope (`LabScope`) configured under `dc01.lab.local`.

