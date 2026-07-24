# GapVision

**Tagline:** *Open Data. Open Equity.*

**Website:** [https://roxanneardary.com](https://roxanneardary.com)  
**GitLab Repository:** [https://gitlab.com/Roxanne_Ardary/gapvision](https://gitlab.com/Roxanne_Ardary/gapvision)  

---

## **Project Overview**

GapVision is an **open-source platform** designed to track, analyze, and visualize compensation data across industries with a focus on **gender pay equity**.  

The platform empowers:  
- **Employees** — to understand their worth and advocate confidently  
- **Companies** — to benchmark and improve pay equity  
- **Policymakers & NGOs** — to access transparent, actionable data  

GapVision leverages **data, AI, and community contributions** to highlight pay gaps, predict trends, and provide actionable solutions.  

---

## **Features**

### **1. Compensation & Pay Data**
- Base salary, bonuses, stock options, retirement contributions  
- Gender breakdown: men, women, non-binary/other  
- Intersectional data: age, experience, education, seniority, ethnicity, disability status  
- Part-time, full-time, gig/contract roles  
- Benefits & perks equity (parental leave, training, flexible work)  

### **2. Equity & Gap Analysis**
- Auto-calculation of **gender pay gaps**  
- Automatic **flagging** of roles/sectors exceeding thresholds  
- Historical trends & predictive forecasts  
- Industry and company leaderboards  

### **3. Company Metrics**
- Average pay gap per company  
- % women in leadership  
- Compliance flags with pay equity regulations  
- **Pay Equity Seal** for top-performing companies  

### **4. Career Mobility & Negotiation**
- Promotions, lateral moves, career progression  
- Bottleneck detection for gender disparities  
- Tracking of negotiation frequency and success by gender  

### **5. Skills, AI, & Automation Insights**
- Emerging skills and pay impact by gender  
- AI and automation risk scoring for roles  
- Predictive modeling of future pay gaps  

### **6. Community & Crowdsourcing**
- Anonymous salary submissions  
- Verified contributions  
- Gamification: points, badges, leaderboards  
- Mentorship programs for underrepresented employees  

### **7. Dashboards & Visualization**
- Interactive dashboards by industry, role, company, gender, skills, and location  
- Historical trends, predictive charts, and heatmaps  
- Exportable reports (CSV, JSON, PDF)  

### **8. Policy & Advocacy Tools**
- Generate anonymized reports for NGOs, media, and policymakers  
- Simulate impact of policies on pay gaps  
- Provide recommendations for interventions at role, company, or sector level  

---

## **Getting Started**

### **1. Installation**
```bash
# Clone the repository
git clone https://gitlab.com/Roxanne_Ardary/GapVision.git

# Navigate to project directory
cd GapVision

# Install backend dependencies
pip install -r requirements.txt

# Install frontend dependencies (if using React/Vue)
npm install
```

Running the Platform
```bash
# Start backend API
python app.py

# Start frontend dashboard
npm start
```

## **Database Schema**
GapVision includes tables for:  
- `jobs`, `salary_data`, `pay_gap_flags`  
- `company_metrics`, `career_mobility`  
- `automation_impact`, `negotiation_data`, `community_contributions`  

Refer to `/docs/schema.md` for full ERD and field descriptions.

---

## **API Endpoints (Examples)**
- `GET /jobs?industry=finance&location=SG` → List jobs with pay data  
- `GET /jobs/{job_id}` → Detailed pay breakdown  
- `GET /industries/top-gaps` → Top industries by pay gap  
- `POST /contribute/salary` → Submit verified salary data  
- `GET /dashboard` → Interactive visualization  

---

## **Contributing**
See [`CONTRIBUTING.md`](CONTRIBUTING.md) for guidelines on:  
- Code contributions  
- Data submission & verification  
- Reporting issues and feature requests  

All contributions are licensed under **AGPL 3.0+ with attribution**.

---

## Specification Branding License (SBL):  
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

Optional:
- Specification Branding License (SBL)
  - attribution-free commercial deployment
  - pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/gapvision/](https://roxanneardary.com/gapvision/)

---

## License & Notice Requirements

GapVision is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- GapVision specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## **Acknowledgements**
GapVision builds on open-source contributions and publicly available datasets.  
Special thanks to contributors and the community working towards **gender pay equity worldwide**.
