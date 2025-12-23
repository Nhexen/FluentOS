# DWMBlurGlass Integration

## Overview

**DWMBlurGlass** is an open-source utility that applies Aero-style blur effects to window decorations and background surfaces in Windows 11.

**Role in FluentOS:** DWMBlurGlass enhances the visual coherence of FluentOS by providing modern blur and transparency effects that complement the light/dark themes and overall design language.

## Status in v0.1

- **Availability:** Optional (not required for Core edition)
- **Integration:** Basic skeleton; effect tuning TODO for v0.2+
- **Stability:** DWMBlurGlass is actively developed; FluentOS integration is POC-phase

## Key Features

- **Window Blur Effects:** Apply Aero-style blur to window backgrounds and borders
- **Customizable Intensity:** Fine-tune blur strength per visual element
- **Performance-conscious:** Designed to minimize impact on GPU and battery
- **Global Toggle:** Enable/disable all effects system-wide with one setting

## Installation

### Automatic (via FluentOS installer)

```powershell
.\scripts/install/winget.ps1
# Select "yes" when prompted for DWMBlurGlass installation
```

### Manual

1. Download from [GitHub: australiern/DWMBlurGlass](https://github.com/australiern/DWMBlurGlass/releases)
2. Extract to a permanent directory (e.g., `C:\Program Files\DWMBlurGlass`)
3. Run `DWMBlurGlass.exe`
4. Enable effects and adjust settings

## Configuration

TODO: Add detailed effect configuration examples

- Effect types: Window blur, taskbar blur, Start Menu blur, notification blur
- Intensity settings: Custom per-element blur strength (0–100%)
- Corner radius: Window corner effect customization
- Advanced options: Custom effect profiles, per-application settings

## Performance Considerations

- Blur effects have minimal GPU impact on modern systems
- May increase power consumption on laptops with older GPUs
- Disable blur if system is unstable or performance suffers
- Test on your specific hardware before full deployment

## Known Issues

- TODO: Document DWMBlurGlass-specific limitations for v0.1
- May not work optimally on some integrated GPUs
- Some older GPU drivers may have compatibility issues
- Blur effects may not render correctly with 4K displays on some systems

## Compatibility

- **Supported:** Windows 11 22H2 and later (including 25H2)
- **GPU:** NVIDIA, AMD, Intel Iris; older integrated GPUs may have limited support
- **Conflicts:** May have visual issues with some third-party theme engines

## Uninstall

```powershell
# Option 1: Run DWMBlurGlass.exe > Disable > Exit, then delete directory
# Option 2: Via Windows Settings > Apps (if installed as app)
# Option 3: Via full FluentOS rollback
.\scripts/uninstall/rollback.ps1 -Full
```

## Further Resources

- [DWMBlurGlass GitHub](https://github.com/australiern/DWMBlurGlass)
- [GitHub Releases (Latest Builds)](https://github.com/australiern/DWMBlurGlass/releases)
- [Windows 11 Aero Glass Effects](https://support.microsoft.com/en-us/windows)
