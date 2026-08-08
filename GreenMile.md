# GreenMile  
**Travel Smarter. Travel Greener.**

GreenMile is an open-source CO₂e (carbon dioxide equivalent) calculator designed to measure, track, and reduce emissions from travel. It focuses heavily on **Scope 3 Category 6 (Business Travel)** while remaining extensible to broader organizational and personal carbon accounting.

It enables individuals, teams, and enterprises to understand the environmental impact of travel decisions and take actionable steps toward reduction.

---

## 🌱 Mission

To make carbon emissions from travel **transparent, measurable, and actionable**, empowering better decisions for a low-carbon future.

---

## 🚀 Core Features

### ⚙️ CO₂e Calculation Engine
- Flight emissions (short-haul and long-haul support)
- Train emissions
- Bus emissions
- Car emissions (average fuel-based)
- Taxi and rideshare emissions
- Distance-based calculation (km / miles support)
- Configurable emission factor system (JSON/YAML-based)
- Trip-level CO₂e computation
- Multi-trip aggregation

---

### ✈️ Business Travel (Scope 3 Category 6)
- Business travel classification
- Employee-level tracking
- Department/team aggregation
- Flight class differentiation (economy/business/first)
- Multi-leg trip support
- Annual corporate travel emissions summaries

---

### 📊 Analytics & Dashboards
- Total CO₂e dashboard (user and organization level)
- Time-based tracking (daily, monthly, yearly)
- Transport-mode breakdowns
- Emissions trend analysis
- Top emission source identification
- Exportable analytics (CSV/JSON)

---

### 🧠 Intelligent Optimization Suggestions
- Alternative transport recommendations
- Emissions reduction estimates per suggestion
- Scenario comparison (“what-if” analysis)
- Route optimization suggestions
- Personalized low-carbon travel recommendations

---

### 👤 User & Profile System
- Individual user profiles
- Personal travel history tracking
- Annual emissions summaries
- Carbon budget and goal setting
- Optional authentication system

---

### 🏢 Organizational Features
- Company-level dashboards
- Department-based emissions tracking
- Employee grouping and comparison
- Corporate annual reporting
- ESG-ready reporting structure
- Audit-friendly emission logs

---

### 🧾 Reporting & Export System
- CSV export (trip and aggregated data)
- JSON export for integrations
- PDF-ready report structure
- Annual sustainability reports
- Scope 3 Category 6 reporting format support

---

### 🌍 Emissions Data Engine
- Configurable emission factor database
- Region-based emission factors
- Load factor adjustments for aviation
- Versioned datasets for transparency
- Explainable calculation outputs
- Full calculation traceability

---

### 🌳 Carbon Offset Layer
- CO₂e to tree-equivalent conversion
- Optional offset estimation per trip
- Net emissions calculation (gross vs offset)
- Offset progress tracking
- Integration-ready offset provider structure

---

### 📡 API & Integration Layer
- REST API for CO₂e calculations
- Batch processing endpoints
- Travel event ingestion API
- Webhook support for external systems
- API authentication tokens
- OpenAPI/Swagger documentation support

---

### 🔌 Integrations (Future Expansion)
- Travel booking systems
- Expense platforms (e.g., corporate expense tools)
- Calendar-based travel detection
- Email receipt parsing (planned)
- Airline itinerary imports

---

### 🧩 Plugin Ecosystem
- Modular emission factor plugins
- Community transport mode extensions
- Dashboard plugins
- Plugin registry system
- Version compatibility management

---

### 🔬 Transparency & Explainability
- Step-by-step emission breakdowns
- “How this was calculated” feature
- Emission factor source attribution
- Adjustable assumptions view
- Reproducible calculation logs

---

### 🌐 Visualization & UX
- Interactive CO₂e charts
- Transport comparison graphs
- Emissions trend dashboards
- Goal tracking visualization
- Mobile responsive design support

---

### ⚙️ System Architecture
- Python backend (FastAPI recommended)
- React frontend dashboard
- SQLite for development
- PostgreSQL for production scaling
- Docker support for deployment
- Environment-based configuration system

---

### 🔓 Open Source Governance
- AGPL-3.0+ licensing
- Contributor guidelines (CONTRIBUTING.md)
- Issue templates (bugs, features, emissions data)
- Code of conduct
- Transparent roadmap
- CHANGELOG support

---

### 🌍 Future Vision Features
- Carbon-aware routing engine
- Real-time emissions estimation during booking
- Global emissions heatmap visualization
- Personal carbon assistant (rule-based system)
- Organizational carbon drift detection system

---

## 🛠 How to Build

### 1. Clone Repository
Clone GreenMile from GitLab:
git clone https://gitlab.com/Roxanne_Ardary/greenmile

### 2. Backend Setup
Install Python dependencies and run FastAPI server in development mode.

### 3. Frontend Setup
Install Node dependencies and start React dashboard.

### 4. Run System
Start backend API and frontend UI locally.

### 5. Extend System
Add:
- New transport modes
- New emission factors
- New dashboards
- New API integrations

---

## 📦 Tech Stack
- Python (FastAPI)
- React
- Chart.js
- SQLite / PostgreSQL
- Docker (optional)

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
  - [https://roxanneardary.com/greenmile/](https://roxanneardary.com/greenmile/)

---

## 📄 License & Notice Requirements

GreenMile is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- GreenMile specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
