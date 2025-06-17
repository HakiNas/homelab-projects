# Step 4 – Active Directory Domain Services (AD DS) Setup

In this step, I installed the **Active Directory Domain Services (AD DS)** role on the domain controller VM `DC01` and confirmed that the `lab.local` domain was successfully created.

---

### 🔧 Key Steps Completed:

- Opened **Server Manager** and selected **Add roles and features**.
- Chose the **Active Directory Domain Services** role and added the required features.
- Completed the wizard and installed the role (server restart occurred if prompted).
- After installation, launched **Active Directory Users and Computers (ADUC)** to verify domain creation.
- Confirmed the `lab.local` domain is active and listed under the console.

---

### 📸 Included Screenshots:

- `ADFirst.png` – Wizard prompt to install required features for Active Directory Domain Services.
- `ADConfirmation.png` – Server Manager dashboard after installation showing the AD DS and DNS roles in the left pane.
- `ADSecondConfirmation.png` – Active Directory Users and Computers console showing the `lab.local` domain.

