# Solution Design Document (SDD) — Mansion Docs

## 1. System Topology
Mansion Docs is architected as a static site generated via Docusaurus (React-based documentation framework):
1. **Docusaurus Core Engine**: Compiles markdown, MDX components, and metadata into an optimized static single-page application bundle.
2. **Algolia / Local Search**: Client-side document indexing for rapid keyword navigation across user guides, roles, and administrative manuals.
3. **GitHub Pages Edge Hosting**: Globally distributed static delivery served at `https://masssolution.github.io/mansion-docs/`.

## 2. Content & Routing Architecture
- **Intro & Getting Started**: `docs/getting-started/` guides tenant provisioning and initial workspace configuration.
- **Role-Based Guides**: `docs/roles/` delineates responsibilities for Administrators, Project Managers, and Contractors.
- **Administration & Governance**: `docs/administration/` covers license tiers, audit logs, and security controls.
- **Release Documentation**: `releases/` archives platform release notes and migration instructions.
