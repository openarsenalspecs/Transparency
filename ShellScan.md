# ShellScan: From Shell to Source

**© 2026 Roxanne Ardary | roxanneardary.com**  
**License:** AGPL 3.0+ (mandatory attribution)

---

## **Project Overview**

ShellScan is an open-source platform designed to **track, visualize, and analyze corporate ownership networks** across the financial sector, including shell companies, mortgage lenders, hedge funds, insurance, fintech, and crypto entities.  

The platform provides:  

- **Global transparency** of corporate and officer networks  
- **Predictive intelligence** to detect fraud, shell formation, and systemic risks  
- **Immersive visualization** (2D, 3D, AR) of financial networks  
- **Citizen engagement tools** for research, advocacy, and education  
- **Policy and governance simulations** for regulators and analysts  

**Tagline:** *From Shell to Source.*

---

## **Phases & Features**

| Phase | Features |
|-------|---------|
| **I–V** | Core ingestion: FDIC, SEC, FINRA, NMLS, hedge funds, insurance, fintech, crypto, global registries. Basic Neo4j graph, shell detection AI, dashboards, predictive simulations. |
| **VI–X** | Continuous monitoring, fraud detection, cross-sector intelligence, policy simulators, governance indices, gamified citizen dashboards, immersive visualization, advocacy tools. |
| **XI–XIV** | Real-time transaction monitoring, derivative exposure mapping, global liquidity stress tests, predictive legal risk, officer influence mapping, narrative extraction, supply chain integration, emerging finance (NFTs, DeFi), self-updating AI models, proactive alerts. |

---

## **Core Capabilities**

1. **Data Ingestion & Normalization**  
   - Aggregates data from U.S., international, and blockchain/DeFi sources  
   - Normalizes companies, officers, and ownership networks  

2. **AI & Predictive Analytics**  
   - Shell detection, anomaly detection, corporate collapse prediction  
   - Fraud pattern recognition, hidden influence mapping  
   - Explainable AI and reinforcement learning for investigative prioritization  

3. **Visualization & Dashboards**  
   - Interactive 2D/3D and AR network graphs  
   - Temporal evolution of ownership, officer interlocks, and company networks  
   - Policy sandbox and citizen dashboards  

4. **Monitoring & Alerts**  
   - Regulatory and sanctions alerts  
   - Officer/board changes and suspicious network activity  
   - Multi-domain anomaly detection  

5. **Citizen & Community Engagement**  
   - Gamified research and investigations  
   - Crowdsourced verification and annotation  
   - Educational modules and advocacy toolkit  

6. **Global & Blockchain Integration**  
   - Cross-border corporate networks  
   - DeFi, smart contracts, and NFT ownership mapping  
   - Multi-currency exposure and risk visualization  

7. **Automation & Reporting**  
   - AI-generated investigative briefings and scheduled reports  
   - Exportable dashboards in CSV, JSON, GraphML, or HTML  

8. **Governance & Policy Tools**  
   - Legislative and regulatory simulations  
   - Governance indices for sectors, countries, and companies  

9. **Proactive Intelligence**  
   - Predictive alerts for fraud, shell formation, and network collapse  
   - Cascading failure simulations and global risk heatmaps  

10. **Security & Compliance**  
    - End-to-end encryption  
    - Role-based access control  
    - GDPR and privacy compliance  
    - Full audit logs of AI inferences and alerts  

---

## **Installation**

1. Clone the repository:

```bash
git clone https://gitlab.com/Roxanne_Ardary/ShellScan.git
cd ShellScan
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Configure environment variables and Neo4j connection in src/utils/config.py.

4. Run the scheduler to start data ingestion:
```bash
python src/scheduler/update_all.py
```

5. Start the dashboard:
```bash
python src/dashboard/interactive_ui.py
```

## **Usage**

- Use **Neo4j dashboards** to explore ownership and officer networks  
- Access **AI predictive modules** via `src/ai/` for fraud detection and risk scoring  
- Monitor **alerts** in `src/monitoring/` for regulatory or suspicious activity  
- Contribute to **crowdsourced verification** via the community dashboard  

---

## **Contribution Guidelines**

All contributions must:  

1. Include proper attribution to **Roxanne Ardary & roxanneardary.com**  
2. Be licensed under **AGPL 3.0+**  
3. Follow the repository’s coding, documentation, and naming standards  

For major contributions, please **open an issue or merge request** on GitLab.  

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
  - [https://roxanneardary.com/shellscan/](https://roxanneardary.com/shellscan/)  

---

## License & Notice Requirements

ShellScan is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- ShellScan specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
