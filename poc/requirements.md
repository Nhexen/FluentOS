# FluentOS v0.1 POC – Requirements

## System Requirements

### Mandatory

- **Windows 11** (version 25H2 or later)
- **Administrator rights** – Many installation and configuration steps require elevated privileges
- **Network access** (optional) – Needed if installing tools via winget or downloading theme assets

### Recommended

- **8+ GB RAM** – For smooth operation with all enhancements enabled
- **SSD or NVMe** – Faster boot and application loading
- **Modern GPU** – For blur effects (DWMBlurGlass) and window animations (Seelen)

## Software Prerequisites

### Core Installation Tools

- **PowerShell 5.1+** – Included with Windows 11; used for all installation scripts
- **Git** (optional) – For cloning the FluentOS repository; can also download as ZIP

### Optional Third-Party Tools

The following tools enhance FluentOS; installation is optional per feature:

- **Seelen** – Advanced window manager with tiling and layout control
  - Source: GitHub (foss-seelen/seelen-ui)
  - License: Open-source
  - Installation: Manual or via script

- **Windhawk** – UX patcher for fine-grained UI modifications
  - Source: Official website (ramensoftware.com)
  - License: Freeware (personal use)
  - Installation: Download and run installer

- **DWMBlurGlass** – Glass blur effects for window decorations
  - Source: GitHub (australiern/DWMBlurGlass)
  - License: Open-source
  - Installation: Manual or via script

- **Explorer Customizations** – Custom tweaks for Windows Explorer
  - Source: Built-in registry modifications and third-party refinements
  - License: Varies per tweak
  - Installation: Script-based

## Data & Backup Considerations

### Before Installation

- [ ] **Backup user data**: Document current system state, settings, installed software
- [ ] **Backup registry**: Use `regedit` → File → Export to create a registry snapshot
- [ ] **Document current configuration**: Note any custom settings you wish to preserve

### Compatibility Notes

- FluentOS tweaks are generally safe and reversible
- Some registry changes may conflict with third-party software
- Always test in a non-critical environment first (VM, secondary machine, etc.)

## Supported Scenarios

### ✓ Supported

- Fresh Windows 11 installation
- Existing Windows 11 with user data
- Virtual machines (Hyper-V, VirtualBox, VMware)
- Laptop or desktop configurations
- Single machine or organizational deployment (Business/Fleet editions)

### ⚠ Not Tested / Limited Support

- Windows 11 IoT or specialized editions
- Heavily modified Windows 11 installations (other tweaking tools)
- Systems with disabled UAC or modified security policies
- ARM-based Windows 11 (Surface Pro X, etc.) – may have limited tool support

---

For installation steps, see [installation.md](installation.md).
