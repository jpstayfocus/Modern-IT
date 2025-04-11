# Exercise 1 - Identify Different Windows Editions

The Windows 10 and Windows 11 Operating systems were released as different Windows Editions. Each edition has distinct functionalities and features intended for various use case scenarios.

In this exercise, we will explore and identify different Windows Editions using multiple methods.

## 📘 Learning Outcomes

After completing this exercise, you should be able to:

- Identify the Windows Edition
- Differentiate between different Windows Editions

## 💻 Devices Used

You will be using the following devices in this lab. Please power these on now:

- `PLABDC01` - (Windows Server 2019 - Domain Controller)
- `PLABWIN10` - (Windows 10 - Domain Member Workstation)
- `PLABWIN11` - (Windows 11 - Domain Member Workstation)

---

## 🧪 Task 1 - Identify the Windows Edition

### Step 1: Connect to PLABWIN10

- Click the **Start** charm.

### Step 2: Type the following command:

```bash
winver
```
- Select **winver** from the **Best match** pop-up menu.

> This command displays the version and build of the Windows OS.
> Example: Windows 10 Pro Edition, Version 21H1.

### Step 3: Close the *About Windows* window.

### Step 4: Connect to PLABWIN11

- Click the **File Explorer** icon on the Taskbar.

> Notice the GUI differences between Windows 10 and 11 (e.g. centered Start button).

### Step 5: Right-click **This PC** and select **Properties**.

- Scroll down to the **Windows specifications** section.

> Example: Windows 11 Pro Edition, Version 21H2, OS Build 22000.527

### Step 6: Close all open windows.

---

## 🧠 Task 2 - Differentiating Between Windows Editions

Windows 10 and 11 were released with the same editions. Each edition serves a different purpose and includes specific features.

### 🔹 Windows 10/11 Home Edition

- Targeted at home users.
- Limited functionality.

**Key Features:**
- New Microsoft Edge browser
- Windows Hello
- Virtual Desktops
- Built-in apps (Photos, Maps, Mail)
- Native firewall and antivirus
- Automatic updates

### 🔸 Windows 10/11 Pro Edition

- Targeted at SMBs with advanced features.

**Key Features:**
- Join Azure Active Directory
- Mobile Device Management (MDM)
- Bitlocker encryption
- Group Policy Management

### 🟣 Windows 10/11 Pro for Workstations Edition

- Adds features for advanced hardware support.

**Key Features:**
- Resilient File System (ReFS)
- Persistent Memory
- Support for 4 CPUs and up to 6TB RAM

### 🟢 Windows 10/11 Enterprise Edition

- For large organizations with volume licensing.

**Key Features:**
- AppLocker
- Start Menu layout management via MDM
- Microsoft Defender Credential Guard
- Microsoft Defender Application Control
- Microsoft Application Virtualization

---

### Identify Domain Membership

### Step 1: Connect to PLABWIN11

- Click **File Explorer** > Right-click **This PC** > **Properties**

### Step 2: Open **Advanced system settings** > **Computer Name** tab

### Step 3: Click **Change**

> Only Pro and Enterprise editions can join a domain. Home edition does not support this.

### Step 4: Cancel and close all windows.

---

## 🧪 Bonus: Accessing Hyper-V

### Step 1: Connect to PLABWIN10

- Open **Hyper-V Manager**

### Step 2: Connect and Start the `PLABWIN11HOME` virtual machine

> Note: Startup may take a few minutes.

---

## 📌 Notes

- This exercise helps understand how to identify and compare Windows Editions.
- Use `winver`, system properties, and domain settings to determine editions and capabilities.

---

© 2025 | Windows Editions Lab Exercise
