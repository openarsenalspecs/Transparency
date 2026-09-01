# LocalAI Builder Specification
**Your AI Without the Subscription Trap.**
- HTML Mirror:  [https://roxanneardary.com/localai-buider-specification/](https://roxanneardary.com/localai-buider-specification/)  

---

## Purpose

LocalAI Builder is an open source, modular AI intelligence and procurement specification designed to help users discover, compare, evaluate, and assemble the specifications, AI models, datasets, software, hardware, machinery, blueprints, and other resources required to build locally hosted systems.

The system is designed for users with varying levels of technical knowledge. It shall translate complex technical, financial, licensing, and compatibility information into understandable recommendations while keeping the user in control of purchasing, licensing, installation, and deployment decisions.

## Core Principles

LocalAI Builder shall prioritize:

- Local hosting and user control where practical
- Perpetual licensing over recurring subscriptions when suitable options exist
- Open source resources where they satisfy user requirements
- Device compatibility as a primary recommendation factor
- Transparent pricing and total cost analysis
- Clear license explanations
- Deep and independent resource discovery
- Vendor-neutral recommendations
- User-defined requirements and constraints
- Human approval before purchases or deployments
- Modular and extensible functionality
- Practical solutions accessible to nontechnical users

---

## User Requirements Module

The system shall ask the user the questions necessary to understand their intended project before making final recommendations.

Questions may include:

- What the user wants to build
- Intended purpose and use
- Required capabilities
- Intended users
- Budget
- One-time or recurring budget preferences
- Technical skill level
- Operating system
- Device type
- Processor
- Memory
- GPU and available VRAM
- Storage
- Network availability
- Offline requirements
- Privacy requirements
- Commercial or noncommercial use
- Licensing requirements
- Redistribution requirements
- Required languages
- Required integrations
- Required performance
- Required physical dimensions where applicable
- Available tools, machinery, workspace, or equipment
- Manufacturing capabilities
- Construction capabilities
- Safety requirements
- Geographic requirements
- Regulatory requirements

The system shall identify missing information that could materially affect a recommendation and ask follow-up questions before producing a final recommendation.

## Device Compatibility Module

The system shall evaluate whether recommended models, software, specifications, machinery, hardware, and other resources are compatible with the user's available equipment.

Compatibility analysis may include:

- CPU architecture
- Processor capability
- RAM
- GPU
- VRAM
- Storage
- Operating system
- Supported software
- Required runtimes
- Required drivers
- Network requirements
- Power requirements
- Physical dimensions
- Ports and interfaces
- Manufacturing capabilities
- Required tools
- Required machinery

Resources shall receive clear compatibility classifications and explanations.

## Deep Search Module

The system shall perform comprehensive searches across multiple search engines and specialized sources rather than relying on a single search algorithm or search provider.

The system shall support searches across:

- General search engines
- Privacy-focused search engines
- Academic resources
- Software repositories
- Model repositories
- Dataset repositories
- Specification repositories
- Hardware catalogs
- Marketplace sites
- Vendor sites
- Manufacturer sites
- Blueprint repositories
- Open hardware repositories
- Machinery catalogs
- Construction resources
- Community resources
- Other relevant public sources

The system shall generate multiple search strategies to identify resources that may be obscured by search ranking algorithms, terminology differences, marketplace structures, or incomplete indexing.

## Resource Discovery Module

The system shall discover and catalog:

- Specifications
- AI models
- Model weights
- Datasets
- Software
- Hardware
- Open hardware designs
- Blueprints
- Schematics
- Machinery
- Tools
- Components
- Housing designs
- Building designs
- Manufacturing plans
- Agricultural systems
- Energy systems
- Infrastructure designs
- Fabrication resources
- Construction resources
- Other resources required to create physical or digital systems

The system shall attempt to identify the original creator, current version, source, seller, marketplace, license, availability, and known alternatives for each resource.

## Resource Identity Module

The system shall determine whether multiple listings represent the same resource, different versions, derivatives, forks, mirrors, or independent resources.

Where possible, identification shall use:

- Resource name
- Creator
- Organization
- Version
- Release date
- Repository
- File information
- Technical specifications
- Documentation
- Model characteristics
- Dataset characteristics
- Design characteristics
- Other identifying information

## Seller and Marketplace Module

The system shall maintain profiles for known sellers, marketplaces, repositories, manufacturers, publishers, model providers, dataset providers, and other resource providers.

Profiles may include:

- Resource categories
- Pricing models
- License practices
- Geographic availability
- Distribution methods
- Local availability
- Download availability
- Documentation
- Support
- Commercial-use options
- Reputation indicators
- Known limitations

The system shall distinguish verified information from seller claims and unverified information.

## Price Comparison Module

The system shall normalize pricing information so users can compare different purchasing models.

Pricing analysis shall include, where applicable:

- One-time purchase price
- Perpetual license price
- Lifetime pricing
- Subscription price
- Usage-based pricing
- Per-user pricing
- Per-device pricing
- Installation costs
- Upgrade costs
- Required hardware
- Hosting costs
- Storage costs
- Maintenance costs
- Required dependencies
- Other material costs

The system shall calculate estimated total cost of ownership over configurable periods.

## Perpetual Licensing Priority Module

The system MUST prioritize perpetual licensing when a suitable perpetual option is available.

A perpetual license shall receive priority over subscription-based licensing when the options provide substantially comparable functionality, compatibility, capability, and legal rights.

The system shall identify recurring payment requirements and explain the financial difference between perpetual and recurring licensing.

If a subscription is recommended when a reasonably comparable perpetual option exists, the system MUST explain why the perpetual option was not selected.

The user may override this priority by explicitly requesting subscription, cloud, or usage-based resources.

## License Intelligence Module

The system shall identify and explain licenses associated with specifications, models, datasets, software, hardware designs, blueprints, machinery designs, documentation, and dependencies.

The system shall explain, where applicable:

- Use rights
- Modification rights
- Commercial-use rights
- Redistribution rights
- Attribution requirements
- Copyleft requirements
- Patent provisions
- Usage restrictions
- Geographic restrictions
- Dataset restrictions
- Model-specific restrictions
- Additional terms

The system shall distinguish between the license of a resource and the licenses of its individual components.

The system shall clearly distinguish legal license text from AI-generated explanations and shall not present AI interpretation as legal advice.

## Skill Level Module

The system shall evaluate the technical skill required to install, configure, operate, modify, manufacture, construct, or otherwise use a resource.

Difficulty levels may range from consumer-level use through expert-level implementation.

The system shall explain the factors contributing to the difficulty score, including required tools, technical knowledge, configuration, fabrication, programming, construction, installation, and maintenance.

## Recommendation Module

The system shall recommend resources based on the complete user requirements profile.

Recommendations shall consider:

- User objective
- Device compatibility
- Budget
- Capability
- Licensing
- Perpetual ownership
- Local hosting
- Privacy
- Skill level
- Installation requirements
- Maintenance
- Quality
- Documentation
- Availability
- Total cost
- Long-term viability

The system shall provide multiple options where appropriate, including budget, value, performance, and ownership-focused options.

## Model Recommendation Module

The system shall recommend AI models based on the user's intended application, available hardware, required capabilities, license requirements, performance requirements, and budget.

The system shall identify:

- Model capability
- Parameter size
- Context requirements
- Hardware requirements
- Quantization options
- Local hosting capability
- Supported modalities
- Language capabilities
- Tool use
- Fine-tuning capability
- License
- Cost
- Installation difficulty

## Dataset Recommendation Module

The system shall recommend datasets appropriate for:

- Training
- Fine-tuning
- Evaluation
- Retrieval
- Classification
- Embeddings
- Domain adaptation
- Testing

Recommendations shall consider dataset quality, size, provenance, freshness, licensing, compatibility, intended purpose, storage requirements, and expected usefulness for the selected model or specification.

## Specification Builder Module

The system shall allow users to describe a desired system and determine which specifications, models, datasets, components, software, hardware, and other resources are needed to create it.

The system shall be capable of producing a dependency-aware build recommendation that identifies:

- Required resources
- Optional resources
- Compatible alternatives
- Estimated costs
- Licensing requirements
- Skill requirements
- Hardware requirements
- Installation or construction requirements
- Potential conflicts
- Missing components

## Open Hardware Module

The system shall support discovery, comparison, evaluation, and recommendation of open hardware designs.

Resources may include:

- Hardware specifications
- Schematics
- Circuit designs
- PCB designs
- Mechanical designs
- CAD files
- Component lists
- Assembly instructions
- Manufacturing instructions
- Fabrication plans
- Open source hardware licenses
- Bill of materials

The system shall evaluate whether a user has the equipment, materials, tools, skills, and manufacturing capabilities required to produce the design.

## Blueprint and Design Module

The system shall support discovery and evaluation of blueprints, plans, schematics, technical drawings, CAD designs, architectural designs, engineering designs, and other build documentation.

The system shall evaluate:

- Required materials
- Dimensions
- Tools
- Machinery
- Skill level
- Construction complexity
- Manufacturing complexity
- License
- Modification rights
- Commercial-use rights
- Estimated material costs
- Compatibility with the user's available resources

## Machinery and Fabrication Module

The system shall support discovery and comparison of machinery and fabrication equipment required to create physical systems.

Resources may include:

- CNC machinery
- 3D printers
- Laser equipment
- Milling equipment
- Welding equipment
- Woodworking equipment
- Metalworking equipment
- Agricultural machinery
- Manufacturing equipment
- Specialized fabrication equipment

The system shall compare purchase cost, perpetual ownership, operating costs, required space, power requirements, materials, skill level, maintenance, and compatibility with intended designs.

## Housing and Construction Module

The system shall support discovery and evaluation of housing designs, building plans, shelters, modular structures, construction systems, and related open designs.

The system shall consider:

- Building materials
- Tools
- Machinery
- Labor requirements
- Construction skill
- Site requirements
- Dimensions
- Environmental requirements
- Local regulations where available
- Estimated material costs
- Design license
- Modification rights
- Construction suitability

The system shall clearly distinguish conceptual designs from professionally engineered or legally approved construction plans.

## Physical Resource Matching Module

The system shall match physical designs to the user's actual capabilities.

The system shall determine whether the user has access to:

- Required tools
- Required machinery
- Required materials
- Required workspace
- Required power
- Required transportation
- Required fabrication capabilities
- Required construction skills

Where the user lacks a required capability, the system shall identify alternatives such as purchasing components, outsourcing fabrication, using a different design, or selecting a design requiring fewer resources.

## Scoring Module

The system shall score resources according to configurable criteria including:

- User suitability
- Device compatibility
- Capability
- Price
- Total cost of ownership
- License compatibility
- Perpetual ownership
- Local deployment
- Privacy
- Skill requirement
- Documentation
- Quality
- Maintenance
- Availability
- Seller reliability
- Resource maturity

Individual scores shall remain visible so users can understand how the overall recommendation was determined.

## Evidence and Verification Module

The system shall maintain an evidence trail for material recommendation claims.

Information shall be classified where possible as:

- Verified
- Source-provided
- Seller-provided
- Community-reported
- Inferred
- Unknown

The system shall not represent assumptions as verified facts.

## Alternatives Module

For each major recommendation, the system should identify suitable alternatives including:

- Lower-cost options
- Free options
- Open source options
- Perpetually licensed options
- Easier options
- More capable options
- Smaller options
- Locally hosted options
- Better-supported options
- More permissively licensed options

## Conflict Detection Module

The system shall identify conflicts between:

- User requirements
- Device capabilities
- Resource requirements
- Licenses
- Dependencies
- Hardware
- Software
- Budget
- Construction requirements
- Manufacturing requirements
- Local deployment requirements

Potential conflicts shall be clearly explained before a recommendation is finalized.

## Local Deployment Module

The system shall prioritize resources that can operate locally where practical.

The system shall identify:

- Local-capable models
- CPU-capable models
- GPU requirements
- Quantized models
- Local runtimes
- Offline resources
- Storage requirements
- Memory requirements
- Network requirements
- Required dependencies

The system should progressively reduce unnecessary dependence on external services.

## Plug and Play Module

Where supported, the system shall provide guided workflows that move users from resource discovery through configuration and deployment.

A deployment recommendation may include:

- Selected resources
- Required hardware
- Required software
- Required dependencies
- Installation steps
- Configuration
- Licensing requirements
- Storage requirements
- Verification steps
- Estimated cost
- Skill level

The system shall maintain modularity so deployment functionality does not require a specific vendor, platform, operating system, or service.

## User Approval Module

The system may research, compare, score, and recommend resources automatically.

The system shall require explicit user authorization before:

- Making purchases
- Creating paid accounts
- Starting subscriptions
- Accepting licenses
- Downloading restricted resources
- Uploading user data
- Installing software
- Deploying systems
- Sharing information with third parties

---

## Optional Plugin Modules

Implementations may provide optional plugins for:

- Additional search engines
- Marketplace discovery
- Seller monitoring
- Price history
- Price alerts
- Model repositories
- Dataset repositories
- Specification repositories
- Open hardware repositories
- Blueprint repositories
- CAD resources
- Hardware price comparison
- Machinery catalogs
- Construction resources
- License databases
- Automated compatibility testing
- Model benchmarking
- Dataset evaluation
- Local deployment
- Guided installation
- Hardware detection
- CAD analysis
- Bill of materials generation
- Material cost estimation
- Manufacturing estimation
- Construction estimation
- Offline resource indexing
- Personal procurement history
- Budget tracking
- Team procurement
- Enterprise procurement
- API access

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
  - [https://roxanneardary.com/localai-builder/](https://roxanneardary.com/localai-builder/)  

---

## License & Notice Requirements

LocalAI Builder is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- LocalAI Builder specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
