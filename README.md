<img width="4096" height="2119" alt="Picsart_26-06-04_03-28-23-368" src="https://github.com/user-attachments/assets/f2948c95-3209-4497-9dee-978e7a738074" />



# Lunaris-AOSP 3.10 | Unofficial 

* **Device:** Realme 8i / Narzo 50 (spaced)
* **Build Type:** User | GAPPS
* **Android Version:** 16 | QPR2
* **Maintainer:** D Ξ Ξ Z N U T Z
* **Release Date:** June 04, 2026
* **Download Link Here:** https://drive.google.com/file/d/1Yyiw0LfWa5kcXA72PWwnymg0GFxX6FrD/view?usp=drive_link

---

### 🚀 **Changelog**

#### 🛠 **Device Tree & System Fixes**
* **Primal Fluidity:** Hardcoded SurfaceFlinger rendering pipeline variables to enforce a locked 120Hz floor across all standard UI threads and frame categories.
* **Touch Response:** Fixed SurfaceFlinger scheduler uclamp errors for background tasks and screenshots, reducing rendering jitter and eliminating micro-stutters when waking the panel.

#### 🛡 **SEPolicy & Security Updates**
* Enforced strict, pristine SELinux rules natively matching Android's production environment specifications.
* Resolved background audit blocks for `mtk_hal_neuralnetwork` by safely mapping VNDK symlink read access to ensure unhindered NeuroPilot/APU initialization.
* Resolved `thermal_manager` access restrictions to allow accurate reading of core `/proc/stat` utilization loops.
* Implemented targeted `dontaudit` silencing rules to clean up user-space framework logs without creating security vulnerabilities.

#### ⚡ **Hyperion Kernel v1.1 Changes**
* **Log Buffer Optimization:** Silenced repetitive watchdog API failure warning logs (`WD API` / `FAILED TO GET`) inside core MTK thermal driver structures (`mtk_tc` / `mtk_lvts_tc`), heavily clearing ring buffer overhead.
* **Stability Hardening:** Implemented strict memory allocation fail-safes and enhanced tracking boundaries for the `clmutt` / `clmutt_tm_pid` procfs drivers to eliminate null-pointer scenarios if nodes are busy.

---

### 📝 **Notes & Installation**
* A clean flash is always recommended if coming from another ROM tree.

### 🤝 **Credits & Thanks**
* Huge thanks to `@HELLINFIX` for the foundational source collaboration and device tree support.
* Thanks to @ViaanLarryROMS for the assistance in adding Sony Dolby
* To all our community testers who ran log streams to track down some issues.
