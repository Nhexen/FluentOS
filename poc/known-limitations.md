# FluentOS v0.1 POC – Known Limitations

## Current Status

FluentOS v0.1 is a **Proof of Concept (POC)**, not production-ready. This document lists current limitations and planned improvements.

## Limitations

### 1. Not Production-Ready

- **Status:** POC phase
- **Impact:** Use only for testing and evaluation
- **Mitigation:** Always test on non-critical systems first; maintain backups
- **Timeline to Fix:** v1.0 (planned Q1 2027)

### 2. Limited Rollback Coverage

- **Issue:** Automatic rollback may not fully restore all system state
- **Affected Areas:**
  - Third-party tool installations (Seelen, Windhawk, DWMBlurGlass) require manual uninstallation
  - Some registry modifications may persist
  - User-customized settings may not be recovered
- **Workaround:** Keep a full system backup before installation
- **Timeline to Fix:** v0.3+ (planned Q2 2026+)

### 3. Visual Consistency Across Systems

- **Issue:** Themes may render differently depending on:
  - GPU capabilities (especially blur effects)
  - Display scaling and DPI settings
  - System font renderings and antialiasing
  - Third-party UI overlays or accessibility tools
- **Affected Areas:** Window decorations, transparency, text rendering
- **Workaround:** Adjust profile settings for your specific hardware
- **Timeline to Fix:** v0.2 (refinement), v1.0 (optimization)

### 4. Limited Theme Variety

- **Current Offering:** Light and Dark profiles only
- **Missing:** High-contrast, seasonal, or role-specific themes (Business/Fleet)
- **Timeline to Add:** v0.2–v0.3

### 5. No Active Directory / Group Policy Support

- **Status:** Not available in v0.1
- **Impact:** Enterprise deployments not yet supported
- **Timeline to Add:** v0.3 (Business Ready), v0.5+ (Fleet)

### 6. Tool Integration Not Comprehensive

**Seelen:**
- Tiling layouts are basic; advanced window rules not yet defined
- Keyboard shortcuts may conflict with other apps

**Windhawk:**
- Only a minimal set of mods are pre-configured
- Custom mod lists not yet supported in profiles

**DWMBlurGlass:**
- Blur effects may cause performance issues on low-end GPUs
- Compatibility with some third-party themes not fully tested

**Timeline to Fix:** v0.2 (core integration), v0.3+ (advanced features)

### 7. No Multi-Language Support

- **Status:** English only
- **Timeline to Add:** v1.0+

### 8. Documentation Incomplete

- **Status:** v0.1 has skeleton documentation with TODO markers
- **Missing:** Detailed configuration examples, troubleshooting, advanced customization
- **Timeline to Complete:** v0.2+

### 9. Performance Not Optimized

- **Impact:** Installation may take longer than expected; boot times may increase slightly
- **Affected by:** Number of enabled tools, system specs, network speed
- **Timeline to Optimize:** v0.2+

### 10. Limited Testing Coverage

- **Status:** Tested on select configurations only
- **May Not Work Well On:**
  - ARM-based Windows 11 (Surface Pro X, etc.)
  - Heavily customized Windows 11 installations
  - Systems with third-party security software
  - Low-spec hardware (< 4 GB RAM, HDD-only, older GPUs)
- **Timeline to Expand:** v0.2+

## Workarounds & Recommendations

### For Current Users

1. **Always backup** before installation (full system image or registry export)
2. **Test on a VM** or non-critical machine first
3. **Keep administrator access** for troubleshooting and rollback
4. **Monitor system** for unexpected behavior after installation
5. **Report issues** on GitHub to help improve future versions

### For Specific Limitations

| Limitation | Workaround |
|-----------|-----------|
| Limited rollback | Maintain full system backup; use System Restore point before install |
| Visual inconsistencies | Manually tweak profile JSON for your hardware |
| Tool conflicts | Disable conflicting tools or applications; test one tool at a time |
| Performance issues | Reduce number of enabled tools; check GPU drivers; upgrade hardware if needed |
| Documentation gaps | Check GitHub issues for user-reported solutions; contribute docs as you learn |

## Roadmap to Stability

- **v0.2:** Improve consistency and core feature refinement
- **v0.3:** Add business-ready features and better rollback
- **v0.4+:** Advanced features and hardening
- **v1.0:** Stable, well-documented, production-ready

---

**Last Updated:** December 2025  
**Current Version:** v0.1 POC

For bug reports and feature requests, visit [GitHub Issues](https://github.com/codixia/fluentos/issues).
