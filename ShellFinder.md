# ShellFinder
*Where Hidden Companies Come to Light*

---

## Overview

ShellFinder is an open-source forensic AI platform designed to map, analyze, and reconstruct the corporate ecosystems surrounding OTC companies.

ShellFinder follows the principle of **following the people, relationships, assets, and transactions rather than relying solely on stock tickers**. The platform builds interconnected profiles of companies, founders, officers, directors, shareholders, subsidiaries, assets, filings, legal events, and other publicly available information.

The system is designed as a modular platform. Core modules provide the foundational corporate intelligence, entity resolution, financial analysis, knowledge graph, AI analysis, and investigative capabilities. Optional plugin modules allow additional data sources, jurisdictions, analytical models, and specialized investigative capabilities to be added without changing the core platform.

---

## Core Objectives

ShellFinder is designed to:

- Build comprehensive profiles of OTC companies.
- Reconstruct corporate histories from incorporation through the present.
- Identify founders, officers, directors, and other corporate participants.
- Track relationships between people and companies across time.
- Map subsidiaries, affiliates, ownership interests, and corporate relationships.
- Track publicly disclosed securities transactions and ownership changes.
- Identify share issuance, dilution, and capital structure changes.
- Map disclosed real estate, intellectual property, equipment, and other assets.
- Connect companies and individuals to publicly available legal and regulatory records.
- Detect unusual patterns, anomalies, and corporate network relationships.
- Preserve historical versions of corporate relationships and events.
- Provide AI-assisted investigation and research tools.
- Maintain evidence and source provenance for generated findings.
- Support open-source community research and independent verification.

---

# Architecture

ShellFinder uses a modular architecture consisting of:

1. **Core Platform**
2. **Core Intelligence Modules**
3. **Core Data Modules**
4. **AI Analysis Modules**
5. **Investigation and Visualization Modules**
6. **Optional Plugin Modules**
7. **API and Integration Layer**

The core system provides the foundational capabilities required to operate ShellFinder. Plugins extend the platform with additional data sources and specialized functionality.

---

# Core Platform

## 1. Data Ingestion Module

The Data Ingestion Module manages the collection and normalization of publicly available information.

### Capabilities

- SEC filing ingestion
- OTC market data ingestion
- Corporate registry ingestion
- Public company disclosures
- Court and legal records
- Regulatory records
- Public property records
- Patent and trademark records
- Public news and press releases
- Public social media data where permitted
- Historical document ingestion
- Scheduled data collection
- Incremental updates
- Duplicate detection
- Source metadata preservation

Every imported record should retain its original source, retrieval date, document identifier, and applicable provenance information.

---

## 2. Corporate Identity Module

The Corporate Identity Module establishes the canonical identity of every company tracked by ShellFinder.

### Capabilities

- Legal company name
- Former company names
- Ticker symbols
- Former ticker symbols
- Trading symbols
- Jurisdiction of incorporation
- Incorporation date
- Corporate status
- Corporate addresses
- Registered agents
- Subsidiaries
- Parent companies
- Affiliates
- Successor entities
- Predecessor entities
- Mergers
- Acquisitions
- Reverse mergers
- Corporate reorganizations
- Corporate name changes

The module maintains historical identities rather than replacing historical records when a company changes its name or ticker.

---

## 3. Founder & Leadership Module

The Founder & Leadership Module creates historical profiles of individuals associated with companies.

### Capabilities

- Founders
- Incorporators
- Original directors
- Officers
- Current directors
- Former directors
- Executives
- Controlling persons
- Significant shareholders where publicly disclosed
- Beneficial owners where publicly disclosed
- Executive tenure
- Board tenure
- Historical positions
- Relationships between executives and companies

ShellFinder distinguishes between **verified founders**, **documented early officers**, and **AI-inferred relationships** so that conclusions are not presented as established facts without supporting evidence.

---

## 4. Entity Resolution Module

The Entity Resolution Module connects records that may represent the same person, company, address, or organization.

### Capabilities

- Name normalization
- Corporate name matching
- Historical company matching
- Individual identity matching
- Address matching
- Registered-agent matching
- Officer overlap detection
- Director overlap detection
- Subsidiary matching
- Corporate successor matching
- Duplicate record detection
- Confidence scoring
- Human verification workflows

Entity resolution must preserve uncertainty rather than automatically treating a probabilistic match as a confirmed identity.

---

## 5. Corporate Genealogy Module

The Corporate Genealogy Module reconstructs the historical lineage of companies.

### Capabilities

- Company origin tracking
- Name-change history
- Ticker history
- Reverse merger reconstruction
- Acquisition history
- Spin-offs
- Corporate reorganizations
- Successor and predecessor relationships
- Historical leadership
- Historical ownership
- Corporate lineage timelines

Users can reconstruct the state of a corporate entity at a particular point in time.

---

## 6. Ownership & Securities Module

The Ownership & Securities Module tracks publicly disclosed ownership and securities information.

### Capabilities

- Insider transactions
- Forms 3, 4, and 5 where applicable
- Beneficial ownership disclosures
- Institutional ownership where available
- Share issuance
- Outstanding shares
- Authorized shares
- Dilution events
- Convertible securities
- Warrants
- Options where disclosed
- Restricted securities
- Stock-based compensation
- Ownership changes
- Capital structure changes

The module records the source document supporting each ownership or transaction record.

---

## 7. Financial Intelligence Module

The Financial Intelligence Module analyzes publicly disclosed financial information.

### Capabilities

- Revenue analysis
- Expense analysis
- Cash analysis
- Debt analysis
- Liabilities
- Assets
- Equity
- Cash-flow analysis
- Related-party transactions
- Inter-company transactions
- Revenue concentration
- Share issuance analysis
- Dilution analysis
- Financial trend analysis
- Capital structure analysis
- Historical financial comparisons

ShellFinder does not treat financial indicators as proof of misconduct. Analytical results are presented as signals requiring verification.

---

## 8. Asset Intelligence Module

The Asset Intelligence Module maps publicly disclosed or legally accessible information about company and related-party assets.

### Capabilities

- Real estate
- Property ownership
- Property addresses
- Property transfers
- Intellectual property
- Patents
- Trademarks
- Copyright information where available
- Equipment
- Inventory
- Vehicles
- Vessels
- Aircraft
- Mining or industrial assets
- Asset transfers
- Asset relationships

Asset records include source provenance and confidence information.

---

## 9. Legal & Regulatory Intelligence Module

The Legal & Regulatory Intelligence Module connects companies and individuals with publicly available legal and regulatory records.

### Capabilities

- Federal litigation
- State litigation
- Bankruptcy records
- Regulatory actions
- SEC enforcement records
- FINRA actions
- CFTC actions
- Administrative proceedings
- Judgments
- Liens where legally accessible
- Settlements
- Corporate compliance events
- Regulatory filing deficiencies
- Legal-document extraction
- Legal timeline reconstruction

Legal records are presented as documented events and should not be interpreted by ShellFinder as proof of wrongdoing unless the underlying record establishes that conclusion.

---

## 10. Address & Geographic Intelligence Module

The Address & Geographic Intelligence Module analyzes relationships between companies, people, and physical locations.

### Capabilities

- Corporate addresses
- Registered-agent addresses
- Executive addresses where legally available
- Shared corporate addresses
- Shared registered-agent addresses
- Property locations
- Geographic clustering
- Corporate concentration by jurisdiction
- Historical address changes
- Address reuse detection
- Geographic relationship graphs

The system should apply privacy and legal restrictions to personal-address data and avoid exposing sensitive information unnecessarily.

---

## 11. Knowledge Graph Module

The Knowledge Graph Module connects ShellFinder's entities and events into an interconnected corporate graph.

### Core Nodes

- Company
- Person
- Founder
- Officer
- Director
- Shareholder
- Subsidiary
- Parent company
- Asset
- Property
- Filing
- Transaction
- Security
- Court case
- Regulatory action
- Address
- Intellectual property
- Organization
- News event

### Core Relationships

- founded_by
- incorporated_by
- officer_of
- director_of
- shareholder_of
- owns
- beneficially_owns
- subsidiary_of
- parent_of
- successor_of
- predecessor_of
- merged_with
- acquired
- acquired_by
- located_at
- registered_at
- filed
- disclosed_in
- involved_in
- transferred_to
- shares_address_with
- mentioned_in

All graph relationships should support dates, sources, confidence levels, and provenance.

---

## 12. Historical Snapshot Module

The Historical Snapshot Module allows users to reconstruct the known state of a company or network at a specific point in time.

### Capabilities

- Historical company profiles
- Historical officer lists
- Historical board composition
- Historical ownership
- Historical ticker information
- Historical subsidiaries
- Historical assets
- Historical filings
- Historical transactions
- Historical network graphs
- Point-in-time investigations

This prevents current information from overwriting historically relevant information.

---

# AI Core Modules

## 13. Document Intelligence Module

Uses AI-assisted extraction to convert unstructured documents into structured records.

### Capabilities

- PDF parsing
- Filing extraction
- Table extraction
- Named entity recognition
- Company identification
- Person identification
- Address extraction
- Transaction extraction
- Ownership extraction
- Relationship extraction
- Document classification
- Document summarization

AI-generated information must retain links to the underlying source material.

---

## 14. Relationship Analysis Module

The Relationship Analysis Module analyzes connections across the knowledge graph.

### Capabilities

- Founder networks
- Officer networks
- Board networks
- Corporate clusters
- Shared-address networks
- Shared-agent networks
- Ownership networks
- Subsidiary networks
- Asset networks
- Cross-company relationships
- Temporal relationship analysis
- Network centrality
- Cluster detection

---

## 15. Anomaly Detection Module

The Anomaly Detection Module identifies unusual patterns for further investigation.

### Capabilities

- Unusual share issuance
- Sudden ownership changes
- Unusual filing activity
- Rapid corporate restructuring
- Repeated officer transitions
- Repeated address usage
- Unusual financial changes
- Unexpected asset transfers
- Network expansion anomalies
- Trading-volume anomalies where appropriate data is available

Anomaly detection produces **investigative signals**, not accusations.

---

## 16. Pattern Analysis Module

The Pattern Analysis Module compares historical corporate behavior across companies and networks.

### Capabilities

- Repeated corporate structures
- Repeated leadership patterns
- Recurring registered agents
- Recurring addresses
- Repeated merger structures
- Similar corporate filings
- Similar capital structures
- Similar transaction patterns
- Historical pattern matching
- Cross-company similarity analysis

---

## 17. AI Investigation Assistant

The AI Investigation Assistant allows users to query ShellFinder using natural language.

### Example Queries

- "Show all companies associated with this founder."
- "Which officers have served on both boards?"
- "Show the corporate history of this ticker."
- "What companies share this registered address?"
- "Show the ownership changes over the last ten years."
- "Which subsidiaries are connected to this company?"
- "Show all documented legal actions involving this company."
- "Reconstruct this company's network as of 2018."
- "Show unusual changes in share issuance."
- "Find relationships between these two companies."

The assistant should distinguish between:

- Verified facts
- Source-derived information
- Probabilistic relationships
- AI-generated analysis
- User-submitted information

---

# Investigative Modules

## 18. Risk Signal Module

The Risk Signal Module organizes measurable indicators into transparent analytical categories.

### Signals May Include

- Reporting history
- Corporate structure changes
- Ownership changes
- Dilution
- Related-party transactions
- Legal events
- Regulatory events
- Officer network concentration
- Repeated corporate relationships
- Unusual financial changes
- Asset transfers
- Trading anomalies

Risk signals should be explainable and traceable to their underlying evidence.

---

## 19. Timeline Module

Provides chronological views of corporate activity.

### Events

- Incorporation
- Name changes
- Ticker changes
- Founder appointments
- Officer changes
- Board changes
- Mergers
- Acquisitions
- Financing events
- Share issuances
- Insider transactions
- Asset transfers
- Lawsuits
- Regulatory actions
- Bankruptcy events
- Major filings

---

## 20. Watchlist & Alert Module

Users can monitor entities and receive alerts when relevant events occur.

### Watchlists

- Companies
- Tickers
- Founders
- Officers
- Directors
- Shareholders
- Assets
- Addresses
- Corporate networks

### Alerts

- New filing
- Officer change
- Director change
- Ownership change
- Insider transaction
- Share issuance
- Corporate name change
- Ticker change
- Merger
- Acquisition
- Legal action
- Regulatory action
- New corporate relationship
- New asset relationship
- Significant anomaly

---

## 21. Reporting Module

Generates structured investigative reports.

### Reports

- Company profile
- Founder profile
- Officer profile
- Corporate genealogy
- Ownership report
- Asset report
- Legal history
- Financial history
- Network analysis
- Historical snapshot
- Risk signal report
- Investigation report

### Export Formats

- Markdown
- HTML
- JSON
- CSV
- PDF
- GraphML

---

# Visualization Modules

## 22. Corporate Network Visualization

Interactive visualization of:

**Person → Company → Subsidiary → Asset → Filing → Transaction → Legal Event**

Features include:

- Interactive graphs
- Relationship filtering
- Date filtering
- Entity filtering
- Source filtering
- Confidence filtering
- Network expansion
- Network clustering

---

## 23. Geographic Visualization

Displays corporate and asset relationships geographically.

### Features

- Company locations
- Registered-agent locations
- Property locations
- Corporate clusters
- Geographic timelines
- Jurisdiction analysis

---

## 24. Financial Visualization

### Features

- Historical price data where available
- Trading volume
- Share issuance
- Dilution
- Ownership changes
- Revenue
- Debt
- Assets
- Cash
- Financial trends

---

# Evidence & Provenance

## 25. Source Provenance Module

Every significant ShellFinder record should be traceable to its underlying source.

### Provenance Data

- Source
- Source URL where permitted
- Document identifier
- Filing date
- Retrieval date
- Source type
- Extracted text
- Supporting passage or location
- Data transformation history
- Confidence level
- Verification status

ShellFinder should never silently transform uncertain information into established fact.

---

## 26. Evidence Verification Module

Allows users and contributors to review AI-generated relationships and claims.

### Verification States

- Unverified
- AI identified
- Source supported
- Human verified
- Disputed
- Rejected
- Superseded

Users should be able to inspect the evidence supporting a relationship or claim.

---

## 27. Dataset Versioning Module

Maintains historical versions of the ShellFinder dataset.

### Capabilities

- Dataset snapshots
- Record history
- Change tracking
- Correction history
- Contributor attribution
- Source updates
- Rollbacks
- Historical comparisons

---

# Community Modules

## 28. Research Contribution Module

Allows researchers to contribute:

- Sources
- Corrections
- Corporate relationships
- Historical information
- Documents
- Entity matches
- Research notes
- Verification results

Contributions should retain contributor attribution and an audit history.

---

## 29. Community Verification Module

Allows contributors to review disputed or uncertain records.

### Features

- Evidence review
- Correction requests
- Verification workflows
- Dispute records
- Contributor history
- Source comparison
- Moderation tools

---

# API Layer

## 30. API Module

ShellFinder provides programmatic access to its data and analytical capabilities.

### API Capabilities

- Company lookup
- Person lookup
- Founder lookup
- Officer lookup
- Ownership lookup
- Asset lookup
- Filing lookup
- Legal event lookup
- Network queries
- Historical snapshots
- Search
- Alerts
- Reports
- Graph queries

API access should enforce appropriate rate limits and permissions.

---

# Optional Plugin Architecture

ShellFinder's core functionality remains independent from optional external integrations.

Plugins can extend the system without requiring changes to the core modules.

## Plugin Types

### Data Source Plugins

Examples:

- Additional securities markets
- Additional corporate registries
- International registries
- Property databases
- Court databases
- Patent databases
- Trademark databases
- News providers
- Public social platforms

### Jurisdiction Plugins

Add support for:

- Canadian corporate records
- United Kingdom corporate records
- European corporate records
- Asia-Pacific corporate records
- Additional U.S. state records

### Intelligence Plugins

Examples:

- Advanced financial models
- Specialized anomaly detection
- Network analysis
- Sentiment analysis
- Document classification
- Specialized entity resolution
- Industry-specific intelligence

### Asset Plugins

Examples:

- Aircraft registries
- Vessel registries
- Vehicle registries
- Mining records
- Environmental records
- Zoning records
- Intellectual property systems

### Visualization Plugins

Examples:

- Advanced graph visualizations
- Geographic dashboards
- Three-dimensional network views
- Time-lapse networks
- Specialized financial charts

### AI Model Plugins

Support alternative:

- Local AI models
- Hosted AI models
- Embedding models
- OCR models
- Document models
- Classification models
- Entity-resolution models

Plugins should use defined interfaces and must not compromise the provenance, security, or integrity of the core system.

---

# Plugin Requirements

Optional plugins should:

- Have a defined manifest.
- Declare their data sources.
- Declare required permissions.
- Preserve source provenance.
- Follow ShellFinder's data model.
- Provide documentation.
- Include tests.
- Identify licensing restrictions.
- Respect source terms of use.
- Avoid silently modifying core records.
- Clearly distinguish plugin-generated analysis from verified source data.

---

# Data Integrity Principles

ShellFinder follows several foundational principles:

### Source First

Important claims should be traceable to their underlying sources.

### Evidence Over Inference

AI inference must be distinguishable from documented facts.

### Historical Preservation

Historical information should not be overwritten by current information.

### Confidence Matters

Entity relationships should have confidence levels.

### Transparent Analysis

Risk signals should be explainable.

### Correction Friendly

Users should be able to challenge and correct records.

### No Automatic Accusations

Patterns and anomalies are investigative signals, not determinations of fraud, criminal conduct, or wrongdoing.

---

# Privacy & Responsible Data Use

ShellFinder is designed around publicly available and legally accessible information.

The platform should:

- Respect applicable privacy laws.
- Respect data-source terms of use.
- Minimize unnecessary exposure of personal information.
- Avoid publishing sensitive personal information when it is not necessary.
- Distinguish public corporate information from personal information.
- Provide correction and dispute mechanisms where appropriate.
- Preserve source context.
- Avoid presenting allegations as established facts.

---

# Security

ShellFinder should implement:

- Secure API authentication
- Role-based access control
- Audit logging
- Data validation
- Source integrity checks
- Secure plugin isolation
- Dependency scanning
- Secrets management
- Rate limiting
- Input validation
- Database access controls

---

# Technology Architecture

ShellFinder is designed to support a replaceable technology stack.

Potential components include:

- Python for data processing and AI services
- PostgreSQL for structured data
- Graph database for relationship analysis
- OpenSearch or equivalent for document search
- Object storage for source documents
- React-based dashboard
- Graph visualization framework
- REST and GraphQL APIs
- Docker for deployment
- Local AI models for privacy-preserving analysis

Specific implementations may change without changing the underlying ShellFinder specification.

---

# Deployment Models

ShellFinder can support multiple deployment configurations.

### Local Deployment

Designed for individual researchers and private investigations.

### Self-Hosted Deployment

Organizations can operate their own ShellFinder instance and data infrastructure.

### Research Deployment

Universities, journalists, and independent researchers can operate specialized installations.

### Enterprise Deployment

Organizations can deploy ShellFinder with controlled access, private data sources, and specialized plugins.

---

# Core vs Optional Functionality

The ShellFinder architecture separates foundational capabilities from specialized integrations.

## Core

- Corporate identity
- Founder and leadership mapping
- Entity resolution
- Corporate genealogy
- Ownership and securities
- Financial intelligence
- Asset intelligence
- Legal intelligence
- Knowledge graph
- AI document analysis
- Relationship analysis
- Anomaly detection
- Historical reconstruction
- Provenance
- Investigation tools
- Reporting
- API
- Dashboard
- Community verification

## Optional Plugins

- Additional markets
- International jurisdictions
- Specialized registries
- Additional property systems
- Specialized legal databases
- Social data providers
- News providers
- Advanced AI models
- Specialized financial models
- Additional asset registries
- Advanced visualization systems
- Industry-specific intelligence

This separation allows ShellFinder to remain modular, maintainable, and extensible while allowing users to build specialized investigative environments.

---

# Contributing

Contributions are welcome from developers, researchers, data scientists, journalists, and other contributors interested in improving corporate transparency and investigative technology.

Please review `CONTRIBUTING.md` before submitting changes.

Contributions should prioritize:

- Verifiable information
- Reproducible analysis
- Source attribution
- Data integrity
- Privacy
- Security
- Clear documentation
- Test coverage

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
  - [https://roxanneardary.com/shellfinder/](https://roxanneardary.com/shellfinder/)

---

## License & Notice Requirements

ShellFinder is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- ShellFinder specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
