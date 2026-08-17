# SafeMeds Index Specification
**Powering insight across the world of medicine.**
- HTML Mirror:  [https://roxanneardary.com/safemeds-index-specification/](https://roxanneardary.com/safemeds-index-specification/)  

---

## Overview

SafeMeds Index is an open-source global pharmaceutical intelligence platform designed to provide transparent, searchable, and continuously updated information about medicines, pharmaceutical pricing, manufacturing, distribution, recalls, safety developments, and therapeutic alternatives.

SafeMeds Index is designed to help individuals, researchers, healthcare professionals, journalists, policymakers, and organizations understand the global pharmaceutical market and identify meaningful differences in medication availability, pricing, provenance, safety, and therapeutic options.

### Mission

The mission of SafeMeds Index is to make pharmaceutical information more transparent and accessible by connecting fragmented global data into a unified intelligence system.

---

## Design Principles

### Open Source

The platform shall be developed and distributed as open-source software under the GNU Affero General Public License v3.0 or later (AGPL-3.0+), including the applicable Section 7 attribution requirement.

### Global Coverage

The system shall support pharmaceutical data from countries and jurisdictions worldwide while accounting for differences in naming conventions, currencies, regulatory systems, availability, pricing structures, and data formats.

### Modular Architecture

The platform shall use modular components with clearly defined interfaces. Core capabilities shall remain independent from optional integrations and extensions.

### Local First

The system should support local processing, local data storage, self-hosted deployments, and operation without mandatory dependence on a single commercial cloud provider.

### Vendor Neutrality

The platform shall avoid unnecessary vendor lock-in and support interchangeable databases, AI models, search engines, storage systems, data providers, and deployment environments.

### Evidence and Provenance

Information shall retain source provenance whenever possible. The system shall distinguish verified information from inferred, estimated, incomplete, outdated, or conflicting information.

### Human Oversight

AI-generated classifications, summaries, recommendations, and risk assessments shall remain reviewable and traceable to their underlying sources.

### Safety

SafeMeds Index shall present pharmaceutical information as informational intelligence rather than a substitute for professional medical diagnosis, prescribing, or treatment decisions.

---

## Core Modules

### Pharmaceutical Identity Module

The Pharmaceutical Identity Module shall create standardized identities for medications and pharmaceutical products across international markets.

Features shall include:

- Generic and active ingredient names
- Brand names
- International and regional names
- Active pharmaceutical ingredients
- Strength and concentration
- Dosage form
- Route of administration
- Package size
- Product identifiers
- Regulatory identifiers
- Anatomical Therapeutic Chemical classifications
- Synonyms and spelling variations
- Country-specific product names
- Ingredient normalization
- Combination medication identification
- Product status tracking

The module shall establish canonical medication identities that other SafeMeds Index modules can reference.

### Global Price Intelligence Module

The Global Price Intelligence Module shall collect, normalize, compare, and analyze pharmaceutical prices across countries and markets.

Features shall include:

- Country-specific medication prices
- Pharmacy pricing
- Distributor pricing
- Manufacturer pricing where publicly available
- Retail and wholesale pricing where available
- Insurance and reimbursement information where available
- Package-size normalization
- Dosage normalization
- Currency conversion
- Purchasing-power comparisons
- Historical price tracking
- Price change detection
- Geographic price comparisons
- Price anomaly detection
- Availability and price correlation
- Lowest identified price indicators
- Data freshness indicators

The system shall distinguish between listed prices, observed prices, estimated prices, negotiated prices, reimbursed prices, and other pricing categories.

### Manufacturer Intelligence Module

The Manufacturer Intelligence Module shall maintain structured information about companies and organizations responsible for pharmaceutical production.

Features shall include:

- Manufacturer identity
- Parent company relationships
- Subsidiaries
- Production facilities
- Manufacturing countries
- Manufacturing locations
- Active pharmaceutical ingredient manufacturers
- Finished-product manufacturers
- Contract manufacturers
- Packaging facilities
- Regulatory registrations
- Product relationships
- Manufacturing history
- Regulatory actions
- Recall history
- Source provenance

The module shall distinguish between the brand owner, marketing authorization holder, manufacturer, contract manufacturer, API manufacturer, packaging facility, and distributor where the available data supports those distinctions.

### Distribution Intelligence Module

The Distribution Intelligence Module shall map pharmaceutical movement through available distribution networks.

Features shall include:

- Distributors
- Wholesalers
- Importers
- Exporters
- Pharmacies
- Healthcare providers where appropriate
- Distribution territories
- Import and export relationships
- Product distribution relationships
- Country-specific availability
- Supply chain relationships
- Distribution changes
- Source documentation

The system shall represent known relationships without presenting inferred supply chains as verified facts.

### Batch and Lot Intelligence Module

The Batch and Lot Intelligence Module shall provide traceability for pharmaceutical batches and lots.

Features shall include:

- Batch numbers
- Lot numbers
- Expiration dates
- Manufacturing dates where available
- Production facilities
- Product identifiers
- Packaging information
- Recall relationships
- Safety alert relationships
- Distribution relationships
- Geographic distribution
- Batch status
- Source records

The module shall allow users to determine whether a specific batch or lot has been associated with a recall, warning, contamination event, manufacturing defect, or other regulatory action.

### Recall and Regulatory Safety Module

The Recall and Regulatory Safety Module shall aggregate pharmaceutical recalls, safety alerts, regulatory actions, warnings, withdrawals, restrictions, and related notices from jurisdictions around the world.

Features shall include:

- Recall identification
- Recall dates
- Affected products
- Affected batches
- Affected manufacturers
- Recall classifications
- Recall reasons
- Geographic scope
- Regulatory authority
- Regulatory notices
- Product withdrawals
- Safety warnings
- Manufacturing violations
- Import alerts
- Distribution restrictions
- Historical recall records

The module shall preserve the originating regulatory source whenever possible.

### Global News Intelligence Module

The Global News Intelligence Module shall monitor worldwide news and publicly available reporting concerning medications, manufacturers, pharmaceutical products, and relevant safety issues.

Features shall include:

- Global news ingestion
- Medication entity recognition
- Manufacturer entity recognition
- Safety event detection
- Recall event detection
- Litigation monitoring
- Regulatory reporting
- Research reporting
- Manufacturing incidents
- Contamination reporting
- Shortage reporting
- Pricing reporting
- Supply chain reporting
- Adverse event reporting
- International language processing
- Duplicate story detection
- Source credibility metadata
- Publication date tracking
- Event timeline construction

The system shall preserve links and source information for material claims.

### Scientific and Clinical Evidence Module

The Scientific and Clinical Evidence Module shall collect and organize scientific literature and clinical evidence associated with medications and therapeutic alternatives.

Features shall include:

- Clinical trials
- Systematic reviews
- Meta-analyses
- Peer-reviewed research
- Regulatory evidence
- Pharmacological studies
- Comparative effectiveness studies
- Safety studies
- Drug interaction studies
- Outcome data
- Evidence quality indicators
- Publication dates
- Research provenance

The module shall distinguish between established evidence, emerging evidence, conflicting evidence, and insufficient evidence.

### Generic Equivalence Module

The Generic Equivalence Module shall identify generic products associated with the same active ingredient, strength, dosage form, and applicable regulatory equivalence criteria.

Features shall include:

- Generic product identification
- Active ingredient matching
- Strength matching
- Dosage-form matching
- Regulatory equivalence information
- Bioequivalence information where available
- Brand-to-generic relationships
- Country-specific generic availability
- Manufacturer comparisons
- Price comparisons
- Evidence links

The system shall not automatically represent a product as interchangeable when regulatory or clinical evidence does not support that conclusion.

### Therapeutic Alternatives Module

The Therapeutic Alternatives Module shall identify medications that may be used for the same or related therapeutic purposes while clearly distinguishing therapeutic alternatives from pharmaceutical equivalents.

Features shall include:

- Therapeutic class comparisons
- Active ingredient comparisons
- Indication matching
- Clinical evidence comparisons
- Effectiveness evidence
- Safety evidence
- Contraindication information
- Interaction information
- Country-specific availability
- Price comparisons
- Evidence quality
- Clinical uncertainty indicators

The module shall avoid presenting therapeutic alternatives as universally interchangeable.

### Medication Safety Intelligence Module

The Medication Safety Intelligence Module shall combine information from recalls, regulatory actions, scientific literature, news, and other validated sources to create medication safety intelligence.

Features shall include:

- Safety event aggregation
- Risk categorization
- Event timelines
- Manufacturer risk history
- Product risk history
- Batch risk history
- Geographic risk mapping
- Source confidence
- Evidence strength
- Conflicting evidence detection
- Safety trend detection

Safety assessments shall remain transparent and traceable to their underlying evidence.

### Drug Shortage and Availability Module

The Drug Shortage and Availability Module shall track medication availability across countries and markets.

Features shall include:

- Drug shortages
- Supply interruptions
- Manufacturing disruptions
- Distribution interruptions
- Geographic availability
- Shortage duration
- Shortage severity
- Alternative availability
- Historical shortages
- Manufacturer availability
- Regulatory shortage notices

### Currency and Market Normalization Module

The Currency and Market Normalization Module shall make international pharmaceutical pricing comparable.

Features shall include:

- Currency conversion
- Historical exchange rates
- Purchasing-power comparisons
- Unit-price normalization
- Package-size normalization
- Dosage normalization
- Regional market classification
- Price-date tracking
- Exchange-rate provenance

The system shall preserve the original price and currency alongside normalized values.

### Search and Discovery Module

The Search and Discovery Module shall provide a unified interface for locating pharmaceutical intelligence.

Features shall include:

- Medication search
- Brand search
- Generic search
- Manufacturer search
- Distributor search
- Batch search
- Recall search
- Country search
- Price search
- Safety search
- News search
- Alternative search
- Full-text search
- Multilingual search
- Synonym matching
- Fuzzy matching
- Advanced filtering

### Data Provenance Module

The Data Provenance Module shall track where information originated and how it was transformed.

Features shall include:

- Source identification
- Source URLs
- Publication dates
- Retrieval dates
- Data provider identification
- Transformation history
- Import history
- Confidence indicators
- Verification status
- Data freshness
- Conflict identification
- Version history

Every significant data point should be traceable to its source whenever technically and legally possible.

### Data Quality Module

The Data Quality Module shall evaluate incoming and existing pharmaceutical data.

Features shall include:

- Validation rules
- Duplicate detection
- Contradiction detection
- Missing-field detection
- Stale-data detection
- Invalid-identifier detection
- Currency validation
- Unit validation
- Source validation
- Confidence scoring
- Human review queues

### AI Intelligence Module

The AI Intelligence Module shall provide machine-assisted analysis across the SafeMeds Index data ecosystem.

Features shall include:

- Named entity recognition
- Pharmaceutical entity matching
- Multilingual classification
- Document classification
- News event extraction
- Recall detection
- Safety event extraction
- Price anomaly detection
- Relationship extraction
- Summarization
- Translation
- Semantic search
- Evidence clustering
- Alternative discovery
- Duplicate detection
- Conflict detection

AI-generated results shall include provenance and confidence information whenever possible.

### Alert and Notification Module

The Alert and Notification Module shall allow users to monitor medications, manufacturers, batches, prices, recalls, and safety developments.

Features shall include:

- Price alerts
- Recall alerts
- Batch alerts
- Safety alerts
- Manufacturer alerts
- Shortage alerts
- News alerts
- Regulatory alerts
- Availability alerts
- Watchlists
- Email notifications
- Push notifications
- Web notifications
- Configurable thresholds

### User Intelligence Module

The User Intelligence Module shall provide personalized monitoring without requiring unnecessary personal information.

Features shall include:

- Saved medications
- Saved manufacturers
- Saved countries
- Saved pharmacies
- Saved searches
- Watchlists
- Price targets
- Safety monitoring
- Notification preferences
- Data export
- Account deletion

### API Module

The API Module shall provide programmatic access to SafeMeds Index data and intelligence.

Features shall include:

- Medication endpoints
- Pricing endpoints
- Manufacturer endpoints
- Distribution endpoints
- Batch endpoints
- Recall endpoints
- Safety endpoints
- News endpoints
- Evidence endpoints
- Alternative endpoints
- Search endpoints
- Provenance endpoints
- Authentication
- Authorization
- Rate limiting
- API versioning
- Documentation

### Internationalization Module

The Internationalization Module shall support global deployment.

Features shall include:

- Multilingual interfaces
- Multilingual search
- Pharmaceutical name localization
- Local currency support
- Country-specific regulatory terminology
- Regional date formats
- Regional measurement conventions
- Translation workflows
- Language-aware NLP

### Governance and Audit Module

The Governance and Audit Module shall maintain transparency around system operations.

Features shall include:

- Audit logs
- Data change history
- Model version tracking
- Administrative actions
- Source changes
- Moderation history
- Verification history
- User reports
- Correction requests
- Governance records

## Optional Plugin Modules

### Pharmacy Integration Plugin

Connects SafeMeds Index to participating pharmacies and pharmacy data providers for current pricing and availability information.

### Government Data Plugin

Connects to national and regional government pharmaceutical databases, regulatory systems, pricing databases, and public health datasets.

### Regulatory Authority Plugin

Provides jurisdiction-specific integrations for regulatory agencies and safety authorities.

### News Provider Plugin

Adds additional news feeds and licensed news sources to the Global News Intelligence Module.

### Scientific Literature Plugin

Connects additional scientific literature databases and research repositories.

### Trade and Customs Plugin

Adds international pharmaceutical import and export information where legally available.

### Supply Chain Plugin

Provides additional pharmaceutical manufacturing and distribution intelligence.

### Barcode and Product Identifier Plugin

Supports scanning and interpretation of pharmaceutical barcodes, package identifiers, serialization information, and related product identifiers where available.

### OCR Plugin

Extracts structured pharmaceutical information from product packaging, labels, regulatory documents, invoices, and other permitted documents.

### Translation Plugin

Adds external or locally hosted translation models for pharmaceutical terminology and international sources.

### AI Model Plugin

Allows operators to add, remove, or replace AI models without changing the core application.

Supported model categories may include:

- Large language models
- Small language models
- Medical language models
- Multilingual language models
- Named entity recognition models
- Embedding models
- Classification models
- Ranking models
- Recommendation models
- Translation models
- Vision-language models

### Local AI Plugin

Allows SafeMeds Index to run supported AI models locally or on private infrastructure without requiring external AI services.

### Mapping Plugin

Adds geographic visualization of pharmaceutical prices, manufacturers, production facilities, distributors, recalls, shortages, and availability.

### Visualization Plugin

Provides advanced charts, graphs, timelines, geographic views, price comparisons, and pharmaceutical relationship visualizations.

### Notification Provider Plugin

Adds external notification systems such as email providers, messaging systems, mobile push services, or self-hosted notification infrastructure.

### Identity Provider Plugin

Supports optional authentication systems while allowing self-hosted deployments to select their preferred identity provider.

### Data Export Plugin

Provides export formats for researchers, journalists, healthcare organizations, governments, and other authorized users.

Supported formats may include:

- CSV
- JSON
- XML
- RDF
- Parquet
- API feeds

### Research Plugin

Provides tools for researchers to compare pharmaceutical prices, safety events, manufacturers, clinical evidence, and therapeutic alternatives.

### Public Health Plugin

Provides specialized analytics for public health organizations, including shortage monitoring, availability analysis, and geographic medication access.

### Accessibility Plugin

Provides additional accessibility capabilities for users with visual, auditory, cognitive, or motor accessibility requirements.

## Model Architecture

SafeMeds Index shall support a model-agnostic AI architecture so that models can be evaluated and replaced independently of the core application.

### Language Models

Language models may be used for:

- Document understanding
- Summarization
- Question answering
- Structured extraction
- Research synthesis
- Classification
- Pharmaceutical intelligence analysis

The system shall support both locally hosted and externally hosted models where compatible with the deployment requirements.

### Medical Language Models

Medical and biomedical language models may be used for:

- Medical terminology extraction
- Drug and disease entity recognition
- Clinical document analysis
- Biomedical literature analysis
- Pharmacological relationship extraction

### Embedding Models

Embedding models shall support:

- Semantic search
- Pharmaceutical entity matching
- Multilingual matching
- Duplicate detection
- Similarity analysis
- Evidence clustering

### Named Entity Recognition Models

NER models shall identify:

- Medications
- Active ingredients
- Manufacturers
- Distributors
- Regulatory organizations
- Countries
- Healthcare organizations
- Medical conditions
- Clinical events
- Safety events
- Batch numbers
- Product identifiers

### Classification Models

Classification models may identify:

- Recall events
- Safety events
- Pricing information
- Clinical evidence
- Regulatory actions
- Manufacturing incidents
- Shortages
- News categories
- Source categories
- Evidence quality

### Recommendation Models

Recommendation models may assist with:

- Generic discovery
- Therapeutic alternative discovery
- Evidence retrieval
- Price comparison
- Search ranking

Recommendations must remain evidence-linked and must not imply clinical interchangeability without appropriate supporting evidence.

### Anomaly Detection Models

Anomaly detection models may identify:

- Unusual price changes
- Unusual regional price differences
- Suspicious data patterns
- Unexpected availability changes
- Data quality anomalies
- Supply chain anomalies

### Knowledge Graph Models

Knowledge graph technologies may represent relationships among:

- Medications
- Ingredients
- Manufacturers
- Production facilities
- Distributors
- Pharmacies
- Countries
- Batches
- Recalls
- Safety events
- Clinical evidence
- Therapeutic alternatives

### Computer Vision Models

Computer vision models may optionally process permitted images of:

- Medication packaging
- Labels
- Product identifiers
- Regulatory documents
- Recall notices

Visual extraction must remain subject to validation and human review when accuracy is uncertain.

## Data Sources

SafeMeds Index shall prioritize authoritative and legally accessible sources.

Potential sources include:

- Government pharmaceutical databases
- National regulatory agencies
- International regulatory organizations
- Public pharmacy pricing databases
- Manufacturer publications
- Distributor data
- Public procurement databases
- Scientific publications
- Clinical trial registries
- Public recall databases
- Public safety notices
- Licensed news sources
- Publicly accessible pharmaceutical datasets

The platform shall respect applicable terms of use, licensing requirements, copyright restrictions, privacy requirements, robots directives, and data access restrictions.

## Data Integrity

SafeMeds Index shall distinguish among:

- Verified data
- Official data
- Reported data
- Observed data
- Estimated data
- AI-inferred data
- Community-submitted data
- Historical data
- Conflicting data
- Unverified data

The platform shall never present AI inference as verified pharmaceutical fact.

## Security

The platform shall implement appropriate security controls including:

- Secure authentication
- Authorization controls
- Encryption in transit
- Encryption at rest where appropriate
- Secure secrets management
- Dependency monitoring
- Input validation
- API protection
- Audit logging
- Rate limiting
- Security testing
- Vulnerability reporting

## Privacy

SafeMeds Index shall minimize collection of personally identifiable information.

The platform shall avoid collecting sensitive health information unless explicitly required for a specific deployment and appropriately protected.

Personalized medication monitoring should preferably operate using minimal user information and privacy-preserving identifiers.

## Healthcare Safety Disclaimer

SafeMeds Index is an information and pharmaceutical intelligence platform.

Information presented by the platform shall not be represented as a diagnosis, prescription, individualized medical recommendation, or replacement for consultation with a qualified healthcare professional.

Generic products and therapeutic alternatives shall be clearly distinguished. The presence of an alternative in the database shall not mean that it is appropriate for every patient.

## Deployment

SafeMeds Index shall support:

- Local deployment
- Self-hosted deployment
- Private infrastructure
- Institutional deployment
- Public web deployment
- Containerized deployment
- Distributed deployment

The architecture shall avoid requiring a single hosting provider or proprietary service.

## Interoperability

The platform should support widely used standards and interoperable data formats where applicable.

Integration capabilities should support:

- REST APIs
- GraphQL where useful
- JSON
- CSV
- XML
- RDF
- Structured pharmaceutical identifiers
- Standardized medical terminology
- International currency standards
- Geographic standards

## Transparency

Every major intelligence result should provide enough context for users to understand:

- What was found
- When it was found
- Where it came from
- How it was processed
- Whether it was verified
- How confident the system is
- Whether conflicting information exists

## Corrections

Users and authorized data contributors should be able to report:

- Incorrect prices
- Incorrect manufacturer relationships
- Incorrect batch information
- Incorrect recalls
- Incorrect safety information
- Incorrect alternatives
- Outdated information
- Duplicate records
- Misclassified information

Corrections should enter a review and audit process rather than silently overwriting historical records.  

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
  - [https://roxanneardary.com/safemedsindex/](https://roxanneardary.com/safemedsindex/)

---

## License & Notice Requirements

SafeMeds Index is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- SafeMeds Index specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
