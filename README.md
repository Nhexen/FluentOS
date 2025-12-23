<div align="center">

<img src="docs/assets/FluentOS.png" alt="FluentOS Logo" width="200" height="auto">

# FluentOS

**A modern UX layer for Windows 11**  
*Coherence • Readability • Productivity*

[![Status](https://img.shields.io/badge/Status-POC-orange?style=for-the-badge)](docs/roadmap.md)
[![Version](https://img.shields.io/badge/Version-0.1.0-0078D4?style=for-the-badge)](docs/roadmap.md)
[![License](https://img.shields.io/badge/License-MIT-50C878?style=for-the-badge)](LICENSE)
[![Windows](https://img.shields.io/badge/Windows-11+-0078D4?style=for-the-badge&logo=windows11&logoColor=white)](https://www.microsoft.com/en-us/windows/windows-11)
[![GitHub Issues](https://img.shields.io/github/issues/codixia/fluentos?style=for-the-badge&logo=github)](https://github.com/codixia/fluentos/issues)

---

</div>

## About FluentOS

FluentOS is **not** a custom Windows build, fork, or security bypass. It is a curated set of:

- ✨ **UX Presets & Configurations** — Cohesive visual design and behavior
- 🚀 **PowerShell Automation** — Reproducible, scriptable installations
- 🛠️ **Third-Party Integrations** — Seelen, Windhawk, DWMBlurGlass, Explorer customizations
- 📋 **Policy Guidelines** — Best practices for organizational deployments

This v0.1 POC establishes the foundation and vision for what FluentOS will become in v1.0 and beyond.

## 🎯 Quick start

| Resource | Link |
|----------|------|
| **Vision & Goals** | [📖 docs/vision](docs/vision.md) |
| **Installation** | [⚙️ poc/installation](poc/installation.md) |
| **Requirements** | [📋 poc/requirements](poc/requirements.md) |
| **Roadmap** | [🗺️ docs/roadmap](docs/roadmap.md) |
| **Legal** | [⚖️ docs/legal](docs/legal.md) |

## 📦 Repository structure

```
fluentos/
├── docs/               # 📚 Documentation & Vision
│   ├── vision.md       # What FluentOS is (and isn't)
│   ├── scope.md        # What's in scope / out of scope
│   ├── non-goals.md    # Explicit non-goals
│   ├── editions.md     # Core, Business, Fleet editions
│   ├── roadmap.md      # v0.1 → v1.0 timeline
│   └── legal.md        # Licensing & legal framework
│
├── poc/                # 🧪 POC Documentation
│   ├── requirements.md
│   ├── installation.md
│   ├── configuration.md
│   └── known-limitations.md
│
├── scripts/            # 🔧 Installation & Configuration
│   ├── install/        # winget.ps1, tweaks.ps1, services.ps1
│   ├── uninstall/      # rollback.ps1
│   └── profiles/       # JSON theme presets
│
├── tools/              # 🛠️ Third-Party Tool Guides
│   ├── seelen/         # Window manager integration
│   ├── windhawk/       # UX patcher integration
│   ├── dwmblurglass/   # Blur effects integration
│   └── explorer/       # Explorer customizations
│
├── LICENSE             # MIT License
└── README.md           # This file
```

## 🚀 Editions

FluentOS comes in **three editions**, each tailored to different scales:

| Edition | Target | Use Case |
|---------|--------|----------|
| **Core** | 👤 Individuals | Personal Windows 11 enhancement |
| **Business** | 🏢 SMBs | Standardized workstation deployments |
| **Fleet** | 🏭 Enterprise | Multi-machine governance & management |

→ [Learn more about editions](docs/editions.md)

## ⚠️ Project status

This **v0.1 POC is not production-ready**. It serves to:

1. **Define** the vision and scope
2. **Establish** the organizational structure  
3. **Outline** the approach for v0.2+ iterations

Current limitations and known issues are documented in [poc/known-limitations](poc/known-limitations.md).

## 🗺️ Roadmap

<img src="docs/assets/roadmap_info.png" alt="Roadmap" width="900" height="auto">

→ [Full roadmap with details](docs/roadmap.md)

## 🤝 Contributing

FluentOS is open source and welcomes contributions. Areas of interest:

- 📚 Documentation improvements
- 🐛 Bug reports and fixes
- ✨ Theme enhancements
- 🔧 Script improvements
- 📦 Tool integration guides

## 📄 License

FluentOS is released under the **MIT License**. See [LICENSE](LICENSE) for full details.

**Key Points:**
- ✅ Use freely on systems you own or manage
- ✅ Modify and distribute per MIT terms
- ❌ Cannot circumvent Windows licensing
- ❌ Cannot claim Microsoft affiliation

## ⚖️ Legal

FluentOS respects Microsoft licensing and operates through supported APIs only. 
→ [Legal framework & compliance](docs/legal.md)

---

<div align="center">

**[Docs](docs/) • [Issues](https://github.com/codixia/fluentos/issues) • [License](LICENSE)**

*Last updated: December 2025*  
*Maintained / Owned by [Codixia](https://github.com/codixia)*

</div>