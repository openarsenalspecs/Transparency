# OpenBid Ledger
**Infrastructure for Transparent, Auditable Advertising.**
- HTML Mirror:  [https://roxanneardary.com/openbid-ledger-specification/](https://roxanneardary.com/openbid-ledger-specification/)  

---

OpenBid Ledger is an open source specification for transparent, auditable digital advertising auctions. It defines a modular system in which business bidding is visible within the applicable auction environment and auction activity is recorded in an immutable, verifiable ledger.

The specification is designed to eliminate hidden bidding, undisclosed host intervention, bid manipulation, selective bid suppression, and alteration of historical auction records. Every applicable bid, auction event, administrative action, pricing calculation, advertising delivery event, and settlement event must be recorded according to the specification's immutable logging requirements.

OpenBid Ledger supports separate **Cost Per Click (CPC)** and **Cost Per Impression Unit (CPIU)** advertising models. CPC functionality manages auctions and billing based on validated clicks. CPIU functionality manages auctions and billing based on validated impressions using an Impression Unit defined by the hosting service. The hosting service must disclose the applicable Impression Unit before bidding begins, and the definition becomes part of the permanent auction record.

## Specification Objectives

OpenBid Ledger is designed to provide:

- Transparent digital advertising auctions
- Visible business bidding
- Immutable auction records
- Verifiable auction outcomes
- Host accountability
- Independent auditing
- Deterministic auction execution
- Published and versioned auction rules
- Separate CPC and CPIU functionality
- Transparent billing and settlement
- Tamper-evident historical records
- Modular implementation
- Vendor-neutral interoperability
- Independent hosting and verification

---

## Core Requirements

### Visible Bidding

All qualifying bids must be visible within the applicable auction environment.

The system must not provide hidden bids, private host bids, undisclosed bids, preferential bidding channels, selective bid visibility, or other mechanisms that prevent applicable participants from observing qualifying bids.

Each bid must include sufficient information to establish when the bid was submitted, who submitted it according to the system's identity requirements, the amount bid, the applicable advertising model, the auction to which it belongs, and its current status.

A bid cannot be silently changed. Any withdrawal, rejection, expiration, correction, or other change in state must be recorded as a new immutable event.

### Immutable Auction Records

All auction events must be recorded in an append-only ledger.

Historical records must not be deleted, altered, backdated, reordered, or silently replaced. Corrections must create additional records that preserve the original event and identify the subsequent correction.

The ledger must provide mechanisms for detecting unauthorized modification and independently verifying the sequence and integrity of auction events.

### Host Accountability

The hosting service provides the infrastructure for operating auctions but must not have an undisclosed mechanism capable of manipulating the auction or its historical records.

The host must not secretly alter:

- Bids
- Bid timestamps
- Bid rankings
- Auction results
- Clearing prices
- Auction rules
- Impression records
- Click records
- Billing calculations
- Settlement records
- Historical auction events

Administrative actions capable of affecting an auction must themselves be recorded and auditable.

### Published Auction Rules

The rules governing an auction must be available to applicable participants before bidding begins.

The rules must identify the applicable auction model, bid requirements, eligibility requirements, ranking method, winner determination method, pricing method, applicable fees, Impression Unit where applicable, and other material conditions.

An active auction must remain governed by the ruleset associated with that auction. Changes to future auctions must not retroactively modify completed or active auction records.

---

## Core Modules

### Auction Core Module

The Auction Core Module manages the lifecycle and execution of advertising auctions.

Features include:

- Auction creation
- Auction identification
- Auction scheduling
- Auction start and end events
- Bid acceptance
- Bid validation
- Bid ranking
- Winner determination
- Clearing-price calculation
- Auction status
- Auction rules association
- Auction result generation
- Auction event recording
- Deterministic auction execution

### Bid Ledger Module

The Bid Ledger Module maintains the immutable record of bidding activity.

Features include:

- Unique bid identification
- Bid timestamps
- Bid sequence numbers
- Bid amounts
- Bidder identification
- Bid status
- Bid acceptance records
- Bid rejection records
- Bid withdrawal records
- Bid expiration records
- Winning bid records
- Losing bid records
- Append-only event storage
- Cryptographic event linking
- Tamper detection
- Historical record preservation
- Ledger integrity verification

### CPC Module

The Cost Per Click Module provides advertising auctions based on validated clicks.

Features include:

- CPC bid submission
- CPC bid visibility
- CPC bid ranking
- CPC auction execution
- Click registration
- Click validation
- Click attribution
- Invalid-click detection
- Duplicate-click detection
- CPC clearing-price calculation
- CPC billing
- CPC settlement
- Immutable click records
- Immutable CPC billing records
- Click dispute records

### CPIU Module

The Cost Per Impression Unit Module provides advertising auctions based on validated advertising impressions.

Features include:

- CPIU bid submission
- CPIU bid visibility
- CPIU auction execution
- Impression registration
- Impression validation
- Impression attribution
- Duplicate-impression detection
- Invalid-impression detection
- Impression Unit configuration
- CPIU clearing-price calculation
- CPIU billing
- CPIU settlement
- Immutable impression records
- Immutable CPIU billing records
- Impression dispute records

The hosting service determines the number of impressions represented by an Impression Unit. The applicable quantity must be publicly disclosed before bidding begins and must be permanently associated with the applicable auction. The hosting service must not change the Impression Unit during or after an auction.

### Advertising Inventory Module

The Advertising Inventory Module manages advertising placements available for auction.

Features include:

- Publisher registration
- Inventory registration
- Placement identification
- Inventory classification
- Inventory availability
- Placement specifications
- Inventory status
- Minimum bid configuration
- Auction eligibility
- Inventory ownership records
- Inventory change history

### Advertiser Module

The Advertiser Module manages businesses participating in advertising auctions.

Features include:

- Advertiser registration
- Business identification
- Campaign management
- Budget management
- Bid management
- Campaign scheduling
- Advertising placement selection
- Campaign limits
- Bid limits
- Campaign status
- Advertiser activity records

### Publisher Module

The Publisher Module manages organizations providing advertising inventory.

Features include:

- Publisher registration
- Publisher identification
- Inventory management
- Placement management
- Auction configuration
- Impression Unit configuration
- Floor-price configuration
- Publisher settlement records
- Publisher audit access
- Publisher activity records

### Verification Module

The Verification Module allows participants and independent parties to verify auction integrity.

Features include:

- Auction verification
- Bid verification
- Event verification
- Ledger verification
- Timestamp verification
- Cryptographic record verification
- Auction result verification
- Pricing verification
- Settlement verification
- Verification certificates
- Independent verification
- Historical reconstruction

### Audit Module

The Audit Module provides access to the records necessary to independently examine auction activity.

Features include:

- Auction-level auditing
- Bid-level auditing
- Advertiser auditing
- Publisher auditing
- Billing auditing
- Settlement auditing
- Administrative auditing
- Configuration auditing
- Ruleset auditing
- Fraud-event auditing
- Dispute auditing
- Audit-log export
- Machine-readable records
- Human-readable audit reports

### Billing Module

The Billing Module records and calculates charges resulting from advertising delivery.

Features include:

- CPC billing
- CPIU billing
- Clearing-price records
- Click-based billing
- Impression-based billing
- Host fee records
- Transaction fee records
- Refund records
- Adjustment records
- Billing reconciliation
- Billing verification
- Immutable billing events

### Settlement Module

The Settlement Module manages financial settlement between applicable parties.

Features include:

- Advertiser settlement records
- Publisher settlement records
- Host fee records
- Settlement calculations
- Settlement reconciliation
- Refunds
- Adjustments
- Settlement disputes
- Immutable settlement events
- Independent settlement verification

### Fraud Detection Module

The Fraud Detection Module identifies suspicious advertising activity without modifying historical records.

Features include:

- Invalid-click detection
- Automated-click detection
- Duplicate-click detection
- Impression fraud detection
- Duplicate-impression detection
- Bot activity detection
- Bid manipulation detection
- Bid flooding detection
- Coordinated bidding detection
- Auction interference detection
- Suspicious activity records
- Fraud findings
- Immutable fraud events

Fraud detection must not be used as a mechanism for silently deleting or altering historical auction events. Any determination affecting an existing record must be recorded as a subsequent event.

### Dispute Module

The Dispute Module manages disputes involving auctions, bids, advertising delivery, billing, and settlement.

Features include:

- Bid disputes
- Auction disputes
- Click disputes
- Impression disputes
- Billing disputes
- Settlement disputes
- Evidence records
- Evidence timestamps
- Dispute status
- Resolution records
- Immutable dispute history
- Administrative decision records

### Governance Module

The Governance Module manages changes to the specification, auction rules, configuration, and system policies.

Features include:

- Published governance rules
- Ruleset versioning
- Configuration versioning
- Change proposals
- Change records
- Approval records
- Activation dates
- Immutable governance history
- Historical rules preservation
- Non-retroactive rule changes

### Administration Module

The Administration Module provides operational controls while restricting administrative authority over immutable auction records.

Features include:

- Role-based administration
- Permission management
- Administrative identity
- Privileged-action logging
- Configuration management
- System maintenance records
- Permission-change records
- Administrative audit trails
- Immutable administrative events
- Separation of administrative duties

No administrative function may provide an undisclosed mechanism for rewriting historical auction records.

---

## Optional Plugin Modules

OpenBid Ledger supports optional plugin modules that extend functionality without changing the requirements of the Core Modules.

### Identity Plugin

Provides optional identity verification, business verification, organizational credentials, and participant authentication.

### Targeting Plugin

Provides optional advertising targeting functionality, including geographic, contextual, placement, scheduling, and audience targeting.

### Analytics Plugin

Provides optional reporting, performance analysis, campaign analytics, auction analytics, and historical trend analysis.

### Fraud Intelligence Plugin

Provides advanced fraud analysis, behavioral analysis, anomaly detection, and external fraud intelligence while preserving immutable historical records.

### Payment Plugin

Provides integration with external payment and financial settlement systems.

### Tax Plugin

Provides configurable tax calculation and tax reporting functionality where required.

### Notification Plugin

Provides auction, campaign, billing, settlement, dispute, and administrative notifications.

### Reporting Plugin

Provides customizable advertiser, publisher, host, auditor, and public transparency reports.

### Federation Plugin

Allows compatible independent OpenBid Ledger hosts to exchange advertising inventory, auction participation, verification information, and other permitted records.

### Public Transparency Plugin

Provides public-facing auction information, transparency dashboards, historical auction records, published rules, verification information, and other records designated for public access.

### External Audit Plugin

Provides controlled access for independent auditors and verification organizations without granting authority to modify the underlying ledger.

## Optional Auction Plugin Modules

OpenBid Ledger supports optional auction plugins that adapt the core auction, bid ledger, verification, audit, billing, settlement, and governance capabilities to additional auction markets.

Each plugin must operate within the core transparency, immutability, auditability, and host-accountability requirements of OpenBid Ledger. Plugins may introduce market-specific rules and data fields but must not weaken or bypass immutable auction records or create undisclosed host control over auction outcomes.

### Art Auction Plugin

Supports auctions for paintings, sculptures, photography, digital art, collectibles, and other artistic works.

Features include:

- Artwork registration
- Artist identification
- Ownership records
- Provenance records
- Artwork descriptions
- Condition records
- Authentication records
- Reserve prices
- Bid management
- Auction catalogs
- Winning bid records
- Buyer records
- Seller records
- Commission calculations
- Settlement records
- Provenance history
- Immutable auction records

### Collectibles Auction Plugin

Supports auctions for collectible physical and digital items.

Features include:

- Item registration
- Category classification
- Item condition
- Authentication
- Ownership history
- Rarity information
- Reserve prices
- Bid management
- Auction results
- Buyer and seller records
- Fees
- Settlement
- Provenance tracking

### Real Estate Auction Plugin

Supports auctions for real property and related property interests.

Features include:

- Property registration
- Property identification
- Seller identification
- Property documentation
- Auction terms
- Bid registration
- Deposit requirements
- Reserve prices
- Bid eligibility
- Winning bid records
- Buyer records
- Seller records
- Closing conditions
- Settlement records
- Transaction history
- Immutable auction records

### Vehicle Auction Plugin

Supports auctions for automobiles, trucks, motorcycles, recreational vehicles, boats, and other vehicles.

Features include:

- Vehicle identification
- Vehicle history
- Ownership records
- Condition reports
- Inspection records
- Mileage records
- Authentication
- Reserve prices
- Bid management
- Auction results
- Buyer records
- Seller records
- Fees
- Settlement records

### Equipment Auction Plugin

Supports auctions for industrial, agricultural, construction, commercial, and specialized equipment.

Features include:

- Equipment registration
- Manufacturer information
- Model information
- Serial number records
- Condition reports
- Inspection records
- Maintenance history
- Ownership records
- Reserve prices
- Bid management
- Auction results
- Buyer and seller records
- Settlement records

### Domain Name Auction Plugin

Supports auctions for internet domain names and other transferable digital naming assets.

Features include:

- Domain registration
- Ownership verification
- Domain history
- Expiration information
- Transfer eligibility
- Reserve prices
- Bid management
- Auction results
- Transfer records
- Buyer and seller records
- Settlement records
- Immutable ownership events

### Intellectual Property Auction Plugin

Supports auctions involving transferable intellectual property rights where legally permissible.

Features include:

- Asset registration
- Rights identification
- Ownership records
- Licensing status
- Geographic scope
- Duration
- Restrictions
- Encumbrances
- Bid management
- Reserve prices
- Auction results
- Transfer records
- Settlement records
- Immutable rights history

### Ticket Auction Plugin

Supports auctions for tickets, admissions, reservations, and transferable access rights.

Features include:

- Event identification
- Ticket identification
- Seat or access information
- Original issuer
- Transfer restrictions
- Bid management
- Auction rules
- Winning bid
- Transfer records
- Fees
- Settlement records
- Transfer history

### Memorabilia Auction Plugin

Supports auctions for historical, cultural, entertainment, and sports memorabilia.

Features include:

- Item registration
- Provenance
- Authentication
- Condition records
- Ownership history
- Documentation
- Reserve prices
- Bid management
- Auction results
- Buyer and seller records
- Settlement records

### Agricultural Auction Plugin

Supports auctions for livestock, crops, agricultural equipment, land-use assets, and other agricultural commodities where applicable.

Features include:

- Asset registration
- Producer identification
- Quantity records
- Quality records
- Inspection records
- Location records
- Auction terms
- Bid management
- Reserve prices
- Winning bid records
- Buyer and seller records
- Settlement records

### Commodity Auction Plugin

Supports auctions for physical commodities and standardized commodity lots.

Features include:

- Commodity identification
- Lot registration
- Quantity
- Grade
- Quality
- Inspection
- Delivery terms
- Bid management
- Reserve prices
- Auction results
- Buyer and seller records
- Fees
- Settlement
- Delivery records

### Service Auction Plugin

Supports auctions in which businesses or individuals bid to provide services.

Features include:

- Service registration
- Provider identification
- Service specifications
- Qualification requirements
- Delivery requirements
- Bid submission
- Bid comparison
- Selection rules
- Contract terms
- Winning provider records
- Settlement records
- Performance records
- Dispute records

### Procurement Auction Plugin

Supports competitive purchasing auctions in which suppliers submit bids to fulfill a defined procurement requirement.

Features include:

- Procurement request registration
- Buyer identification
- Product or service requirements
- Supplier registration
- Qualification requirements
- Bid submission
- Bid comparison
- Award determination
- Contract records
- Supplier records
- Purchase terms
- Settlement records
- Audit records

### Freelance and Contract Auction Plugin

Supports competitive auctions for freelance work, contracts, projects, and professional services.

Features include:

- Project registration
- Scope definition
- Requirements
- Provider qualifications
- Bid submission
- Proposal records
- Selection rules
- Award records
- Contract records
- Milestone records
- Payment records
- Dispute records
- Immutable project history

### Energy Auction Plugin

Supports auctions for electricity, renewable energy, capacity, energy credits, and other applicable energy products.

Features include:

- Energy product registration
- Quantity
- Delivery period
- Delivery location
- Generation source
- Bid management
- Reserve prices
- Auction rules
- Winning bid records
- Delivery records
- Settlement
- Verification
- Immutable transaction history

### Carbon and Environmental Asset Auction Plugin

Supports auctions involving environmental credits, certificates, offsets, and other transferable environmental assets where applicable.

Features include:

- Asset registration
- Issuer identification
- Quantity
- Certification
- Verification
- Vintage information
- Geographic information
- Ownership history
- Bid management
- Auction results
- Retirement records
- Transfer records
- Settlement
- Immutable asset history

### Financial Asset Auction Plugin

Supports auction mechanisms for financial instruments and other regulated assets where legally permissible.

Features include:

- Asset identification
- Eligibility requirements
- Participant verification
- Bid management
- Auction rules
- Pricing rules
- Winning bid determination
- Transaction records
- Settlement records
- Regulatory records
- Immutable transaction history

### Digital Asset Auction Plugin

Supports auctions for transferable digital assets.

Features include:

- Asset registration
- Asset identification
- Ownership verification
- Transfer rules
- Bid management
- Auction execution
- Winning bid records
- Transfer records
- Settlement records
- Provenance
- Immutable ownership history

### Custom Auction Plugin

Provides a standardized framework for creating additional auction types not covered by the predefined plugins.

A Custom Auction Plugin must define:

- Auction asset
- Participant types
- Eligibility requirements
- Bid format
- Bid visibility requirements
- Auction duration
- Ranking method
- Winner determination
- Pricing method
- Reserve-price rules
- Fees
- Settlement rules
- Verification requirements
- Audit requirements
- Dispute procedures
- Required immutable records

Custom plugins must inherit the core OpenBid Ledger requirements and may not disable immutable logging, auditability, bid transparency, or host accountability.

---

## Security and Integrity Requirements

OpenBid Ledger implementations must protect the integrity of auction records and prevent unauthorized modification.

The specification requires:

- Secure authentication
- Access controls
- Least-privilege administration
- Bid integrity protection
- Ledger integrity protection
- Tamper detection
- Immutable event recording
- Privileged-action logging
- Security-event logging
- Record verification
- Independent audit capability

Security mechanisms must not create undisclosed administrative capabilities that undermine the transparency and immutability requirements of the specification.

## Transparency Requirements

An implementation must provide sufficient information for applicable participants to understand and verify an auction.

Depending on the applicable access level, this may include:

- Auction identity
- Advertising inventory
- Auction rules
- Ruleset version
- Bid history
- Bid timestamps
- Bid status
- Winning bid
- Clearing price
- Impression Unit
- Click records
- Impression records
- Fees
- Billing calculations
- Settlement calculations
- Administrative events
- Verification information

The implementation must not selectively expose or conceal auction information for the purpose of manipulating auction participation or outcomes.

## Auction Certificate

Each completed auction should produce a verifiable Auction Certificate containing the information necessary to establish the identity, rules, activity, result, and integrity of the auction.

The certificate may include:

- Auction identifier
- Auction type
- Inventory identifier
- Ruleset identifier
- Ruleset version
- Auction start time
- Auction end time
- Participating bids
- Bid sequence
- Winning bid
- Clearing price
- Applicable fees
- Impression Unit where applicable
- Validated clicks where applicable
- Validated impressions where applicable
- Settlement information
- Ledger verification information
- Cryptographic verification data

## Non-Retroactive Operation

OpenBid Ledger must preserve the historical state of completed auctions.

New rules, configurations, fees, Impression Unit definitions, algorithms, or policies must apply according to their declared activation conditions and must not silently modify historical auctions.

Historical records must remain associated with the rules and configuration under which the applicable auction occurred.

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
  - [https://roxanneardary.com/openbid-ledger/](https://roxanneardary.com/openbid-ledger/)  

---

## License & Notice Requirements

OpenBid Ledger is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- OpenBid Ledger specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
