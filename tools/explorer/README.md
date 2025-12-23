# Windows Explorer Customizations

## Overview

**Windows Explorer** is the primary file manager in Windows 11. FluentOS includes a collection of tweaks and enhancements to make Explorer more cohesive with the overall FluentOS visual design and user experience.

**Role in FluentOS:** Explorer customizations address navigation, visual consistency, and productivity improvements. They bridge the gap between system UI and user workflows.

## Status in v0.1

- **Availability:** Integrated into core installation (always included)
- **Integration:** Basic skeleton; detailed tweaks TODO for v0.2+
- **Stability:** Registry-based modifications; generally safe and reversible

## Customizations Included

TODO: Implement detailed Explorer tweaks for v0.1–v0.2

### Planned Customizations

**Visual Enhancements:**
- [ ] Quick Access customization (pinned folders, toolbar organization)
- [ ] Thumbnail size and preview settings optimization
- [ ] Font and spacing adjustments for better readability
- [ ] Color scheme alignment with theme (light/dark)

**Behavioral Improvements:**
- [ ] File sorting and grouping defaults (by name, date, type)
- [ ] Default view settings (Details view, icon size, layout)
- [ ] Ribbon visibility and customization
- [ ] Details pane behavior and information display

**Navigation Enhancements:**
- [ ] Quick navigation toolbar customization
- [ ] Address bar improvements
- [ ] Breadcrumb navigation styling
- [ ] Search bar refinements

## Configuration

### Quick Access Customization

TODO: Add configuration steps for v0.2

Current approach (manual):
1. Open Explorer
2. Right-click "Quick Access" folders
3. Organize by moving, pinning, or hiding items

### View Settings

```powershell
# TODO: Implement Explorer view configuration via registry
# Set default view to Details
# Set icon size to Medium
# Enable breadcrumb navigation
```

### Ribbon and Interface

TODO: Add ribbon customization details

## Known Limitations in v0.1

- [ ] Ribbon modifications not yet implemented
- [ ] Some view settings may reset after Windows Updates
- [ ] Custom toolbar buttons not supported in v0.1
- [ ] Search indexing optimizations TODO

## Advanced Customizations (Future)

TODO for Business and Fleet editions:
- [ ] Custom context menu items
- [ ] Explorer extension integration
- [ ] Group Policy-based configurations (Business/Fleet)
- [ ] Cloud integration customization (OneDrive, SharePoint)
- [ ] Advanced file preview handlers

## Rollback

All Explorer customizations are reversible:

```powershell
# Restore Explorer defaults
.\scripts/uninstall/rollback.ps1

# Or manually:
# 1. Open Settings > System > Restore
# 2. Use System Restore point
```

## Related Tools

- [ExplorerPatcher](https://github.com/valinet/ExplorerPatcher) – Advanced Explorer tweaks (for reference)
- [Open Shell](https://github.com/Open-Shell/Open-Shell-Menu) – Classic menu and customizations (alternative)

## Further Resources

- [Microsoft Explorer Documentation](https://support.microsoft.com/en-us/windows/open-file-explorer)
- [Windows Registry Reference](https://learn.microsoft.com/en-us/windows/win32/sysinfo/structure-of-the-registry)
