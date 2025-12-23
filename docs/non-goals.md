# FluentOS Non-Goals

This document explicitly lists what FluentOS will **never** be or do.

## 1. No Custom Windows ISO

FluentOS will **not**:
- Create custom Windows 11 installation images
- Redistribute Windows components or binaries
- Modify core system files or replace system DLLs
- Patch or rebuild Windows system libraries

**Why?** Such activities would require proprietary access and legal complexity, and violate Microsoft licensing terms.

## 2. No Kernel Patching

FluentOS will **not**:
- Modify the Windows kernel
- Load unsigned drivers
- Intercept system calls
- Perform low-level OS hooking

**Why?** Kernel access is beyond the scope of a UX layer and introduces security/stability risks.

## 3. No License or Security Bypasses

FluentOS will **not**:
- Circumvent Windows Activation
- Disable security features (Windows Defender, UAC) permanently or without consent
- Bypass User Account Control (UAC) prompts for unauthorized operations
- Enable piracy or unauthorized use of Windows

**Why?** FluentOS is designed for legitimate, authorized users with valid licenses.

## 4. Not a Replacement Shell

FluentOS will **not**:
- Replace Explorer.exe or the Windows Shell
- Introduce a custom desktop environment (like KDE or GNOME on Linux)
- Change the fundamental Windows 11 UI paradigm

**Why?** Instead, FluentOS enhances and tailors the existing shell via configuration, theming, and third-party integrations.

---

FluentOS is a **UX enhancement layer**, not a fork, reconstruction, or bypass tool.
