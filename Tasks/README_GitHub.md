
# 🧪 Practice Lab: Identifying Windows Editions

This lab is part of the **CompTIA 220-1102: A+ Certification** path and focuses on identifying and upgrading different editions of Windows 10 and Windows 11.

---

## 📚 Overview

You will explore various methods to identify Windows editions and learn upgrade paths using hands-on practice with the following virtual machines:

- `PLABDC01` – Windows Server 2019 (Domain Controller)
- `PLABWIN10` – Windows 10 (Domain Member)
- `PLABWIN11` – Windows 11 (Domain Member)
- `PLABWIN11HOME` – Windows 11 Home Edition
- `PLABSUSE`, `PLABUBUNTU`, `PLABANDROID` – Additional environments

---

## 🎯 Learning Objectives

- Identify the Windows edition
- Differentiate between editions of Windows 10 and 11
- Understand and simulate in-place upgrade paths

---

## 📝 Exercise 1 – Identify Different Windows Editions

### 🔍 Using `winver` Command
1. Connect to `PLABWIN10`
2. Press **Start** → Type `winver`
3. View edition/version (e.g. Windows 10 Pro, Version 21H1)

### 📂 Using System Properties
1. Connect to `PLABWIN11`
2. Open **File Explorer** → Right-click **This PC** → **Properties**
3. Check version info under **System > About**

### 🖥 Notable GUI Differences
- Windows 11 centers the Start Menu on the taskbar
- Enhanced GUI and new layout options

---

## 🧩 Windows Edition Comparison

| Edition                  | Target Users         | Key Features |
|--------------------------|----------------------|--------------|
| **Home**                | Home Users           | Edge, Hello, Virtual Desktops, Auto Updates |
| **Pro**                 | SMBs                 | Bitlocker, GPO, Azure AD, MDM |
| **Pro for Workstations**| Power Users          | ReFS, Persistent Memory, 4 CPU/6TB RAM |
| **Enterprise**          | Large Organizations  | AppLocker, Credential Guard, Application Control |

> ⚠️ Home editions **cannot join domains** or use Bitlocker.

---

## 🧪 Exercise 2 – Explore Upgrade Pathways

### 🔄 In-Place Upgrade Example (Home → Pro)
1. Attach **Windows 11 ISO** via **Hyper-V**
2. Launch VM: `PLABWIN11HOME`
3. Open **DVD Drive (D:)** → Run `setup.exe`
4. Proceed through the wizard (updates, checks, etc.)
5. Upgrade proceeds without data loss

> Note: Upgrade is simulated due to lab limitations

---

## 🔑 Optional: Product Key Upgrade
1. Go to **Settings > System > Activation**
2. Click **Change product key**
3. Enter valid Pro edition key to trigger upgrade

---

## ✅ Summary

### Completed:
- [x] Identify Windows Editions
- [x] Compare Pro vs Home, Enterprise, Workstation
- [x] Simulate Windows 11 Home → Pro in-place upgrade

---

## 🧹 After Lab
Shutdown all virtual machines or log out from the lab platform.

---

© 2025 | Lab Practice for CompTIA A+
