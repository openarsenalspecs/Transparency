# RepoHub Specification (RHS)

A modular, AI-assisted specification for creating repository hubs that aggregate, organize, and document publicly available information about software repositories, projects, specifications, websites, and associated resources.

The RepoHub Specification (RHS) defines a vendor-neutral standard for building centralized repository directories capable of automatically discovering repositories, categorizing projects, establishing relationships between projects, and generating structured metadata, documentation indexes, analytics, and knowledge graphs.

The specification is designed to improve the discoverability, interoperability, and long-term preservation of open-source ecosystems while maintaining human oversight and avoiding vendor lock-in.

---

# Objectives

- Create centralized repository hubs.
- Aggregate publicly available project information.
- Automatically categorize repositories and projects.
- Generate structured metadata and documentation.
- Build knowledge graphs and project relationships.
- Preserve provenance and source attribution.
- Support AI-assisted ecosystem discovery and analysis.
- Enable interoperability between repository hub implementations.
- Provide long-term preservation of open-source ecosystems.

---

# Design Principles

- Modular architecture
- Vendor neutrality
- Platform agnostic
- Human-in-the-loop governance
- Local-first compatibility
- Extensible schemas
- Privacy respecting data collection
- Public information only
- No vendor lock-in
- Machine-readable outputs
- Long-term preservation

---

# Supported Sources

- Codeberg
- GitLab
- GitHub
- Forgejo
- Gitea
- Self-hosted Git services
- Personal websites
- Documentation websites
- Wikis
- Package registries
- Public social profiles
- Project directories
- Specification websites

---

# Modules

## Identity Module

Collects and indexes publicly available user and organization information.

### Files

- identity.json
- profiles.json
- accounts.json
- organizations.json

## Repository Discovery Module

Discovers repositories and associated projects.

### Files

- repositories.json
- organizations.json
- mirrors.json
- forks.json

## Categorization Module

Automatically groups repositories into categories.

### Files

- categories/

## Association Module

Creates relationships between projects and repositories.

### Files

- relationships.json
- dependency-graph.json
- related-projects.json

## Website Module

Indexes websites associated with repositories.

### Files

- websites.json
- documentation.json

## Pricing Module

Records optional commercial information.

### Files

- pricing.json
- services.json

## Provenance Module

Tracks data origin, attribution, and verification.

### Files

- provenance/sources.json
- provenance/crawl-log.json
- provenance/attribution.json
- provenance/confidence.json
- provenance/verification.json

## License Intelligence Module

Records licensing information and compatibility.

### Files

- licenses/licenses.json
- licenses/compatibility.json
- licenses/attribution.json
- licenses/copyright.json

## Documentation Module

Indexes all publicly available documentation.

### Files

- documentation/documentation.json
- documentation/readmes.json
- documentation/wikis.json
- documentation/api-docs.json
- documentation/tutorials.json

## Analytics Module

Provides ecosystem metrics and reporting.

### Files

- analytics/analytics.json
- analytics/statistics.json
- analytics/trends.json
- analytics/reports.json

## Funding Module

Records sponsorship and support information.

### Files

- funding/funding.json
- funding/sponsors.json
- funding/donations.json
- funding/services.json

## Security Module

Indexes security information and advisories.

### Files

- security/security.json
- security/advisories.json
- security/vulnerabilities.json
- security/disclosure.json

## AI Knowledge Module

Creates machine-readable representations of the ecosystem.

### Files

- knowledge/knowledge-graph.json
- knowledge/ontology.json
- knowledge/entities.json
- knowledge/embeddings.json
- knowledge/relationships.json

## Timeline Module

Tracks historical events and repository evolution.

### Files

- timeline/timeline.json
- timeline/milestones.json
- timeline/history.json
- timeline/releases.json

## Repository Quality Module

Measures project health and maintenance indicators.

### Files

- quality/quality.json
- quality/health.json
- quality/maintenance.json
- quality/scores.json

---

# Feature List

- Modular and extensible architecture
- AGPL-3.0+ licensed specification
- Vendor-neutral implementation requirements
- Human-in-the-loop governance
- Local-first compatible deployments
- Multi-platform repository support
- Public data aggregation and indexing
- Automated repository discovery
- Repository categorization and classification
- AI-assisted metadata generation
- Repository relationship mapping
- Dependency graph generation
- Associated website linking
- Documentation indexing and aggregation
- Optional pricing and service information
- Repository search and filtering
- Structured metadata generation
- Repository hub generation
- Project and specification registries
- Cross-repository association mapping
- Public profile aggregation
- Technology stack identification
- Source attribution and provenance tracking
- Data lineage and verification records
- Confidence scoring of accumulated information
- Historical crawl logging
- License detection and analysis
- SPDX license identification
- License compatibility analysis
- Attribution requirement tracking
- Documentation and API indexing
- Wiki and tutorial aggregation
- Analytics and ecosystem reporting
- Repository and category statistics
- Language and technology metrics
- Trend analysis and reporting
- Funding and sponsorship tracking
- Donation and support information indexing
- Consulting and commercial offering tracking
- Security policy indexing
- Vulnerability and advisory tracking
- Responsible disclosure information
- Security metadata aggregation
- AI knowledge graph generation
- Ontology generation
- Semantic search support
- Embedding generation
- Machine-readable ecosystem intelligence
- AI agent interoperability support
- Timeline and historical event tracking
- Repository lifecycle monitoring
- Release and milestone tracking
- Project evolution history
- Repository quality scoring
- Maintenance health assessment
- Documentation completeness scoring
- Community engagement metrics
- Dependency health analysis
- Test coverage tracking
- Incremental updates and synchronization
- Export and import capabilities
- Structured JSON metadata generation
- Markdown directory generation
- Sitemap generation
- Manual editing and correction support
- Audit and verification capabilities
- Long-term ecosystem preservation
- Open ecosystem interoperability
- No vendor-lock-in requirements

---

# Implementation Requirements

Implementations of the RepoHub Specification:

- MUST collect only publicly available information.
- MUST preserve source attribution.
- MUST maintain provenance records.
- MUST support manual corrections.
- MUST support incremental updates.
- MUST generate machine-readable metadata.
- MUST permit human review of generated information.
- MUST support modular implementation.
- SHOULD support semantic search.
- SHOULD support knowledge graph generation.
- SHOULD support export and import capabilities.

---

# Recommended Directory Structure

- analytics/
- categories/
- documentation/
- funding/
- knowledge/
- licenses/
- pricing/
- profiles/
- provenance/
- quality/
- relationships/
- repositories/
- security/
- specifications/
- timeline/
- websites/
- DIRECTORY.md
- INDEX.md
- README.md
- hub.json

---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/openarsenal/](https://roxanneardary.com/openarsenal/)

---

## License & Notice Requirements

Open Arsenal is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Open Arsenal specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
