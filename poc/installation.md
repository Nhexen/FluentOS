# FluentOS v0.1 POC – Installation Guide

## Prerequisites

Before you begin, ensure your system meets the requirements in [requirements.md](requirements.md).

## Step 1: Clone or Download FluentOS

### Option A: Clone with Git

```powershell
# Open PowerShell and navigate to your desired location
git clone https://github.com/codixia/fluentos.git
cd fluentos
```

### Option B: Download as ZIP

1. Visit the [FluentOS GitHub repository](https://github.com/codixia/fluentos)
2. Click "Code" → "Download ZIP"
3. Extract the ZIP to your desired location
4. Open PowerShell in the extracted `fluentos` folder

## Step 2: Verify Windows Version

Run this command to check your Windows version:

```powershell
[System.Environment]::OSVersion.Version
```

**Expected:** Version `10.0.26100` or higher (Windows 11 25H2+)

TODO: Add automated version check and warning script

## Step 3: Run Installation Scripts

Navigate to the `scripts/install/` directory and run scripts in order:

### 3.1 Install Tools (Optional)

```powershell
.\winget.ps1
```

This script will prompt you to install optional tools:
- Seelen (window manager)
- Windhawk (UX patcher)
- DWMBlurGlass (blur effects)

TODO: Implement tool installation logic and error handling

### 3.2 Apply System Tweaks

```powershell
.\tweaks.ps1
```

This applies:
- Theme customization
- Taskbar and Start Menu changes
- Windowing behavior adjustments

TODO: Add registry modification and system settings configuration

### 3.3 Optimize Services

```powershell
.\services.ps1
```

This enables/disables non-essential Windows services for better performance.

TODO: Implement service management and rollback

## Step 4: Apply Theme Profile

Choose a theme profile and apply it:

```powershell
# Light theme (default)
Import-FluentOSProfile -Path "scripts/profiles/fluentos-core-light.json"

# Dark theme
Import-FluentOSProfile -Path "scripts/profiles/fluentos-core-dark.json"
```

TODO: Implement profile application function

## Step 5: Verify Installation

Restart your system and verify:
- [ ] Desktop theme applied correctly
- [ ] Taskbar and Start Menu reflect new styling
- [ ] Optional tools (Seelen, Windhawk, etc.) functioning as expected
- [ ] No system instability or performance issues

## Troubleshooting

### Scripts Won't Run

If you encounter execution policy errors:

```powershell
# Allow scripts to run in current session
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
```

### System Feels Unstable

Run the rollback script:

```powershell
.\scripts/uninstall/rollback.ps1
```

TODO: Expand rollback procedure and recovery options

## Uninstall / Rollback

To revert FluentOS changes:

```powershell
.\scripts/uninstall/rollback.ps1
```

This will:
- Restore original Windows 11 defaults
- Disable FluentOS-installed tools (optional)
- Reset registry modifications
- Restore user settings

TODO: Add comprehensive rollback logic

---

**Next Steps:**
- See [configuration.md](configuration.md) for customization options
- See [known-limitations.md](known-limitations.md) for current constraints
- See [../docs/legal.md](../docs/legal.md) for legal and compliance information
