# Scripts — CatPilot OS

This directory contains the minimal set of scripts used by CatPilot OS.

The goal of these scripts is not aggressive optimization,  
but **careful, predictable configuration** based on the H.E.G.M. approach.

CatPilot OS does not automate everything —  
only what is necessary and well understood.

---

## Structure

- `autounattend.xml`  
  Used during installation.  
  Handles basic system setup that cannot be safely postponed.

- `CatPilot-Setup.ps1`  
  Main configuration script.  
  Applies H.E.G.M. principles after installation.

- `CatPilot-PostInstall.ps1` *(optional)*  
  Additional configuration:
  - drivers
  - network
  - ID-card support
  - verified power settings  

  Not required for core system operation.

---

## Design Principles

- One installation file  
- One main PowerShell script  
- No hidden logic  
- No obfuscation  
- No forced behavior  

Scripts are:
- readable
- reversible
- updated slowly (1–2 times per year)

---

## What These Scripts Do

- reduce unnecessary background activity
- improve stability on real hardware
- respect long hardware life cycles
- avoid constant system changes

---

## What These Scripts Do NOT Do

- no registry spam
- no unsafe tweaks
- no aggressive debloating
- no constant reconfiguration

If the system works — it is not touched.

---

## Compatibility

Designed and tested with:

- Windows 10 (2019 / IoT Enterprise 21H2)
- Windows 11 (IoT Enterprise 24H2 / Pro 25H2)

The same H.E.G.M. approach is used across versions.

---

## Update Policy

Scripts are updated only when:
- a real issue is confirmed
- a change is necessary for compatibility
- stability is preserved or improved

Silence is preferred over frequent updates.

---

## Final Note

These scripts are not a product.  
They are a **method of interaction** with the operating system.

Sometimes the best improvement  
is to leave the system alone.

_Minute of reflection — a step into History._
