# FluentOS Editions

FluentOS comes in three editions, each tailored to different use cases and organizational scales.

---

## FluentOS Core

**Target:** Power users, enthusiasts, individual productivity.

**Purpose:**
A cohesive, visually modern UX layer for Windows 11, emphasizing personal productivity and aesthetic polish.

**Scope:**
- Desktop theming (light/dark profiles)
- Taskbar and Start Menu customization
- Window decoration (via Seelen or DWMBlurGlass)
- Explorer navigation enhancements
- Personal productivity tweaks

**Excluded:**
- Active Directory integration
- Group Policy configuration
- Multi-machine deployment automation
- Organizational branding (placeholder support only)
- Specialized role profiles

**Edition-specific features:**
- Minimal footprint
- Simple one-click installation
- Light/dark theme toggle
- Personal customization settings

---

## FluentOS Business

**Target:** Small-to-mid organizations, standardized workstation deployments.

**Purpose:**
A professionally configured UX layer with light policy enforcement, enabling organizations to deploy cohesive, maintainable workstations quickly.

**Scope:**
- All Core features
- Light Group Policy integration (non-domain scenarios)
- Company branding (logo, colors, welcome screens)
- Fast, repeatable workstation setup scripts
- Basic role profiles (e.g., standard user, power user)
- Service optimization (disable unnecessary services)
- Compliance documentation

**Excluded:**
- Deep Active Directory integration
- Enterprise MDM/Intune configuration
- Multi-site governance
- Specialized departmental profiles

**Edition-specific features:**
- Company branding and customization
- Light policy templates
- Automated setup with minimal manual steps
- Standardized application stacks
- Basic audit and rollback capabilities

---

## FluentOS Fleet

**Target:** Large organizations, many-machine deployments, complex role-based governance.

**Purpose:**
A comprehensive UX and policy framework for deploying and maintaining consistent experiences across hundreds or thousands of machines, with support for multiple organizational roles.

**Scope:**
- All Core and Business features
- Full Group Policy support (domain and non-domain)
- Advanced role profiles: Accounting, Reception, Management, Direction (C-suite), Development, etc.
- Multi-site organizational structure
- Centralized configuration management
- Machine rollout and lifecycle automation
- Advanced auditing, logging, and compliance tracking
- Integration with Intune/Azure AD
- Patch management and update coordination
- Performance monitoring and reporting

**Excluded:**
- Custom kernel modifications
- Bypass of licensing or security features
- Redistribution of proprietary Windows binaries

**Edition-specific features:**
- Role-based configuration profiles with fine-grained customization
- Centralized management console or dashboard
- Advanced rollback and disaster recovery
- Fleet-wide monitoring and health checks
- Integration with enterprise identity and device management systems
- Compliance and security audit reports

---

## Edition Comparison

| Feature | Core | Business | Fleet |
|---------|------|----------|-------|
| Desktop theming | ✓ | ✓ | ✓ |
| Taskbar/Start customization | ✓ | ✓ | ✓ |
| Window decoration | ✓ | ✓ | ✓ |
| Explorer tweaks | ✓ | ✓ | ✓ |
| Company branding | – | ✓ | ✓ |
| Light policy support | – | ✓ | ✓ |
| Role profiles | – | Basic | Advanced (5+) |
| Service optimization | – | ✓ | ✓ |
| Active Directory integration | – | Light | Full |
| Multi-site governance | – | – | ✓ |
| Intune/Azure AD integration | – | – | ✓ |
| Centralized management | – | – | ✓ |
| Audit & compliance | – | Basic | Advanced |
| Fleet monitoring | – | – | ✓ |

---

**Next Step:** See [roadmap.md](roadmap.md) for the version timeline and planned availability of each edition.
