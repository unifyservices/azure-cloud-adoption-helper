# Contributing to Azure Cloud Adoption Helper

Thank you for your interest in contributing!

## How to Contribute

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/your-feature`)
3. **Make your changes** to `index.html`
4. **Test** by opening `index.html` in Chrome, Firefox, and Edge
5. **Submit** a Pull Request with a clear description

## Contribution Ideas

- New Azure resource types (add to `RESOURCE_TYPES` array)
- Updated pricing data (update `COST_RESOURCES` array)
- New WAF checklist questions (add to `WAF_PILLARS` array)
- Additional governance policies (add to `POLICIES` array)
- New Azure regions (update region dropdowns)
- UI improvements and bug fixes

## Code Standards

- All changes go in `index.html` — keep it as a single self-contained file
- No external dependencies (no CDN links, no npm packages)
- Test offline (disconnect network before testing)
- Follow existing JavaScript patterns (plain ES6+, no frameworks)

## Confidentiality

Do not include any client-specific data, internal IPs, or proprietary configurations.
