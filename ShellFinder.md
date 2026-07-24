# ShellFinder  
*Where Hidden Companies Come to Light*

---

## Overview

**ShellFinder** is an open-source forensic AI platform designed to provide full transparency into OTC (Over-The-Counter) companies. The platform maps **founders, officers, subsidiaries, assets, and corporate networks**, uncovering hidden ownership structures, shell companies, and suspicious activity.  

By integrating **financial, legal, real estate, and social intelligence**, ShellFinder empowers **investors, researchers, and regulators** to make informed decisions and gain insight into complex OTC networks.  

---

## Key Features

### Corporate Forensics
- Track OTC companies from inception to present  
- Map founders, officers, and board members  
- Reconstruct historical corporate networks and shell companies  
- Visualize ownership, assets, and subsidiaries  

### Financial Intelligence
- Monitor insider trades and share issuances  
- Analyze liquidity, revenue streams, debt, and off-balance sheet activity  
- Track derivatives and inter-company financial relationships  
- Detect suspicious patterns and potential market manipulation  

### Legal & Regulatory Monitoring
- Integrate SEC, FINRA, PACER, and state court filings  
- Track bankruptcy, liens, and lawsuits  
- Automated legal document extraction and summary  
- Compliance scoring and risk alerts  

### Asset Tracking
- Map real estate, equipment, vehicles, vessels, and aircraft  
- Track intellectual property (patents, trademarks, copyrights)  
- Detect shared addresses and clustering of assets  

### Social & Media Intelligence
- Monitor Twitter, Reddit, Discord, StockTwits  
- Detect OTC chatter, meme stock trends, and influencer mentions  
- Perform sentiment analysis correlated with trading events  
- Identify potential misinformation or manipulative news  

### AI & Predictive Analytics
- Entity resolution across duplicate company records and name changes  
- Network graph analysis for founders, officers, and subsidiaries  
- Anomaly detection for insider activity and shell creation  
- Predictive alerts for potential fraud, shell activity, or suspicious networks  

### Visualization & Dashboard
- Interactive network graphs: founder → officer → company → assets  
- Timeline views of mergers, filings, and asset acquisitions  
- Real-time alerts dashboard with heatmaps and risk scores  
- 3D network visualization and scenario simulations  

---

## Installation

**Prerequisites:**  
- Python 3.11+  
- Node.js 18+  
- PostgreSQL / Clickhouse  
- Neo4j / ArangoDB for graph database  
- Docker & Docker Compose (recommended)

**Clone the repository:**
```bash
git clone https://gitlab.com/Roxanne_Ardary/shellfinder.git
cd shellfinder
```

## Install Python dependencies:
```bash
pip install -r requirements.txt
```
Install Node dependencies (for dashboard):
```bash
cd dashboard/frontend
npm install
```
Start services with Docker Compose:
```bash
docker-compose up -d
```

## Usage
Data Collection: Run scrapers to fetch OTC filings, corporate registries, legal filings, and social media data.
```bash
python src/scrapers/run_scrapers.py
```
Entity Resolution: Process and unify company, founder, and officer data.
```bash
python src/entity_resolution/resolve_entities.py
```
Graph Building: Construct the knowledge graph for analysis.
```bash
python src/graph_builder/build_graph.py
```
Analytics & Alerts: Generate dashboards, risk scores, and predictive alerts.
```bash
python src/analytics/run_analytics.py
python src/alerts/run_alerts.py
```
Dashboard Access: Open the frontend to explore networks and reports.
```bash
cd dashboard/frontend
npm run dev
```

## Repository Structure
```
/otc-forensic-ai
├─ /data               # Raw and processed datasets
├─ /src                # Core scrapers, AI modules, entity resolution, graph builder, analytics, alerts
├─ /dashboard          # Frontend (React/Tailwind/Next.js) and backend
├─ /docs               # Documentation (architecture, API, usage)
├─ /tests              # Unit and integration tests
├─ notice.md           # Project notice with attribution
├─ License.md          # AGPL-3.0+ license with attribution
├─ README.md           # This file
├─ docker-compose.yml  # Docker setup
└─ /assets             # Logo and visual assets
```

## Contributing

ShellFinder is **open-source**. Contributions are welcome!  

- Ensure contributions comply with **AGPL-3.0+** license  
- Include **attribution to Roxanne Ardary / roxanneardary.com** in your changes  
- Verify data accuracy and provide sources  
- Use clear commit messages and maintain code style  

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

---

## Disclaimer

ShellFinder is a **research and transparency tool**. It does **not provide financial, legal, or professional advice**. Users are solely responsible for decisions based on this software.
