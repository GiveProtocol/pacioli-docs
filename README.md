# Pacioli Documentation

**Official documentation for Pacioli - Open-source crypto accounting platform for Polkadot**

🌐 **Live Documentation**: [docs.pacioli.io](https://docs.pacioli.io)
🏠 **Main Repository**: [GiveProtocol/pacioli-core](https://github.com/GiveProtocol/pacioli-core)

## Overview

This repository contains the comprehensive documentation for Pacioli, covering everything from getting started to advanced developer guides and API references.

## Documentation Structure

```
pacioli-docs/
├── user-guide/              # End-user documentation
│   ├── getting-started.md
│   ├── faq.md
│   └── ...
├── developer-guide/         # Developer documentation
│   ├── architecture.md
│   ├── local-development.md
│   ├── contributing.md
│   └── plugin-development.md
├── crypto-operations/       # Blockchain-specific guides
│   ├── POLKADOT_REFERENCE.md
│   ├── evm-chains.md
│   └── wallet-connections.md
├── tutorials/               # Step-by-step tutorials
│   ├── first-transaction.md
│   ├── multi-wallet-setup.md
│   └── creating-reports.md
├── self-hosting/            # Self-hosting guides
│   ├── installation.md
│   ├── configuration.md
│   └── DEPLOYMENT.md
├── api-reference/           # API documentation
│   ├── rest-api.md
│   ├── rust-api.md
│   └── plugin-api.md
├── implementation-guides/   # Technical implementation docs
│   ├── CRYPTO_ACCOUNTING_IMPLEMENTATION.md
│   ├── CURRENCY_ARCHITECTURE.md
│   └── CURRENCY_IMPLEMENTATION_GUIDE.md
└── index.md                 # Documentation home page
```

## Contributing to Documentation

We welcome contributions to improve our documentation! Whether it's fixing typos, clarifying explanations, or adding new guides, your help is appreciated.

### Quick Start

1. **Fork this repository**

2. **Clone your fork:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/pacioli-docs.git
   cd pacioli-docs
   ```

3. **Create a branch:**
   ```bash
   git checkout -b docs/your-improvement
   ```

4. **Make your changes** and test locally (see below)

5. **Commit and push:**
   ```bash
   git commit -m "docs: describe your changes"
   git push origin docs/your-improvement
   ```

6. **Open a Pull Request** on GitHub

### Writing Guidelines

#### Style Guide

- **Use clear, concise language** - avoid jargon when possible
- **Include code examples** - show, don't just tell
- **Add screenshots** for UI-related documentation
- **Link to related docs** - help users navigate
- **Keep it up-to-date** - verify accuracy against latest code

#### Markdown Format

- Use **ATX-style headers** (#, ##, ###)
- Include **code fences** with language specifiers:
  ````markdown
  ```typescript
  const example = "code here"
  ```
  ````
- Add **front matter** for Jekyll (if applicable)
- Follow **semantic line breaks** (one sentence per line in source)

#### File Naming

- Use **lowercase with hyphens**: `my-new-guide.md`
- Be **descriptive**: `wallet-connection-guide.md` not `guide1.md`
- Group related docs in appropriate directories

## Local Development

### Option 1: Jekyll (GitHub Pages)

```bash
# Install Jekyll
gem install bundler jekyll

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# View at http://localhost:4000
```

### Option 2: Simple HTTP Server

```bash
# Python 3
python3 -m http.server 8000

# Node.js
npx http-server

# View at http://localhost:8000
```

## Documentation Types

### User Guide
- **Target audience**: End users who want to use Pacioli
- **Focus**: How to accomplish tasks, step-by-step workflows
- **Example**: "How to track your first transaction"

### Developer Guide
- **Target audience**: Contributors who want to build or extend Pacioli
- **Focus**: Architecture, setup, contribution process
- **Example**: "Setting up local development environment"

### API Reference
- **Target audience**: Developers integrating with Pacioli
- **Focus**: Complete API specifications, parameters, responses
- **Example**: "POST /api/transactions - Create a new transaction"

### Tutorials
- **Target audience**: All users learning specific features
- **Focus**: Learning by doing, complete walkthrough
- **Example**: "Creating your first multi-currency report"

## Documentation Hosting

### GitHub Pages

This documentation is hosted on GitHub Pages at `docs.pacioli.io`.

**Configuration:**
- **Site generator**: Jekyll
- **Theme**: Just the Docs (or custom theme)
- **Base URL**: `/`
- **Custom domain**: `docs.pacioli.io`

To update the live site, simply merge changes to the `main` branch. GitHub Actions will automatically rebuild and deploy.

### Jekyll Configuration

The `_config.yml` file contains Jekyll configuration:

```yaml
title: Pacioli Documentation
description: Official documentation for Pacioli crypto accounting
baseurl: "" # for GitHub Pages
url: "https://docs.pacioli.io"
```

## Documentation Versioning

- **Main branch** - Latest documentation (matches main repo)
- **Version tags** - Documentation for specific releases (e.g., `v0.1.0`)
- **Legacy docs** - Archived in `docs/legacy/`

## Getting Help

- **General questions**: [GitHub Discussions](https://github.com/GiveProtocol/pacioli-core/discussions)
- **Documentation issues**: [File an issue](https://github.com/GiveProtocol/pacioli-docs/issues)
- **Community forum**: https://community.pacioli.io

## License

This documentation is licensed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**, consistent with the main Pacioli project.

See [LICENSE](LICENSE) for the full license text.

---

**Built with ❤️ by the Pacioli community**
