# Seelen Integration

## Overview

**Seelen** is an advanced window manager for Windows 11 that brings tiling and layout control to the desktop, similar to window managers found in Linux environments.

**Role in FluentOS:** Seelen enhances the windowing experience by providing keyboard-driven window management, virtual desktops, and customizable tiling layouts. It complements FluentOS's focus on productivity and coherence.

## Status in v0.1

- **Availability:** Optional (not required for Core edition)
- **Integration:** Basic skeleton; configuration details TODO for v0.2+
- **Stability:** Seelen itself is stable; FluentOS integration is POC-phase

## Key Features

- **Tiling Layouts:** Automatically arrange open windows in efficient grid patterns
- **Virtual Desktops:** Organize windows across multiple virtual workspaces
- **Keyboard Shortcuts:** Quick window management without mouse
- **Customizable Themes:** Match Seelen decorations to FluentOS visual identity

## Installation

### Automatic (via FluentOS installer)

```powershell
.\scripts/install/winget.ps1
# Select "yes" when prompted for Seelen installation
```

### Manual

1. Download from [GitHub: foss-seelen/seelen-ui](https://github.com/foss-seelen/seelen-ui/releases)
2. Run the installer
3. Configure via Seelen settings UI

## Configuration

TODO: Add detailed configuration schema and examples

- Configuration file: `~/.seelen/seelen.yaml`
- Themes directory: `~/.seelen/themes/`
- Layouts: Tiling, floating, stacking modes

## Known Issues

- TODO: Document Seelen-specific limitations for v0.1
- Possible conflicts with other window management tools
- May require driver updates for optimal performance on some GPUs

## Uninstall

```powershell
# Option 1: Via Windows Settings > Apps
# Option 2: Via Seelen UI uninstaller
# Option 3: Via full FluentOS rollback
.\scripts/uninstall/rollback.ps1 -Full
```

## Further Resources

- [Seelen GitHub](https://github.com/foss-seelen/seelen-ui)
- [Windows Virtual Desktops Guide](https://support.microsoft.com/en-us/windows/using-virtual-desktops-in-windows-10-ac7537d0)
