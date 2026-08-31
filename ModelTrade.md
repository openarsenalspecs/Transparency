# ModelTrade Specification
**The AI Trade Network**
- HTML Mirror:  [https://roxanneardary.com/modeltrade-specification/](https://roxanneardary.com/modeltrade-specification/)  

---

## Overview

ModelTrade is a federated, open source AI trade network for publishing, discovering, sharing, licensing, buying, selling, reviewing, and rating AI models, datasets, applications, and related AI projects.

ModelTrade is designed as a decentralized ecosystem of independently operated nodes. Each node can provide its own community, users, projects, storefronts, moderation policies, and services while participating in a larger federated network.

The specification prioritizes interoperability, user ownership, portability, transparent licensing, creator-controlled commerce, federated discovery, reputation, provenance, and modular deployment.

## Design Principles

ModelTrade shall:

- Support independently operated federated nodes.
- Allow users and organizations to publish AI resources.
- Provide every user with a profile and optional storefront.
- Support free and commercial resources.
- Provide built-in reviews, ratings, and reputation.
- Support searchable models, datasets, projects, creators, and organizations.
- Preserve licensing and provenance information.
- Support versioned AI resources.
- Support user and project portability.
- Avoid mandatory dependence on a single vendor or service provider.
- Separate core functionality from optional integrations.
- Support local-first operation where practical.
- Provide transparent federation mechanisms.
- Support self-hosted deployments.
- Support interoperability between compatible nodes.
- Keep users in control of their published resources and account data.

---

## Core Identity Module

The Identity Module shall provide the foundational identity services required by the network.

Features include:

- User registration
- Authentication
- Usernames
- Unique user identifiers
- Account profiles
- Account recovery
- Session management
- Security controls
- Multi-factor authentication support
- Account export
- Account deletion
- Identity portability
- Identity verification
- Federated identity discovery

## Core Profile Module

The Profile Module shall provide public profiles for individuals and organizations.

Profiles may contain:

- Display name
- Username
- Biography
- Profile image
- Organization information
- External links
- Published projects
- Published models
- Published datasets
- Published applications
- Storefront
- Collections
- Reviews written
- Reviews received
- Ratings received
- Followers
- Following
- Reputation
- Verification status
- Featured projects
- Activity information

## Core Organization Module

The Organization Module shall allow groups to operate as shared entities.

Features include:

- Organization profiles
- Organization verification
- Multiple administrators
- Team membership
- Shared projects
- Shared storefronts
- Contributor management
- Role-based permissions
- Shared licensing information
- Shared analytics
- Organization-level publishing

## Core Federation Module

The Federation Module shall allow independent ModelTrade nodes to communicate and exchange compatible information.

Features include:

- Node identity
- Node discovery
- Node metadata
- Node verification
- Federated user discovery
- Federated project discovery
- Federated model discovery
- Federated dataset discovery
- Federated storefront discovery
- Federated search
- Cross-node references
- Federation synchronization
- Federation event handling
- Federation provenance
- Selective federation
- Node allowlists
- Node blocklists
- Local federation policies
- Public nodes
- Private nodes
- Community nodes
- Organization nodes

Federation shall not require every node to trust every other node.

Node operators shall be able to determine which external nodes and resources they accept, display, synchronize, or block.

## Core Project Module

The Project Module shall provide a common container for related AI resources.

Projects may contain:

- Models
- Datasets
- Applications
- APIs
- Documentation
- Evaluations
- Demonstrations
- Publications
- Dependencies
- Related projects
- Provenance information
- Version information
- Licensing information
- Discussions
- Reviews
- Ratings

Projects may be free or commercial.

## Core Model Module

The Model Module shall provide first-class support for publishing and distributing AI models.

Features include:

- Model repositories
- Model metadata
- Model documentation
- Model cards
- Model versions
- Releases
- Model files
- Model tags
- Model categories
- Model tasks
- Model architectures
- Parameter information
- Model size
- Hardware requirements
- Framework information
- Runtime requirements
- Dependencies
- Supported languages
- Intended use
- Limitations
- Evaluation information
- Base model relationships
- Fine-tuning relationships
- Derivative relationships
- Model lineage
- Changelogs
- Download statistics
- Purchase statistics
- Reviews
- Ratings
- Licensing
- Pricing

## Core Dataset Module

The Dataset Module shall provide first-class support for publishing and distributing datasets.

Features include:

- Dataset repositories
- Dataset metadata
- Dataset cards
- Dataset versions
- Dataset releases
- Dataset files
- Dataset categories
- Dataset tags
- Dataset size
- Record counts
- File formats
- Languages
- Domains
- Collection methodology
- Source information
- Data quality information
- Data limitations
- Privacy information
- Dataset provenance
- Dataset lineage
- Dataset transformations
- Dataset licensing
- Evaluation information
- Download statistics
- Purchase statistics
- Reviews
- Ratings
- Pricing

## Core Application Module

The Application Module shall support publishing AI applications associated with models, datasets, projects, or independent functionality.

Features include:

- Application pages
- Application documentation
- Application versions
- Application demonstrations
- Application licensing
- Application pricing
- Application subscriptions
- Model dependencies
- Dataset dependencies
- API dependencies
- Application reviews
- Application ratings

## Core Search Module

The Search Module shall provide simple and advanced discovery across the ModelTrade network.

Users shall be able to search by:

- Keyword
- Project name
- Model name
- Dataset name
- Application name
- Creator
- Organization
- Node
- Category
- Tag
- License
- Framework
- Language
- Task
- Price
- Rating
- Review count
- Popularity
- Download count
- Sales
- Release date
- Update date

Search shall support:

- Keyword search
- Exact-name search
- Partial-name search
- Fuzzy matching
- Advanced filtering
- Sorting
- Relevance ranking
- Federated search
- Local search
- Network-wide discovery

## Core Discovery Module

The Discovery Module shall help users find relevant AI resources without requiring a specific search query.

Features include:

- Trending models
- Trending datasets
- Trending projects
- Trending creators
- Trending storefronts
- New releases
- Recently updated resources
- Popular resources
- Highly rated resources
- Most reviewed resources
- Free resources
- Commercial resources
- Related projects
- Similar resources
- Featured creators
- Featured collections

## Core Storefront Module

The Storefront Module shall provide each eligible user or organization with a personal marketplace.

Features include:

- Personal storefronts
- Organization storefronts
- Storefront descriptions
- Storefront branding
- Featured products
- Product categories
- Product collections
- Free products
- Paid products
- Pay-what-you-want products
- Subscription products
- Tiered pricing
- Product bundles
- Discounts
- Promotional pricing
- Seller policies
- Refund policies
- Licensing information
- Storefront reviews
- Storefront ratings
- Seller verification
- Storefront analytics

## Core Marketplace Module

The Marketplace Module shall provide network-wide discovery and commerce for AI resources.

Features include:

- Marketplace listings
- Local marketplace listings
- Federated marketplace listings
- Product discovery
- Product comparison
- Featured products
- Trending products
- New products
- Popular products
- Highest-rated products
- Free resources
- Paid resources
- Creator discovery
- Organization discovery
- Related products
- Similar projects

Marketplace results shall identify the node responsible for the resource.

## Core Commerce Module

The Commerce Module shall provide standardized support for transactions involving digital AI resources.

Features include:

- Product listings
- Product pricing
- Currency support
- Shopping carts
- Checkout
- Orders
- Receipts
- Purchase history
- Seller accounts
- Buyer accounts
- Seller balances
- Revenue records
- Refunds
- Cancellations
- Discounts
- Coupons
- Bundles
- Promotional campaigns
- Transaction records

Payment processing shall remain modular and shall not require a specific payment provider.

## Core Digital Delivery Module

The Digital Delivery Module shall control access to purchased resources.

Features include:

- Authorized downloads
- Download permissions
- Access tokens
- License keys
- Version-specific access
- Subscription access
- API access
- Download limits
- Expiration controls
- Access revocation
- Purchase verification
- Digital receipts

## Core Licensing Module

The Licensing Module shall clearly identify the rights and restrictions associated with every published resource.

Features include:

- Open source licenses
- Proprietary licenses
- Custom licenses
- Commercial licenses
- Noncommercial licenses
- Attribution requirements
- Redistribution terms
- Modification terms
- Dataset restrictions
- Model restrictions
- Usage restrictions
- Training restrictions
- Derivative-work terms
- License versioning
- License compatibility information

The platform license and the license governing an individual model, dataset, application, or project shall be treated as separate licensing layers.

## Core Versioning Module

The Versioning Module shall maintain distinct versions of published resources.

Features include:

- Immutable versions
- Release tags
- Version history
- Changelogs
- Version comparisons
- Version-specific downloads
- Version-specific purchases
- Version-specific licensing
- Version-specific pricing
- Version-specific reviews
- Version-specific ratings
- Archived versions

Reviews and ratings shall identify the version to which they apply.

## Core Provenance Module

The Provenance Module shall record relationships between AI resources and their sources.

Features include:

- Model provenance
- Dataset provenance
- Source attribution
- Training dataset declarations
- Base model declarations
- Fine-tuning relationships
- Derivative relationships
- Dataset transformation history
- Version lineage
- Dependency lineage
- Provenance records
- Provenance verification
- Provenance display

The system should make it possible to trace relationships such as:

Model → Base Model → Training Dataset → Source Data

## Core Dependency Module

The Dependency Module shall allow projects to declare dependencies on other resources.

Supported dependencies may include:

- Models
- Datasets
- Applications
- APIs
- Libraries
- Projects

Dependency information shall include:

- Dependency name
- Version
- Source node
- License
- Availability
- Required version
- Compatibility information

## Core Review Module

The Review Module shall provide built-in user reviews for marketplace resources and creators.

Features include:

- Written reviews
- Product reviews
- Project reviews
- Creator reviews
- Seller reviews
- Version-specific reviews
- Verified purchase reviews
- Verified acquisition reviews
- Review responses
- Review editing
- Review history
- Review reporting
- Review moderation
- Review provenance
- Review timestamps

Creators shall be able to respond to reviews but shall not be able to unilaterally delete legitimate reviews.

## Core Rating Module

The Rating Module shall provide structured ratings for resources and creators.

Features include:

- Five-star ratings
- Overall ratings
- Version ratings
- Model ratings
- Dataset ratings
- Application ratings
- Project ratings
- Creator ratings
- Seller ratings
- Rating distributions
- Verified-user ratings
- Recent ratings
- Lifetime ratings

## Core Review Integrity Module

The Review Integrity Module shall protect the reliability of the marketplace reputation system.

Features include:

- Verified purchase indicators
- Verified acquisition indicators
- One rating per eligible user per version
- Duplicate review detection
- Suspicious review detection
- Review manipulation detection
- Review abuse reporting
- Review moderation
- Transparent moderation records
- Seller responses
- Review history
- Review provenance

## Core Reputation Module

The Reputation Module shall provide transparent reputation information for creators, sellers, organizations, and other participating entities.

Potential reputation signals include:

- Ratings
- Reviews
- Verified purchases
- Successful transactions
- Account history
- Project history
- Community participation
- Verification status
- Moderation history
- Node reputation

Reputation calculations shall be documented and should not rely solely on an unexplained proprietary score.

## Core Collections Module

The Collections Module shall allow users to organize and share resources.

Collections may contain:

- Models
- Datasets
- Applications
- Projects
- Creators
- Storefronts

Collections may be:

- Private
- Public
- Shared
- Collaborative
- Federated

## Core Social Module

The Social Module shall provide community discovery and relationship features.

Features include:

- Following users
- Following organizations
- Following projects
- Following models
- Following datasets
- Following nodes
- Favorites
- Bookmarks
- Activity feeds
- Creator updates
- Project updates
- Release notifications

## Core Notification Module

The Notification Module shall provide notifications for important platform activity.

Notifications may include:

- Purchases
- Sales
- Reviews
- Ratings
- Replies
- New versions
- Price changes
- Product updates
- New followers
- New projects
- Federation events
- Moderation events
- Account security events

## Core Evaluation Module

The Evaluation Module shall allow creators and communities to publish performance information.

Features include:

- Model benchmarks
- Dataset benchmarks
- Evaluation datasets
- Performance metrics
- Accuracy measurements
- Speed measurements
- Resource requirements
- Evaluation methodology
- Evaluation results
- Reproducibility information
- Creator evaluations
- Community evaluations
- Third-party evaluations
- Evaluation history

## Core Demonstration Module

The Demonstration Module shall allow projects to provide interactive demonstrations.

Supported demonstrations may include:

- Text interfaces
- Chat interfaces
- Image interfaces
- Audio interfaces
- Video interfaces
- Model playgrounds
- Dataset explorers
- Interactive applications
- API demonstrations

## Core Moderation Module

The Moderation Module shall allow node operators and authorized moderators to manage platform activity.

Features include:

- User reporting
- Product reporting
- Review reporting
- Dataset reporting
- Model reporting
- Copyright complaint workflows
- License violation reporting
- Abuse reporting
- Spam detection
- Moderator tools
- Node-level moderation
- Federation-level blocking
- Moderation history
- Appeals
- Transparent moderation policies

Moderation decisions made by one node shall not automatically require every federated node to take the same action.

## Core Trust and Verification Module

The Trust and Verification Module shall provide visible indicators for verified entities and resources.

Verification levels may include:

- Unverified
- Account verified
- Identity verified
- Creator verified
- Organization verified
- Seller verified
- Provenance verified
- Model provenance verified
- Dataset provenance verified
- Purchase verified

Verification indicators shall clearly communicate what has actually been verified.

## Core File Integrity Module

The File Integrity Module shall provide mechanisms for verifying digital resources.

Features include:

- Cryptographic hashes
- File checksums
- Artifact verification
- Version integrity
- Download integrity verification
- File manifests
- Dependency manifests
- Signed releases
- Optional cryptographic signatures

## Core API Module

The API Module shall provide standardized interfaces for programmatic access.

APIs may provide access to:

- Users
- Profiles
- Organizations
- Projects
- Models
- Datasets
- Applications
- Search
- Federation
- Storefronts
- Products
- Orders
- Reviews
- Ratings
- Licensing
- Provenance
- Analytics

## Core Federation API Module

The Federation API Module shall provide standardized interfaces for node communication.

Federation services may include:

- Node discovery
- Identity discovery
- Profile discovery
- Project discovery
- Model discovery
- Dataset discovery
- Search
- Reviews
- Ratings
- Follows
- Updates
- Storefront information
- Product information
- Availability information
- Federation events

## Core Import and Export Module

The Import and Export Module shall allow users to move their information between compatible systems.

Supported exports may include:

- Profiles
- Projects
- Model metadata
- Dataset metadata
- Reviews
- Collections
- Storefronts
- Licensing information
- Provenance
- Federation metadata

## Core Portability Module

The Portability Module shall reduce dependence on individual nodes.

Features include:

- Profile migration
- Project migration
- Storefront migration
- Metadata migration
- Collection migration
- Identity portability
- Redirects from previous locations
- Historical project preservation
- Federated identity continuity

## Core Permissions Module

The Permissions Module shall provide granular access control.

Supported roles may include:

- Owner
- Administrator
- Maintainer
- Contributor
- Moderator
- Reviewer
- Finance manager
- Store manager

Permissions may be assigned separately for:

- Profiles
- Organizations
- Projects
- Models
- Datasets
- Storefronts
- Commerce
- Moderation
- Federation

## Core Analytics Module

The Analytics Module shall provide creators and organizations with information about their resources.

Analytics may include:

- Profile views
- Storefront views
- Product views
- Downloads
- Purchases
- Revenue
- Conversion rates
- Ratings
- Reviews
- Followers
- Popular products
- Search impressions
- Version adoption

Analytics should provide useful aggregate information without unnecessarily exposing individual user behavior.

## Core Creator Dashboard Module

The Creator Dashboard shall provide a unified management interface for:

- Profiles
- Projects
- Models
- Datasets
- Applications
- Storefronts
- Products
- Orders
- Sales
- Revenue
- Reviews
- Ratings
- Followers
- Analytics
- Licenses
- Releases
- Federation activity

## Core Buyer Dashboard Module

The Buyer Dashboard shall provide access to:

- Purchased products
- Download access
- Licenses
- Receipts
- Subscriptions
- Saved products
- Favorites
- Collections
- Reviews
- Ratings
- Followed creators
- Followed projects
- Purchase history

## Core User Interface Module

The User Interface Module shall provide a user-friendly interface suitable for developers, researchers, organizations, creators, sellers, and general users.

Primary interface areas should include:

- Home
- Search
- Explore
- Marketplace
- Models
- Datasets
- Projects
- Creators
- Storefronts
- Collections
- Dashboard
- Notifications
- Profiles

Important product information should be clearly visible, including:

- Price
- License
- Rating
- Review count
- Verification status
- Version
- Size
- Last update
- Source node
- Provenance information

## Core Accessibility Module

The Accessibility Module shall support accessible use of the platform.

Features include:

- Keyboard navigation
- Screen-reader compatibility
- Accessible forms
- Accessible search
- Accessible marketplace controls
- Adjustable text sizing
- High-contrast support
- Semantic interface elements
- Accessible media controls

## Core Internationalization Module

The Internationalization Module shall support global deployment.

Features include:

- Multiple interface languages
- Localized interfaces
- Currency localization
- Date localization
- Number localization
- Right-to-left language support
- International seller support

## Core Audit Module

The Audit Module shall maintain records of important system activity.

Audit records may include:

- Administrative actions
- Commerce actions
- Federation events
- Moderation actions
- Account security events
- License changes
- Product changes
- Pricing changes
- Review moderation
- Version history

## Core Transparency Module

The Transparency Module shall make important information about users, resources, transactions, licensing, and federation visible and understandable.

Transparency features may include:

- License display
- Provenance display
- Verification explanations
- Review verification
- Version history
- Pricing history
- Seller information
- Node information
- Moderation information
- Reputation methodology
- Federation status

## Core Storage Module

The Storage Module shall provide an abstraction layer for storing AI resources.

Supported storage approaches may include:

- Local storage
- Object storage
- Distributed storage
- External storage
- Content-addressed storage
- Replicated storage

Storage providers shall be replaceable without requiring changes to the core specification.

## Core Infrastructure Independence

ModelTrade shall avoid requiring a specific:

- Cloud provider
- Database
- Payment processor
- AI provider
- Storage provider
- Identity provider
- Search engine
- Inference provider

Infrastructure integrations should be replaceable modules.

---

## Optional Plugin Modules

ModelTrade shall support optional plugins that extend functionality without requiring changes to the core specification.

Potential plugins include:

- Payment providers
- Tax services
- Identity providers
- Storage providers
- Search engines
- AI inference providers
- Compute providers
- Email providers
- Analytics systems
- Verification services
- Content moderation services
- Authentication systems
- Decentralized identity systems
- Enterprise integrations
- External marketplaces

Plugins should have defined interfaces and should not compromise the interoperability of the core network.

## Optional Subscription Module

The Subscription Module may provide:

- Recurring subscriptions
- Subscription products
- Subscription tiers
- Subscription access
- Subscription management
- Subscription cancellation
- Subscription analytics

## Optional Donation Module

The Donation Module may provide:

- Creator donations
- Project donations
- Organization donations
- Recurring donations
- Donation goals
- Donation history

## Optional Sponsorship Module

The Sponsorship Module may provide:

- Creator sponsorships
- Project sponsorships
- Organization sponsorships
- Recurring sponsorships
- Sponsorship tiers

## Optional Bounty Module

The Bounty Module may allow users and organizations to fund requested work.

Features may include:

- Bounties
- Funding targets
- Contributor submissions
- Milestones
- Completion verification
- Bounty payments
- Dispute handling

## Optional Crowdfunding Module

The Crowdfunding Module may support:

- Project campaigns
- Funding goals
- Campaign rewards
- Campaign updates
- Contribution tracking
- Campaign completion

## Optional Inference Module

The Inference Module may allow creators to offer models as hosted services.

Features may include:

- Hosted inference
- API endpoints
- Usage metering
- API pricing
- Usage limits
- Authentication
- Usage analytics
- Inference subscriptions

## Optional Compute Marketplace Module

The Compute Marketplace may allow participants to offer AI compute resources.

Features may include:

- Compute listings
- GPU availability
- CPU availability
- Memory availability
- Storage availability
- Pricing
- Availability schedules
- Provider ratings
- Provider reviews
- Usage metering

## Optional Training Marketplace Module

The Training Marketplace may allow creators to offer model training services.

Features may include:

- Training requests
- Training jobs
- Training pricing
- Dataset selection
- Model selection
- Training specifications
- Training results
- Provider ratings
- Provider reviews

## Optional Evaluation Services Module

The Evaluation Services Module may allow users to purchase independent model or dataset evaluations.

Features may include:

- Evaluation requests
- Evaluation packages
- Evaluation pricing
- Benchmark execution
- Evaluation reports
- Evaluator profiles
- Evaluator ratings
- Evaluator reviews

## Optional Certification Module

The Certification Module may provide optional certification programs for:

- Creators
- Organizations
- Models
- Datasets
- Applications
- Provenance
- Security
- Compliance

Certification status should remain distinct from community ratings and reviews.

## Optional Enterprise Module

The Enterprise Module may provide:

- Enterprise organizations
- Private projects
- Private storefronts
- Private nodes
- Team management
- Advanced permissions
- Enterprise licensing
- Enterprise analytics
- Private federation
- Internal marketplaces

## Optional Affiliate Module

The Affiliate Module may support:

- Affiliate links
- Creator referrals
- Product referrals
- Referral tracking
- Commission rules
- Affiliate reporting

## Optional Revenue Sharing Module

The Revenue Sharing Module may allow project owners to distribute revenue among contributors.

Features may include:

- Contributor revenue shares
- Organization revenue shares
- Automated distribution rules
- Revenue reporting
- Contributor statements

## Optional Marketplace Promotion Module

The Promotion Module may provide:

- Featured listings
- Promotional campaigns
- Sponsored listings
- Discount campaigns
- Product launches
- Creator promotions

Promotional listings should be clearly identified so that users can distinguish them from organic search results.

## Governance

ModelTrade nodes may establish their own governance policies while remaining interoperable with the broader ModelTrade specification.

Node governance may define:

- Membership policies
- Federation policies
- Moderation policies
- Commerce policies
- Verification policies
- Seller requirements
- Content policies
- Resource policies
- Administrative permissions

Federation shall preserve node autonomy while providing standardized interoperability.

## Security

ModelTrade implementations should provide security mechanisms appropriate to the resources and transactions they support.

Security considerations include:

- Secure authentication
- Access control
- Session security
- File integrity
- Download authorization
- Transaction security
- API authentication
- Audit logging
- Abuse prevention
- Account protection
- Secure federation
- Data protection

## Data Ownership and Portability

Users should be able to export their profiles, projects, metadata, collections, storefront information, and other supported data.

The system should minimize unnecessary lock-in to individual nodes.

Where technically and legally possible, users should be able to migrate their work to another compatible ModelTrade node.

## Federation Trust

Federation shall use explicit trust relationships.

Nodes should be able to:

- Accept federation from selected nodes
- Reject federation from selected nodes
- Temporarily suspend federation
- Block nodes
- Block users
- Block resources
- Preserve local moderation decisions
- Preserve local commerce policies

A federated relationship shall not imply universal endorsement of another node's content or policies.

## Marketplace Trust

Marketplace transactions should preserve sufficient information to establish:

- Who published the resource
- Which node hosts the resource
- What was purchased
- Which version was purchased
- What license applies
- What price was paid
- Whether the transaction was verified
- Which creator received the transaction
- Which reviews are associated with the purchase

## Resource Identity

ModelTrade should provide stable identifiers for published resources.

Identifiers should distinguish:

- Node
- Creator
- Organization
- Project
- Resource
- Version

Resource identifiers should support reliable references between federated projects.

## Resource Relationships

The platform should support relationships such as:

- Project contains Model
- Project contains Dataset
- Model derived from Model
- Model trained on Dataset
- Dataset derived from Dataset
- Application uses Model
- Application uses Dataset
- Project depends on Model
- Project depends on Dataset
- Project depends on Application
- Resource belongs to Creator
- Resource belongs to Organization
- Resource hosted by Node

## Economic Transparency

Commercial resources should clearly communicate:

- Price
- Currency
- License
- Included resources
- Version
- Subscription requirements
- Renewal terms
- Refund terms
- Seller identity
- Node identity

Users should not be required to purchase a resource without being able to determine the basic rights and conditions associated with the purchase.

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
  - [https://roxanneardary.com/modeltrade/](https://roxanneardary.com/modeltrade/)  

---

## License & Notice Requirements

ModelTrade is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- ModelTrade specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
