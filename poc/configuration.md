# FluentOS v0.1 POC – Configuration

## Overview

FluentOS v0.1 provides basic configuration through:
- **Theme profiles** (JSON files in `scripts/profiles/`)
- **PowerShell parameters** (in installation and configuration scripts)
- **Registry modifications** (applied via tweaks.ps1 or manual registry editing)

## Theme Profiles

### What are Theme Profiles?

Theme profiles are JSON files that define:
- Visual theme (light or dark)
- Color scheme (accent colors, background colors)
- Typography settings (font families, sizes)
- UX behavior (animations, transitions)
- Tool-specific configurations (Seelen layouts, Windhawk mods)

### Available Profiles in v0.1

**FluentOS Core – Light**
- File: `scripts/profiles/fluentos-core-light.json`
- Description: Light theme optimized for daytime use
- Includes: Soft whites, light grays, colorful accents

**FluentOS Core – Dark**
- File: `scripts/profiles/fluentos-core-dark.json`
- Description: Dark theme optimized for reduced eye strain
- Includes: Deep blacks, dark grays, muted accents

### Applying a Profile

TODO: Implement profile application function

```powershell
# Load and apply a profile
Import-FluentOSProfile -Path "scripts/profiles/fluentos-core-light.json"
```

### Creating a Custom Profile

Copy an existing profile and modify:

1. Start with `fluentos-core-light.json`
2. Change the `name` field
3. Modify `settings` values as desired
4. Save to `scripts/profiles/your-custom-profile.json`
5. Apply with `Import-FluentOSProfile`

TODO: Add detailed profile schema documentation

## Configuration Areas

### 1. Visual Customization

**Modifiable elements:**
- Desktop background (wallpaper)
- Accent color (used in taskbar, Start Menu, highlights)
- Window decoration (border colors, blur intensity)
- Icon pack (if using community icon sets)

**How to adjust:**
- Edit the `settings.visual` section in your theme profile
- Or use Windows Settings → Personalization → Colors

TODO: Add example visual configurations

### 2. Taskbar & Start Menu

**Modifiable elements:**
- Taskbar position (bottom, top, auto-hide)
- Start Menu layout (grid density, grouping)
- Button styling (icons, text, size)
- Transparency and blur effects

**How to adjust:**
- Edit `settings.taskbar` in theme profile
- Or use Windows Settings → Personalization → Taskbar

TODO: Add example taskbar configurations and custom layouts

### 3. Windowing Behavior

**Modifiable elements (if Seelen installed):**
- Window snapping behavior (tiling, floating)
- Keyboard shortcuts for window management
- Virtual desktop management
- Focus and mouse following

**How to adjust:**
- Edit `settings.windowing` in theme profile
- Or configure Seelen directly (see [../tools/seelen/README.md](../tools/seelen/README.md))

TODO: Add example windowing configurations

### 4. Optional Tools Configuration

**Seelen** (window manager):
- Configuration: `~/.seelen/seelen.yaml`
- TODO: Document configuration schema

**Windhawk** (UX patcher):
- Configuration: Via Windhawk UI or registry
- TODO: Document available mods and defaults for FluentOS

**DWMBlurGlass** (blur effects):
- Configuration: Via DWMBlurGlass settings
- TODO: Document blur intensity and effect tuning

## Registry-Based Configuration

### Viewing Current Registry Settings

```powershell
# View all FluentOS-related registry keys
Get-ItemProperty -Path "HKCU:\Software\FluentOS"
```

### Modifying Registry Values

**WARNING:** Incorrect registry modifications can cause system instability. Always backup your registry first.

```powershell
# Backup
Export-RegReg -Path "HKCU:\Software\FluentOS" -Path "C:\Backups\fluentos-registry-backup.reg"

# Modify
Set-ItemProperty -Path "HKCU:\Software\FluentOS\Theme" -Name "DarkMode" -Value 1
```

TODO: Add safe registry modification helpers and validation

## Resetting to Defaults

To reset a specific configuration area:

```powershell
# Reset theme to Light (default)
Reset-FluentOSTheme -Theme "Light"

# Reset Taskbar to defaults
Reset-FluentOSTaskbar

# Full reset to Windows 11 defaults
.\scripts/uninstall/rollback.ps1
```

TODO: Implement reset functions

---

## Next Steps

- See [known-limitations.md](known-limitations.md) for current constraints
- See [../docs/editions.md](../docs/editions.md) for edition-specific configurations (v0.2+)
- See [../tools/](../tools/) for tool-specific configuration guides
