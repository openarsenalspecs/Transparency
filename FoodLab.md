# FoodLab

**FoodLab — The truth behind every brand**

FoodLab is an open-source transparency platform designed to document, track, and connect food brands with scientific evidence of chemical exposure, toxicology findings, and relevant regulatory or legislative frameworks.

It is built to provide a structured, evidence-based system where every data point is traceable back to its original source.

---

## 🔍 Mission

FoodLab exists to create a fully transparent, verifiable database of:

- Food brands and products
- Chemical compounds detected in food
- Scientific studies and published research
- Regulatory limits, recalls, and enforcement actions
- Legislative provisions affecting food and chemical safety

The goal is to connect fragmented public data into a unified, queryable system of truth.

---

## 🚀 Features

### 🧪 Core Database System
- Relational structure connecting brands, chemicals, studies, and laws
- Fully cross-linked entity system for traceable data relationships
- Designed for auditability and long-term data integrity

### 🏷️ Brand Transparency Profiles
- Dedicated page for every food brand
- Aggregated list of all detected chemicals across studies
- Product categories and tested variants
- Historical timeline of findings
- Brand-level summary of chemical exposure patterns

### ☣️ Chemical Intelligence Layer
- Detailed chemical profiles with CAS identifiers
- Toxicity classifications (e.g., carcinogen, endocrine disruptor, neurotoxin)
- Detection records across brands and food categories
- Regulatory thresholds and contextual safety references

### 📚 Study & Evidence Tracking
- Direct linking to peer-reviewed and government-funded studies
- Extraction of:
  - Tested food items
  - Detected chemicals
  - Brand mentions
- DOI, PubMed, and official report integration
- Clear labeling of verified and unverified sources

### ⚖️ Legislative & Protection Tracking
- Catalog of food safety and chemical regulation laws
- Breakdown of provisions that may:
  - Limit liability for manufacturers
  - Create regulatory exemptions
  - Alter enforcement standards
- Mapping of legislation to specific chemicals and brands

### 🔎 Search & Discovery System
- Search by brand, chemical, study, or legislation
- Advanced filtering by toxicity type, category, and jurisdiction
- Cross-referenced navigation between all dataset entities

### 📊 Analytics & Visualization
- Brand toxicity summaries and comparisons
- Chemical prevalence across food categories
- Time-based trend analysis
- Regulatory impact visualization dashboards

### 🌐 Open Source Infrastructure
- Hosted on GitLab under AGPL-3.0+
- Fully transparent backend, schema, and ETL pipeline design
- Version-controlled dataset evolution
- Community-driven development model

### 🤝 Community Contributions
- Open submission of new studies and datasets
- Structured review and verification workflow
- Public issue tracking for corrections and updates

### 🔐 Transparency & Auditability
- Every entry must be traceable to a primary source
- Full citation requirement for all data points
- Historical logging of changes and updates
- Separation of verified vs. pending data

---

## 🧩 System Architecture (Planned)

- PostgreSQL relational database for structured entity relationships
- FastAPI or Node.js backend for data access and aggregation
- ETL pipelines for ingesting government and scientific datasets
- Next.js frontend for brand, chemical, and study profile pages
- Visualization layer for analytics and reporting dashboards

---

## 🜁 Specification Branding License (SBL):  
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

Optional:
- Specification Branding License (SBL)
  - attribution-free commercial deployment
  - pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/foodlab/](https://roxanneardary.com/foodlab/)


---

## License & Notice Requirements

FoodLab is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- FoodLab specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
