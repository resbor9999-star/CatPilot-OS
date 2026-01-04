# Installation Guide

This document describes how to install Windows using the CatPilot OS approach.
It applies to both beginners and advanced users.

CatPilot OS does not replace Windows.
It works **only with original Microsoft Windows images**.

---

## 1. Supported Windows versions

Use **official ISO images only**:

- Windows 10 (2019 / 21H2 / IoT Enterprise)
- Windows 11 (IoT 24H2 / 25H2)

Unofficial builds, repacks, or modified ISOs are **not supported**.

---

## 2. Creating a bootable USB drive

### Recommended tools
- **Rufus**
- **Microsoft Media Creation Tool**

Follow the tool’s default recommendations:
- GPT or MBR — depending on your system
- UEFI or Legacy — depending on hardware
- FAT32 or NTFS — as selected automatically

After this step, the USB drive becomes a standard Windows installer.

---

## 3. `autounattend.xml` placement

Place the file:

Windows Setup will automatically detect and use this file.

---

## 4. Windows installation

1. Insert the USB drive
2. Boot the system from USB
3. Installation will proceed automatically or semi-automatically
   (depending on the `autounattend.xml` configuration)
4. Wait for the first login to Windows

No network connection is required during installation.

---

## 5. PowerShell scripts (`.ps1`)

CatPilot OS uses PowerShell scripts **after Windows installation**.

### Recommended location

Create a directory:

---

## 6. Running scripts (Beginner method)

1. Open **PowerShell as Administrator**
2. Temporarily allow script execution:
   ```powershell
.\CatPilot-Setup.ps1
.\CatPilot-PostInstall.ps1
   Set-ExecutionPolicy RemoteSigned -Scope Process



