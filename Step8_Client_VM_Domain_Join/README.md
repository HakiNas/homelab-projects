# Step 8 – Connect a Second VM to the Domain

In this step, I created a second virtual machine running Windows 10 and successfully joined it to the Active Directory domain `lab.local`. This simulates a typical enterprise environment where user workstations are connected to a centralized domain for authentication and policy management.

### Key Steps Completed:

- Set up a new Windows 10 client VM in Hyper-V.
- Verified that the client VM was on the same network as the domain controller.
- Joined the domain `lab.local` via the System Properties dialog.
- Restarted the client after domain join confirmation.
- Logged in using a domain account (`jdoe`) that was created earlier in Active Directory.
- Verified successful login and domain membership using the `whoami` command in Command Prompt.

### Included Screenshots:

- `Step8_DomainJoin.png` – Confirmation message showing the client successfully joined the `lab.local` domain.
- `Step8_JDOE_LOGIN.png` – Command prompt confirming the login as `lab\jdoe` on the Windows 10 client.
