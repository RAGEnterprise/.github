# RAGEnterprise Organization Structure

## Repository Overview

The RAGEnterprise organization manages the RAGOS Linux ecosystem through a modular repository structure. Each repository has a specific purpose and contributes to the overall system.

## Repository Structure

### Core System Repositories

#### ragos-repo
**Purpose:** Binary package repository  
**Description:** Hosts pre-compiled packages and binaries for RAGOS Linux. This is the central package distribution point for the system.

#### ragos-iso
**Purpose:** Official RAGOS ISO build  
**Description:** Contains the build system and configurations for creating official RAGOS Linux ISO images. This is where releases are generated.

#### ragosctl
**Purpose:** Declarative CLI tool  
**Description:** Command-line interface tool for managing RAGOS Linux in a declarative manner. This is the primary user-facing tool for system configuration and management.

#### ragos-modules
**Purpose:** System modules (like NixOS modules)  
**Description:** Contains system modules that provide declarative configuration options. Similar to NixOS modules, these enable modular and composable system configurations.

#### ragos-home
**Purpose:** Declarative user environment manager  
**Description:** Manages user-level configurations and environments in a declarative way. This allows users to define their personal environment settings reproducibly.

### Branding and Documentation

#### ragos-branding
**Purpose:** Visual assets and branding materials  
**Description:** Contains wallpapers, icons, logos, and other design assets for RAGOS Linux. This ensures consistent visual identity across the project.

#### ragos-docs
**Purpose:** Official documentation  
**Description:** Comprehensive documentation for RAGOS Linux, including user guides, developer documentation, and system reference materials.

### Installation and Setup

#### ragos-installer
**Purpose:** Minimalist installer based on ragosctl  
**Description:** A streamlined installation system that leverages ragosctl for system setup. Provides an easy way to install RAGOS Linux on new machines.

### Organization Configuration

#### .github
**Purpose:** Global organization configurations  
**Description:** Contains organization-wide GitHub configurations, workflows, templates, and documentation. This repository also includes:
- Organization profile (`profile/README.md`)
- GitHub Copilot rules and guidelines
- Shared CI/CD workflows
- Issue and PR templates

## Development Guidelines

### Repository Naming Convention
All repositories follow the `ragos-*` or `ragosctl` naming pattern for consistency and easy identification.

### Declarative Philosophy
RAGOS Linux follows a declarative approach to system management, inspired by systems like NixOS. Repositories should maintain this philosophy in their design and implementation.

### Modularity
Each repository should have a clear, single purpose. Cross-repository dependencies should be well-documented and minimal.

## Getting Started

To contribute to any RAGOS Linux project:

1. Review the specific repository's README and contributing guidelines
2. Familiarize yourself with the declarative approach used throughout the ecosystem
3. Join the community channels (Discord, Matrix, Telegram - links in organization profile)
4. Submit issues and pull requests following the organization templates

## Architecture Diagram

```
RAGEnterprise/
 ├── ragos-repo/              → Binary package repository
 ├── ragos-iso/               → Official RAGOS ISO build
 ├── ragosctl/                → Declarative CLI tool
 ├── ragos-modules/           → System modules (like NixOS modules)
 ├── ragos-home/              → Declarative user environment manager
 ├── ragos-branding/          → Wallpapers, icons, logos, and assets
 ├── ragos-docs/              → Official documentation
 ├── ragos-installer/         → Minimalist installer based on ragosctl
 └── .github/                 → Global organization configurations
      └── copilot/
          └── enterprise-rules.md
```

## Support and Community

For questions, support, or discussions:
- Check the `ragos-docs` repository for comprehensive documentation
- Open issues in the relevant repository
- Join community channels (coming soon)

---

*This document serves as the authoritative reference for the RAGEnterprise organization structure and repository purposes.*
