# Windhawk Integration

## Overview

**Windhawk** is a freeware UX patcher that allows fine-grained modifications to Windows UI elements through community-created mods.

**Role in FluentOS:** Windhawk enables visual and behavioral customizations that would otherwise require deep registry hacking or system file modification. FluentOS curates a set of Windhawk mods that enhance coherence and aesthetics while maintaining system stability.

## Status in v0.1

- **Availability:** Optional (not required for Core edition)
- **Integration:** Basic skeleton; mod list TODO for v0.2+
- **Stability:** Windhawk itself is mature; FluentOS integration is POC-phase

## Key Features

- **Non-invasive UI Modifications:** Patch UI elements without replacing system files
- **Community Mods:** Access to hundreds of user-created modifications
- **Easy On/Off:** Toggle mods individually without system restart (usually)
- **Safe Rollback:** Disable any mod to revert its effects

## Installation

### Automatic (via FluentOS installer)

```powershell
.\scripts/install/winget.ps1
# Select "yes" when prompted for Windhawk installation
```

### Manual

1. Download from [ramensoftware.com](https://ramensoftware.com/windhawk)
2. Run the installer
3. Follow the setup wizard

## Recommended Mods for FluentOS

TODO: Create curated mod list for v0.2

Planned mods for Core edition:
- Taskbar styling mods (if any)
- Start Menu refinements
- Window decoration enhancements
- Explorer UI tweaks
- System font refinements

## Configuration

TODO: Add detailed mod configuration examples

- Mod management: Windhawk UI or registry-based
- Custom mods: Place in `%APPDATA%\Windhawk\mods/`
- Settings: Per-mod customization via Windhawk interface

## Known Issues

- TODO: Document Windhawk-specific limitations for v0.1
- Some mods may conflict with third-party themes or accessibility tools
- Requires occasional Windhawk updates to maintain compatibility with Windows updates

## Uninstall

```powershell
# Option 1: Via Windows Settings > Apps
# Option 2: Via Windhawk uninstaller (Settings > About)
# Option 3: Via full FluentOS rollback
.\scripts/uninstall/rollback.ps1 -Full
```

## Further Resources

- [Windhawk Official Site](https://ramensoftware.com/windhawk)
- [Windhawk Mod Repository](https://github.com/ramensoftware/windhawk-mods)
- [Windhawk Documentation](https://ramensoftware.com/windhawk/help)
