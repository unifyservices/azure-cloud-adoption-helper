# Azure Cloud Adoption Helper

[![CAF Aligned](https://img.shields.io/badge/CAF-Aligned-0078d4)](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/)
[![WAF v2](https://img.shields.io/badge/WAF-v2-3fb950)](https://learn.microsoft.com/en-us/azure/well-architected/)
[![Offline Ready](https://img.shields.io/badge/Offline-Ready-50e6ff)](https://github.com/unifyservices/azure-cloud-adoption-helper)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)

> A fully offline, single-file HTML tool for Azure cloud adoption planning. No backend, no dependencies, no installation. Open in any browser and start planning.

**Built by [Unify Services](https://unifyservices.io) — Azure Architecture & Cloud Consulting**

---

## What Is This?

A standalone HTML tool that gives cloud architects, engineers, and consultants seven integrated planning tools grounded in the **Microsoft Cloud Adoption Framework (CAF)** and **Well-Architected Framework (WAF)**.

Everything runs in your browser. No data leaves your machine. Works offline.

## Features — 7 Integrated Tools

### 🏷️ Tab 1: Naming Convention Generator
- 78+ Azure resource types with CAF abbreviations
- Pattern: `{abbr}-{prefix}-{workload}-{env}-{region}-{instance}`
- Real-time validation (length limits, allowed characters, case rules)
- Bulk landing zone name generator — select multiple types, generate all at once
- Save and export naming sheets as **CSV or JSON**
- CAF abbreviation reference table with search

### 🌐 Tab 2: IP Address & CIDR Planner
- Add multiple VNets with name, CIDR, role (Hub/Spoke/Standalone), and region
- Subnet calculator: usable IPs, first/last IP, subnet mask, Azure 5-reserved-IP rule
- **Overlap detection** — real-time check across all VNets and subnets
- Quick CIDR calculator — paste any CIDR to instantly see all details
- One-click **presets**: Small, Medium, Large Hub-Spoke, Sandbox
- CAF IP planning best practices panel
- Export as **JSON or CSV**

### 🔖 Tab 3: Tagging Strategy Builder
- Design your organization's tagging taxonomy
- Pre-loaded templates: CAF Minimum, Extended Enterprise, FinOps, Security
- Required/optional flag, allowed values, enforcement effect (Deny/Audit/Modify)
- **Azure Policy JSON generator** — auto-generates policy rule snippets per tag
- Tag validator — paste a JSON resource object to validate against your schema
- Tag coverage matrix
- Export as **JSON, CSV, Azure Policy JSON, or Markdown table**

### 🏗️ Tab 4: Landing Zone Planner
- Visual **management group hierarchy** builder
- Pre-loaded **CAF Azure Landing Zone (ALZ)** reference template
- Add management groups and subscriptions with budget and owner tracking
- Subscription inventory table
- Export as **JSON, Markdown, or Terraform skeleton**

### ✅ Tab 5: Well-Architected Review Checklist
- **60 questions** across all 5 WAF pillars
- Reliability, Security, Cost Optimization, Operational Excellence, Performance Efficiency
- Real-time per-pillar scoring and **SVG radar chart**
- Recommendations shown for every unchecked item
- Export as **JSON or CSV**

### 💰 Tab 6: Quick Cost Estimator
- Pre-built templates: Basic Web App, Hub Network, AKS Microservices, Data Platform
- 20+ resource types with multiple SKU tiers and approximate monthly pricing
- Reserved Instance discount, Azure Hybrid Benefit, Dev/Test pricing toggles
- Cost breakdown by category with visual bar chart
- Export as **CSV or JSON**

### 🛡️ Tab 7: Governance Policy Catalog
- 22+ recommended Azure Policy definitions (Naming, Tagging, Region, Compute, Networking, Storage, Security, Monitoring)
- Browse and filter by category and effect (Deny/Audit/Modify/DeployIfNotExists)
- Policy rule JSON preview for each policy
- **Initiative builder** — select policies and export as an Azure Policy Initiative JSON or **Terraform skeleton**

---

## Quick Start

```bash
# Clone the repository
git clone https://github.com/unifyservices/azure-cloud-adoption-helper.git
cd azure-cloud-adoption-helper

# Open in your browser (no server needed)
open index.html      # macOS
start index.html     # Windows
xdg-open index.html  # Linux
```

That's it. No `npm install`. No Python server. No build step.

## Data Persistence

All your work is automatically saved to **browser localStorage**. It persists across page reloads. Use the Export buttons to save data externally.

## Use Cases

| Role | How They Use It |
|------|----------------|
| **Cloud Architect** | Generate naming standards for an entire landing zone deployment in minutes |
| **Network Engineer** | Plan VNet and subnet address spaces with overlap detection before deployment |
| **Governance Lead** | Design tagging taxonomy and auto-generate Azure Policy definitions |
| **Security Architect** | Run WAF Security pillar assessment and export findings |
| **FinOps Analyst** | Quick-estimate architecture costs before building a detailed business case |
| **Project Manager** | Plan management group hierarchy and subscription layout for a new workload |

## Standards Alignment

| Framework | Coverage |
|-----------|---------|
| [Microsoft Cloud Adoption Framework](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/) | Naming, IP Planning, Landing Zone, Tagging, Governance |
| [Azure Well-Architected Framework v2](https://learn.microsoft.com/en-us/azure/well-architected/) | All 5 pillars, 60 checklist questions |
| [CAF Azure Landing Zone](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ready/landing-zone/) | ALZ management group reference hierarchy |
| [Azure Naming Rules](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/resource-name-rules) | Per-resource length, character, and case rules |
| [CAF IP Addressing](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-best-practices/plan-for-ip-addressing) | Subnet sizing, reserved IPs, hub-spoke topology |

## Project Structure

```
azure-cloud-adoption-helper/
├── index.html     # Complete application — all HTML, CSS, and JavaScript
├── README.md
└── LICENSE        # Apache 2.0
```

## Contributing

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

Ideas for contributions:
- Additional Azure resource types and CAF abbreviations
- More WAF checklist questions
- Additional governance policies
- Azure region updates
- Price data updates

## License

Apache 2.0 — Free to use, modify, and distribute with attribution.

---

**Built by [Unify Services](https://unifyservices.io)** — Enterprise Azure Architecture, Migration, Security & FinOps in UAE/GCC

*Need help with Azure landing zone design, cloud migration, or governance frameworks? [Get in touch](https://unifyservices.io/contact)*
