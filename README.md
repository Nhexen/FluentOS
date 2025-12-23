# FluentOS v0.1 – POC

A modern UX layer for Windows 11, focusing on coherence, readability, and productivity.

## Overview

FluentOS is **not** a custom Windows build, fork, or security bypass. It is a curated set of:
- UX presets and configurations
- PowerShell installation and configuration scripts
- Third-party tool integrations (Seelen, Windhawk, DWMBlurGlass, Explorer customizations)
- Policy and personalization guidelines

This v0.1 POC establishes the skeletal structure and vision for what FluentOS will become.

## Quick Links

- **Vision & Goals**: see [docs/vision.md](docs/vision.md)
- **Installation**: see [poc/installation.md](poc/installation.md)
- **Requirements**: see [poc/requirements.md](poc/requirements.md)
- **Roadmap**: see [docs/roadmap.md](docs/roadmap.md)

## Repository Structure

```
fluentos/
├─ docs/          # Documentation: vision, scope, roadmap, legal
├─ poc/           # POC-specific docs: requirements, setup, limitations
├─ scripts/       # Installation and configuration scripts
│  ├─ install/    # Winget, tweaks, services setup
│  ├─ uninstall/  # Rollback scripts
│  └─ profiles/   # JSON presets (light/dark themes)
├─ tools/         # Third-party tool integration guides
└─ LICENSE        # MIT License
```

## For v0.1

This POC is **not production-ready**. It serves to:
1. Define the vision and scope
2. Establish the organizational structure
3. Outline the approach for v0.2+ iterations

See [docs/roadmap.md](docs/roadmap.md) for planned versions and milestones.

---

**Last updated**: December 2025  
**Status**: POC – v0.1
