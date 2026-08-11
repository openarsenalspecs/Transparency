# Ledger Watch

**Public data, structured for analysis.**

Ledger Watch is an open-source financial transparency and market intelligence specification for collecting, verifying, normalizing, connecting, and analyzing publicly available information about financial trades, market participants, companies, financial instruments, corporate actions, and related events.

Ledger Watch is designed as a modular system. The **Core Modules** provide the foundational infrastructure required for a functional Ledger Watch implementation. **Optional Plugin Modules** extend the system with additional data sources, markets, analytical capabilities, interfaces, and integrations without requiring changes to the core architecture.

The system is designed around a fundamental principle:

> **Public data, structured for analysis.**

Ledger Watch does not attempt to determine intent or declare wrongdoing. It records verifiable public information, identifies documented relationships and statistical patterns, preserves source provenance, and provides users with the evidence and analytical tools necessary to conduct their own research.

---

# Specification

## Design Goals

Ledger Watch is designed to provide:

- Public financial transparency
- Verifiable trade records
- Source-backed entity profiles
- Company and institutional activity tracking
- Market event correlation
- Historical financial timelines
- Statistical pattern detection
- Data provenance and verification
- Reproducible analysis
- Machine-readable financial records
- Human-readable research interfaces
- Open APIs
- Modular data ingestion
- Extensible analytics
- Auditability
- Vendor independence
- Open-source interoperability

---

# Modular Architecture

Ledger Watch consists of three architectural layers:

## Core Modules

Core Modules provide the minimum functionality required for a Ledger Watch implementation.

Core modules include:

- Identity and Entity Registry
- Public Trade Registry
- Financial Instrument Registry
- Source Verification
- Filing and Disclosure Registry
- Corporate Activity Registry
- Event Registry
- Relationship Engine
- Correlation Engine
- Anomaly Analysis
- Provenance and Audit
- Timeline Engine
- Search and Query
- API
- Access and Administration

## Optional Plugin Modules

Plugin Modules provide additional functionality that can be installed independently.

Examples include:

- SEC EDGAR Connector
- CFTC Data Connector
- Congressional Disclosure Connector
- International Regulatory Connector
- News Intelligence Connector
- Market Price Connector
- Options Analytics
- Commodity Analytics
- ETF Analytics
- Cryptocurrency Analytics
- Graph Database Connector
- Machine Learning Analytics
- Natural Language Processing
- Geographic Intelligence
- Alerting
- Visualization
- Research Workbench
- Data Export
- Public API Gateway

Plugins must communicate with the core through documented interfaces and must not require proprietary infrastructure.

---

# Core Module: Identity and Entity Registry

The Identity and Entity Registry provides the canonical identity system for Ledger Watch.

The registry supports:

- Individuals
- Public companies
- Private companies where publicly documented financial activity exists
- Investment funds
- Hedge funds
- Asset managers
- Pension funds
- Government entities
- Public officials
- Corporate insiders
- Institutional investors
- Financial institutions
- Brokers and intermediaries where publicly documented
- Financial instruments

Each entity may contain:

- Canonical name
- Legal name
- Known names
- Entity type
- Regulatory identifiers
- CIK
- LEI
- Ticker symbols
- Exchange identifiers
- Government identifiers
- Parent organization
- Subsidiaries
- Affiliates
- Historical names
- Source references
- Verification status
- Effective dates

Entity records must distinguish between verified identity information and unresolved identity relationships.

---

# Core Module: Public Trade Registry

The Public Trade Registry stores publicly disclosed financial transactions and positions.

Supported records may include:

- Purchases
- Sales
- Transfers
- Acquisitions
- Dispositions
- Short positions
- Position changes
- Institutional holdings
- Insider transactions
- Corporate securities transactions
- Commodity positions
- Other publicly disclosed financial activity

Each trade record should contain, where available:

- Trade identifier
- Reporting entity
- Instrument
- Transaction type
- Transaction date
- Filing date
- Quantity
- Price
- Currency
- Transaction value
- Position before transaction
- Position after transaction
- Transaction status
- Source
- Source document
- Source location
- Verification status
- Data confidence
- Ingestion timestamp

Ledger Watch must distinguish between:

- Actual reported transactions
- Reported positions
- Derived calculations
- Estimated values
- Analytical interpretations

Derived information must never be represented as an original reported fact.

---

# Core Module: Financial Instrument Registry

The Financial Instrument Registry provides canonical identities for financial assets.

Supported instruments include:

- Common stocks
- Preferred stocks
- ETFs
- Mutual funds
- Bonds
- Options
- Futures
- Commodities
- Commodity contracts
- Indices
- Digital assets where supported by an installed plugin
- Other publicly documented financial instruments

Instrument records may include:

- Symbol
- Exchange
- ISIN
- CUSIP where legally available
- FIGI where available
- Asset class
- Issuer
- Currency
- Market
- Contract specifications
- Effective dates
- Historical symbols
- Corporate action history

---

# Core Module: Source Verification

Source Verification is a foundational Ledger Watch capability.

Every material financial record should maintain provenance to its source.

Sources may include:

- Government filings
- Regulatory databases
- Exchange disclosures
- Corporate filings
- Official company disclosures
- Public government records
- Public institutional disclosures
- Licensed data sources
- Other independently verifiable public records

Each source record should include:

- Source organization
- Source type
- Source identifier
- Source location
- Publication date
- Retrieval date
- Document hash where practical
- Verification state
- Parser version
- Ingestion process
- Modification history

The system should preserve the distinction between the original source and Ledger Watch's normalized representation.

---

# Core Module: Filing and Disclosure Registry

The Filing and Disclosure Registry organizes regulatory and corporate disclosures.

Supported filing categories include:

- Insider transaction filings
- Institutional holdings filings
- Annual reports
- Quarterly reports
- Current reports
- Proxy statements
- Beneficial ownership disclosures
- Corporate transaction disclosures
- Public financial disclosures

The registry provides:

- Filing indexing
- Filing classification
- Entity association
- Instrument association
- Filing version tracking
- Filing timestamps
- Document provenance
- Filing-to-trade relationships

---

# Core Module: Corporate Activity Registry

Companies are first-class entities in Ledger Watch.

The Corporate Activity Registry tracks publicly disclosed corporate activity including:

- Share buybacks
- Share issuance
- Dividends
- Stock splits
- Reverse splits
- Mergers
- Acquisitions
- Divestitures
- Spin-offs
- Debt issuance
- Capital raises
- Earnings releases
- Guidance changes
- Material announcements
- Executive changes
- Major litigation disclosures
- Regulatory actions
- Other material corporate events

Corporate activity can be connected to:

- Company entities
- Executives
- Insiders
- Financial instruments
- Trades
- Market events

---

# Core Module: Event Registry

The Event Registry provides a normalized representation of events that may be relevant to financial activity.

Events may include:

- Corporate announcements
- Earnings releases
- Regulatory decisions
- Government actions
- Economic releases
- Monetary policy decisions
- Legislative events
- Legal proceedings
- Industry events
- Commodity events
- Market-wide events
- Publicly reported news events

Each event should contain:

- Event identifier
- Event type
- Event timestamp
- Publication timestamp
- Affected entities
- Affected instruments
- Source
- Source document
- Event description
- Verification state
- Related filings
- Related trades

---

# Core Module: Relationship Engine

The Relationship Engine connects entities, instruments, filings, trades, and events.

Relationships may include:

- Individual works for company
- Fund manages capital
- Company issues instrument
- Entity owns instrument
- Entity trades instrument
- Filing reports trade
- Filing concerns company
- Event affects instrument
- Event concerns entity
- Trade precedes event
- Trade follows event
- Corporate action affects instrument

Relationships must contain provenance and confidence information when they are derived rather than directly reported.

---

# Core Module: Correlation Engine

The Correlation Engine identifies temporal and statistical relationships between public financial activity and documented events.

The system may evaluate:

- Trade-to-event timing
- Event-to-price movement
- Trade size relative to historical behavior
- Trading frequency
- Repeated event relationships
- Position changes
- Cross-entity activity
- Sector-level activity
- Market-wide activity

Correlation results must clearly distinguish:

- Observed facts
- Statistical relationships
- Derived metrics
- Interpretive conclusions

Ledger Watch must never automatically represent statistical correlation as causation.

---

# Core Module: Anomaly Analysis

The Anomaly Analysis module identifies activity that differs materially from an entity's historical baseline or from relevant comparison groups.

Potential metrics include:

- Timing deviation
- Position-size deviation
- Frequency deviation
- Historical activity deviation
- Market-relative deviation
- Sector-relative deviation
- Event proximity
- Cross-entity clustering
- Repeated pattern frequency

Anomaly scores must be explainable.

A score should be decomposable into the underlying factors that produced it.

The system must avoid automatically labeling an entity or transaction as:

- Illegal
- Corrupt
- Fraudulent
- Manipulative
- Insider trading
- Criminal

unless such a determination is explicitly documented by an authoritative public source and is represented as a sourced external finding rather than a Ledger Watch conclusion.

---

# Core Module: Timeline Engine

The Timeline Engine reconstructs chronological relationships between financial activity and public events.

A timeline may display:

- Trade
- Filing
- Disclosure
- Corporate event
- News event
- Market movement
- Subsequent transaction

Timeline records should preserve exact timestamps whenever available and identify the precision of dates where only a date rather than an exact time is publicly available.

---

# Core Module: Provenance and Audit

The Provenance and Audit module provides the accountability layer of Ledger Watch.

It records:

- Source retrieval
- Data ingestion
- Data normalization
- Entity resolution
- Transformation
- Analytical processing
- Record corrections
- Record versioning
- Administrative changes
- Plugin activity

Where practical, source documents should be cryptographically hashed to provide integrity verification.

Historical records should not be silently overwritten.

Corrections should preserve an audit trail.

---

# Core Module: Search and Query

Ledger Watch provides structured search across:

- People
- Companies
- Funds
- Instruments
- Trades
- Filings
- Events
- Corporate actions
- Relationships
- Anomalies
- Sources

Users should be able to query questions such as:

- Who publicly reported buying an instrument?
- Which companies are associated with a specific trader?
- Which institutions changed their holdings?
- What public events occurred around a transaction?
- Which entities repeatedly traded before specific event types?
- What filings document a transaction?
- What source supports a particular record?

---

# Core Module: API

Ledger Watch should provide a documented API for accessing structured data.

The API should support:

- Entity lookup
- Trade lookup
- Filing lookup
- Event lookup
- Instrument lookup
- Corporate activity lookup
- Relationship queries
- Timeline queries
- Correlation queries
- Anomaly queries
- Provenance queries

API responses should expose source provenance whenever applicable.

---

# Core Module: Access and Administration

The administrative system provides:

- User management
- Role management
- API credentials
- Plugin management
- Source management
- Data-source configuration
- Audit-log access
- System configuration
- Dataset management

Deployments may implement public, private, research, or institutional access policies without changing the underlying data model.

---

# Optional Plugin Modules

Plugins extend Ledger Watch without expanding the required core.

## SEC EDGAR Plugin

Provides automated ingestion of SEC public filings including:

- Form 4
- Form 3
- Form 5
- 13F
- 8-K
- 10-Q
- 10-K
- Proxy filings
- Beneficial ownership filings

---

## CFTC Plugin

Provides commodity-market disclosure capabilities including applicable:

- Large trader information
- Commitment of Traders data
- Commodity positioning
- Futures-related disclosures

---

## Congressional Disclosure Plugin

Provides publicly disclosed trading information for public officials where legally and publicly available.

---

## International Regulatory Plugin

Adds publicly available regulatory disclosures from jurisdictions outside the United States.

The plugin architecture should support:

- Country-specific sources
- Regulatory agencies
- Filing formats
- Identifier systems
- Local market structures

---

## News Intelligence Plugin

Connects publicly available or properly licensed news sources with Ledger Watch events.

Capabilities may include:

- News ingestion
- Source attribution
- Event extraction
- Entity recognition
- Instrument recognition
- Timestamp normalization
- Duplicate detection
- Event clustering

---

## Market Data Plugin

Provides historical and real-time market data where the deployment has appropriate access rights.

Capabilities may include:

- Historical prices
- Intraday prices
- Volume
- Market capitalization
- Volatility
- Benchmark comparisons
- Market reaction analysis

---

## Options Analytics Plugin

Adds:

- Options transactions
- Open interest
- Implied volatility
- Greeks
- Expiration analysis
- Options positioning

All data must clearly identify whether it is directly reported or derived.

---

## Commodity Analytics Plugin

Adds:

- Futures markets
- Commodity contracts
- Position analysis
- Inventory events
- Supply events
- Demand events
- Commodity-specific timelines

---

## Graph Database Plugin

Provides integration with graph databases for large-scale relationship analysis.

Potential implementations may include:

- Neo4j
- Apache AGE
- Other compatible graph systems

The graph plugin must not make a graph database mandatory for core Ledger Watch operation.

---

## Machine Learning Plugin

Provides optional machine learning capabilities including:

- Pattern detection
- Entity resolution
- Event classification
- Anomaly detection
- Clustering
- Similarity analysis

Machine learning outputs must remain distinguishable from verified source data.

---

## Natural Language Processing Plugin

Provides:

- Named entity recognition
- Financial entity extraction
- Event extraction
- Document classification
- Filing summarization
- News classification
- Relationship extraction

Generated information must be labeled as derived or machine-generated.

---

## Alerting Plugin

Provides configurable notifications for:

- New trades
- New filings
- Corporate actions
- Significant position changes
- Event correlations
- Anomaly thresholds
- Entity activity
- Instrument activity

Alerts should identify the underlying records that triggered them.

---

## Visualization Plugin

Provides graphical interfaces for:

- Entity profiles
- Trade timelines
- Capital flows
- Relationship graphs
- Event timelines
- Market activity
- Statistical anomalies

---

## Research Workbench Plugin

Provides tools for researchers, journalists, analysts, and investigators.

Capabilities may include:

- Saved queries
- Custom datasets
- Comparative analysis
- Timeline construction
- Evidence collections
- Research notes
- Exportable reports
- Reproducible analysis

---

## Data Export Plugin

Supports structured exports including:

- CSV
- JSON
- JSON-LD
- Parquet
- SQL
- Graph formats

Exports should preserve source identifiers and provenance metadata whenever possible.

---

# Entity Profiles

Ledger Watch provides profiles for every supported entity.

Profiles may include:

- Identity information
- Regulatory identifiers
- Company relationships
- Employment relationships
- Historical trades
- Holdings
- Corporate actions
- Associated instruments
- Related filings
- Related events
- Statistical activity
- Historical timelines
- Source references

Profiles must distinguish between verified information and derived relationships.

---

# Company Profiles

Company profiles provide a consolidated view of public company activity.

A profile may contain:

- Corporate identity
- Securities
- Executives
- Directors
- Institutional holders
- Insider activity
- Buybacks
- Issuances
- Dividends
- Earnings
- Regulatory filings
- Major public events
- Market activity
- Related entities

---

# Trader Profiles

Trader profiles provide a historical record of publicly disclosed activity.

Profiles may contain:

- Entity identity
- Reported transactions
- Historical positions
- Instruments traded
- Transaction frequency
- Transaction size
- Sector exposure
- Event relationships
- Historical statistical patterns
- Source documents

Trader profiles must never imply that a pattern demonstrates unlawful behavior.

---

# Institutional Profiles

Institutional profiles may track:

- Institutional identity
- Reported holdings
- Position changes
- Portfolio composition
- Sector exposure
- Instrument exposure
- Historical filings
- Related entities
- Corporate relationships

---

# Event-to-Trade Analysis

Ledger Watch allows users to examine public financial activity around events.

The system may display:

**Event → Disclosures → Trades → Market Movement → Subsequent Activity**

Users should be able to modify:

- Time windows
- Comparison periods
- Entities
- Instruments
- Event categories
- Statistical thresholds

---

# Cross-Entity Analysis

Ledger Watch supports analysis across multiple entities.

Examples include:

- Multiple institutions trading the same instrument
- Multiple insiders trading the same company
- Institutional activity surrounding corporate announcements
- Repeated activity across related companies
- Common instruments across multiple portfolios
- Trading clusters surrounding public events

---

# Statistical Baselines

Analytical modules should establish appropriate historical baselines.

Possible comparison groups include:

- Entity's own historical activity
- Sector peers
- Market averages
- Instrument-specific activity
- Institutional peer groups
- Historical event windows

Baseline selection must be documented so results remain reproducible.

---

# Data Quality Framework

Ledger Watch should assign quality metadata to records.

Possible states include:

- Unverified
- Source Located
- Source Verified
- Independently Confirmed
- Corrected
- Superseded
- Disputed

Data quality must never be hidden from users.

---

# Data Integrity

Ledger Watch implementations should:

- Preserve original source records
- Preserve source identifiers
- Record ingestion timestamps
- Track transformations
- Maintain version history
- Prevent silent modification of historical records
- Provide correction mechanisms
- Maintain audit logs
- Preserve provenance

---

# Privacy and Public Information

Ledger Watch is intended to work with publicly available information.

Implementations should:

- Avoid collecting unnecessary personal information
- Respect applicable privacy laws
- Respect source terms and licensing
- Avoid exposing non-public personal information
- Avoid attempting to identify anonymous individuals through private information
- Clearly distinguish public records from derived analysis

---

# Neutrality and Accountability

Ledger Watch is designed for transparency and accountability, not automated accusations.

The system should describe observable information using neutral terminology such as:

- Reported transaction
- Public disclosure
- Temporal relationship
- Statistical anomaly
- Activity concentration
- Position change
- Event correlation
- Historical pattern

The system should not convert statistical findings into accusations of misconduct.

When an authoritative public source establishes a legal or regulatory finding, Ledger Watch may preserve and reference that finding with its original source.

---

# Reproducible Analysis

Analytical results should be reproducible.

Where applicable, Ledger Watch should expose:

- Input records
- Source records
- Analysis parameters
- Time windows
- Algorithms
- Model versions
- Dataset versions
- Calculation timestamps

Users should be able to understand how an analytical result was produced.

---

# Local-First and Self-Hosted Deployment

Ledger Watch should support self-hosted deployments.

Deployments may operate:

- Locally
- On private infrastructure
- On institutional infrastructure
- In public cloud infrastructure
- In research environments
- As a public service

The architecture should avoid unnecessary dependency on a single commercial provider.

---

# Open API and Interoperability

Ledger Watch should expose standardized interfaces allowing external systems to consume its data.

Potential integrations include:

- Research platforms
- Financial dashboards
- Journalism tools
- Academic applications
- Government transparency systems
- Data visualization platforms
- AI systems
- Other open-source financial applications

---

# AI Integration

AI integrations are optional.

AI systems may assist with:

- Filing classification
- Entity resolution
- Event extraction
- Document analysis
- Natural-language search
- Pattern discovery
- Research assistance
- Query generation

AI-generated conclusions must never replace source records.

Every AI-generated result should provide access to the underlying evidence whenever possible.

---

# Security

Ledger Watch implementations should include:

- Secure authentication
- Authorization controls
- API authentication
- Rate limiting
- Input validation
- Audit logging
- Secure secrets management
- Dependency monitoring
- Data integrity verification
- Administrative access controls

Security-sensitive functionality should be modularized where practical.

---

# Plugin Requirements

Optional plugins should:

- Use documented interfaces
- Declare dependencies
- Identify external data sources
- Preserve source provenance
- Clearly distinguish derived information
- Avoid modifying core records without an auditable process
- Support versioning
- Document licensing requirements
- Respect source licensing and usage restrictions

Plugins should not require proprietary services unless clearly identified as optional dependencies.

---

# Recommended Technology Architecture

A deployment may use:

- PostgreSQL for primary relational storage
- TimescaleDB for time-series workloads
- OpenSearch for search and document indexing
- Graph databases through an optional plugin
- Python for data ingestion and analytics
- Rust, Go, or other languages for performance-sensitive services
- REST or GraphQL for APIs
- JSON and JSON-LD for structured interchange

The specification does not mandate a particular implementation language or database.

---

# Implementation Principles

Ledger Watch implementations should follow these principles:

### Source Before Analysis

The original public record is more important than the analytical result.

### Evidence Before Interpretation

Users should be able to inspect the evidence behind a conclusion.

### Facts Before Scores

Scoring systems must never obscure the underlying data.

### Provenance Everywhere

Material information should remain traceable to its source.

### Neutrality

The system should document observable behavior without automatically assigning intent.

### Reproducibility

Analytical results should be independently reproducible.

### Modularity

Core functionality should remain independent from optional data sources and analytical systems.

### Interoperability

Ledger Watch should work with other open-source systems and standardized data formats.

### Vendor Independence

No single commercial data provider should be required for the core specification.

---

# Future Expansion

The modular architecture allows Ledger Watch to expand into:

- International securities markets
- Additional commodities
- Derivatives
- Digital assets
- Fixed income
- Foreign exchange
- Municipal securities
- Government financial disclosures
- Corporate ownership networks
- Supply-chain events
- Patent and intellectual-property events
- Regulatory enforcement datasets
- Political and economic event datasets
- Global financial transparency networks

New capabilities should be implemented as modules or plugins whenever practical.

---

# Contributing

Contributions are welcome.

Areas where contributions are particularly valuable include:

- New public data connectors
- Source verification
- Entity resolution
- Filing normalization
- Corporate action tracking
- Event classification
- Statistical analysis
- Data quality improvements
- API development
- Visualization
- Documentation
- Testing
- Security
- Plugin development

All contributions must preserve Ledger Watch's principles of public-source verification, neutrality, provenance, reproducibility, and transparency.

See `CONTRIBUTING.md` for contribution requirements.

---

# Disclaimer

Ledger Watch provides tools for organizing and analyzing publicly available information.

The presence of a transaction, event correlation, statistical anomaly, or behavioral pattern does not establish intent, causation, illegality, misconduct, or wrongdoing.

Ledger Watch does not provide investment, legal, accounting, or regulatory advice.

Users are responsible for independently evaluating information and consulting authoritative sources when making decisions.

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
  - [https://roxanneardary.com/ledgerwatch/](https://roxanneardary.com/ledgerwatch/)

---

## License & Notice Requirements

Ledger Watch is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Ledger Watch specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
