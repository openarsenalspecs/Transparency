# PayInsight Specification

**Smart Insights for Fair Compensation**

## Overview

PayInsight is an open-source, privacy-first employment platform designed to create a transparent, secure, and intelligent marketplace for employers and job seekers across the United States.

The platform provides comprehensive job discovery across industries and occupations while requiring employers to disclose compensation and time commitments before candidates apply. PayInsight combines transparent employment information with AI-assisted cost-of-living analysis, compensation guidance, skill assessment, career development, secure communication, and privacy-preserving hiring workflows.

PayInsight is designed as a modular platform. Core employment, privacy, search, compensation, assessment, communication, and AI capabilities form the foundation of the system. Optional plugin modules extend the platform with additional services, integrations, datasets, AI models, learning providers, analytics systems, and specialized employment functionality.

## Design Principles

- Open-source development and community participation
- Privacy by design
- End-to-end encryption for sensitive personal communications and information
- Data minimization
- Employer compensation transparency
- Candidate control over personal information
- Human oversight of consequential AI decisions
- Explainable AI recommendations
- Accessibility and inclusive design
- Vendor independence
- Interoperable data standards
- Modular architecture
- Self-hosting capability
- No mandatory dependence on proprietary services
- Transparent employment practices
- Fair compensation awareness
- Candidate and employer autonomy

## Core Modules

### Identity and Privacy Module

The Identity and Privacy Module manages secure accounts, identity protection, authentication, authorization, consent, and privacy controls.

Capabilities include:

- Privacy-preserving account creation
- Optional pseudonymous candidate profiles
- Identity separation between public profiles and protected personal information
- Granular consent controls
- Selective disclosure of personal information
- End-to-end encryption for sensitive information
- Encryption at rest
- Secure key management
- Data minimization
- Data export and deletion controls
- Privacy preferences
- Access auditing
- Session management
- Multi-factor authentication
- Role-based permissions
- Candidate-controlled identity disclosure

### Employer Module

The Employer Module provides employers with tools for creating verified organizational profiles and publishing employment opportunities.

Employer profiles may include:

- Organization name
- Industry
- Organization description
- Location
- Company size
- Website
- Verification status
- Workplace policies
- Benefits
- Compensation practices
- Employment types

The module shall support employer verification without requiring unnecessary disclosure of private information.

### Job Posting Module

The Job Posting Module manages the creation, validation, publication, modification, expiration, and archival of employment opportunities.

Every published job must provide explicit information about:

- Position title
- Employer
- Employment type
- Location
- Remote, hybrid, or on-site status
- Salary or hourly compensation
- Compensation range where applicable
- Expected hours
- Expected schedule
- Time commitment
- Overtime expectations where applicable
- Contract duration where applicable
- Required skills
- Preferred skills
- Required experience
- Education requirements where applicable
- Benefits
- Paid time off
- Bonuses
- Equity or stock compensation where applicable
- Travel requirements
- Physical requirements where applicable
- Application requirements

The system shall identify incomplete, ambiguous, contradictory, or potentially misleading job postings before publication.

### Job Search and Discovery Module

The Job Search and Discovery Module enables users to search employment opportunities across industries, occupations, employers, locations, and employment types throughout the United States.

Search capabilities include:

- Keyword search
- Occupation search
- Industry search
- Skill search
- Employer search
- Location search
- Salary filtering
- Hourly compensation filtering
- Cost-of-living adjusted compensation filtering
- Employment type filtering
- Remote work filtering
- Hybrid work filtering
- On-site work filtering
- Schedule filtering
- Benefits filtering
- Experience filtering
- Education filtering
- Time commitment filtering
- Contract duration filtering
- Accessibility requirement filtering

Search results shall provide transparent information sufficient for candidates to evaluate an opportunity before applying.

### Compensation Transparency Module

The Compensation Transparency Module standardizes and analyzes employer compensation information.

Capabilities include:

- Salary comparison
- Hourly wage comparison
- Total compensation calculation
- Benefits valuation
- PTO valuation
- Bonus analysis
- Equity compensation representation
- Overtime analysis
- Effective hourly compensation calculation
- Compensation range analysis
- Market compensation comparison
- Compensation history where available
- Compensation trend analysis
- Employer compensation transparency scoring

The module shall clearly distinguish employer-provided compensation from AI-generated estimates.

### Cost of Living Module

The Cost of Living Module helps job seekers determine whether advertised compensation is likely to support the cost of living associated with a job location.

The module may evaluate:

- Housing
- Utilities
- Food
- Transportation
- Healthcare
- Taxes
- Insurance
- Childcare
- Other essential expenses
- Regional price differences
- Local wage conditions

The system shall present assumptions, source data, calculation methodology, and uncertainty where applicable.

Users may specify personal budgeting assumptions without exposing those details to employers.

### AI Compensation Advisor Module

The AI Compensation Advisor assists candidates in evaluating compensation and preparing for negotiations.

Capabilities include:

- Compensation adequacy analysis
- Cost-of-living adjusted compensation analysis
- Market compensation comparisons
- Salary negotiation preparation
- Hourly rate negotiation
- Counter-offer suggestions
- Negotiation scripts
- Total compensation comparisons
- Benefits valuation
- Opportunity cost analysis
- Compensation scenario modeling

AI recommendations shall be presented as guidance rather than guaranteed financial outcomes.

### Skill Assessment Module

The Skill Assessment Module evaluates whether a candidate's demonstrated abilities align with the requirements of a position.

Capabilities include:

- Job-specific assessments
- Skill testing
- Knowledge testing
- Practical exercises
- Scenario-based testing
- Adaptive assessments
- Candidate self-assessment
- AI-generated assessment questions
- Skill gap identification
- Assessment scoring
- Assessment explanations
- Candidate preparation recommendations
- Employer-defined assessment criteria

Assessments should measure relevant skills rather than unnecessary personal characteristics.

Candidates shall be able to review their own assessment results and identify areas for improvement.

### AI Job Matching Module

The AI Job Matching Module recommends employment opportunities based on candidate-defined preferences and relevant qualifications.

Matching factors may include:

- Skills
- Experience
- Education
- Compensation requirements
- Cost-of-living requirements
- Location
- Remote preferences
- Schedule preferences
- Employment type
- Career objectives
- Required qualifications
- Demonstrated assessment results

Matching systems shall provide understandable explanations for recommendations and shall not make irreversible employment decisions without appropriate human oversight.

### Career Development Module

The Career Development Module helps users plan and improve their careers.

Capabilities include:

- Career path exploration
- Skill gap analysis
- Personalized development plans
- Learning recommendations
- Career trajectory modeling
- Salary trajectory analysis
- Industry demand analysis
- Occupation demand analysis
- Transferable skill identification
- Resume improvement guidance
- Interview preparation
- Professional development tracking

### Candidate Profile Module

The Candidate Profile Module allows users to maintain a private professional profile while controlling what employers can see.

Profiles may include:

- Skills
- Experience
- Education
- Certifications
- Portfolio information
- Work preferences
- Compensation expectations
- Availability
- Career objectives
- Assessment results
- Verified credentials

Sensitive identity information shall remain separated from publicly searchable professional information unless the candidate explicitly chooses to disclose it.

### Application Module

The Application Module manages the candidate application lifecycle.

Capabilities include:

- Saved jobs
- Applications
- Application status
- Candidate-controlled disclosures
- Employer requests for additional information
- Application history
- Application documents
- Application notifications
- Withdrawal controls
- Interview invitations
- Offer management

Candidates shall retain control over whether and when protected personal information is disclosed.

### Employer Hiring Module

The Employer Hiring Module provides tools for managing candidate pipelines.

Capabilities include:

- Applicant management
- Candidate search
- Skill matching
- Assessment review
- Interview management
- Candidate communications
- Application stages
- Hiring workflows
- Interview scheduling
- Offer management
- Hiring analytics

Candidate privacy controls shall remain enforced throughout the hiring process.

### Secure Messaging Module

The Secure Messaging Module provides encrypted communication between candidates and employers.

Capabilities include:

- End-to-end encrypted messages
- Candidate-controlled communication
- Attachments
- Interview invitations
- Application notifications
- Message history
- Message deletion
- Delivery status
- Security notifications

### Video Interview Module

The Video Interview Module provides an open-source alternative to proprietary video meeting services for employment interviews.

Capabilities include:

- One-on-one video interviews
- WebRTC-based communication
- Encrypted communications
- Audio and video controls
- Screen sharing
- Text chat
- Interview scheduling
- Waiting rooms
- Session controls
- Optional recording
- Recording consent controls
- Accessibility features

The module shall be designed to integrate with open-source conferencing infrastructure and shall not require a proprietary video conferencing provider.

### Interview Scheduling Module

The Interview Scheduling Module coordinates interviews between candidates and employers.

Capabilities include:

- Availability management
- Time zone handling
- Interview invitations
- Calendar integration
- Automatic reminders
- Rescheduling
- Cancellation
- Interview duration
- Interview type
- Secure interview links

### Employer Reputation Module

The Employer Reputation Module provides transparent information about employer practices.

Capabilities may include:

- Candidate feedback
- Employee feedback
- Anonymous reviews
- Compensation transparency indicators
- Posting completeness indicators
- Hiring process feedback
- Workplace practice indicators
- Employer verification
- Reputation history

The system shall include safeguards against fraudulent reviews, retaliation, harassment, manipulation, and coordinated abuse.

### Market Intelligence Module

The Market Intelligence Module provides aggregated employment information.

Capabilities include:

- Salary trends
- Hourly wage trends
- Occupation demand
- Industry demand
- Geographic employment trends
- Skill demand
- Compensation trends
- Cost-of-living comparisons
- Remote work trends
- Career opportunity analysis

Personal information shall not be exposed through aggregate analytics.

### Community Module

The Community Module supports optional professional interaction among users.

Capabilities may include:

- Mentorship
- Career discussions
- Professional communities
- Skill discussions
- Industry discussions
- Career advice
- Knowledge sharing
- Moderation
- Reporting
- Privacy controls

### Notification Module

The Notification Module manages user alerts and communication preferences.

Notifications may include:

- New matching jobs
- Application updates
- Interview invitations
- Interview reminders
- Employer messages
- Assessment requests
- Compensation changes
- Saved search alerts
- Career recommendations

Users shall control notification frequency and delivery methods.

### Accessibility Module

The Accessibility Module ensures that the platform can be used by people with diverse abilities.

Capabilities include:

- Keyboard navigation
- Screen reader support
- High contrast support
- Adjustable text
- Captions
- Transcripts
- Accessible forms
- Accessible assessments
- Accessible video interviews
- Reduced motion options
- Alternative interaction methods

### Trust and Safety Module

The Trust and Safety Module protects users and the employment marketplace.

Capabilities include:

- Employer verification
- Fraud detection
- Scam detection
- Suspicious posting detection
- Abuse reporting
- Account security
- Automated moderation
- Human review
- Rate limiting
- Anti-spam protections
- Audit logging
- Security alerts

### Analytics Module

The Analytics Module provides privacy-preserving operational and employment analytics.

Capabilities include:

- Job posting analytics
- Application analytics
- Hiring funnel analytics
- Search analytics
- Compensation analytics
- Platform performance analytics
- Candidate engagement analytics
- Employer engagement analytics

Analytics shall use data minimization and aggregation techniques where appropriate.

## Optional Plugin Modules

### Learning Provider Plugin

Connects PayInsight to external or self-hosted education and training providers.

Capabilities may include:

- Course discovery
- Skill-to-course matching
- Learning recommendations
- Credential import
- Progress synchronization

### Credential Verification Plugin

Provides verification of certifications, licenses, education, training, and professional credentials.

### Labor Market Data Plugin

Imports external labor market datasets for compensation, occupation demand, employment trends, and geographic analysis.

### Cost of Living Data Plugin

Connects additional regional cost-of-living datasets to improve compensation analysis.

### Calendar Integration Plugin

Connects external calendar providers for interview scheduling and availability management.

### Open Video Provider Plugin

Allows administrators to connect alternative open-source WebRTC or conferencing infrastructure.

### AI Model Plugin

Allows administrators to select, host, replace, or combine AI models for matching, assessment, analysis, and career assistance.

### Local AI Plugin

Provides support for locally hosted AI models to reduce dependence on external AI providers and improve data privacy.

### Resume and Portfolio Plugin

Provides tools for importing, creating, analyzing, and managing resumes and professional portfolios.

### Skills Taxonomy Plugin

Provides configurable occupation, skill, competency, and industry taxonomies.

### Employer Verification Plugin

Connects external verification services or self-hosted verification systems for confirming employer identity.

### Background Verification Plugin

Provides optional integrations for legally compliant background verification services while maintaining candidate consent and privacy controls.

### Payroll and Compensation Plugin

Provides optional integration with payroll or compensation systems for organizations that choose to use them.

### Tax Estimation Plugin

Provides optional tax estimation capabilities for comparing gross and estimated net compensation across locations.

### Benefits Comparison Plugin

Standardizes and compares employer benefits packages.

### Commute Analysis Plugin

Analyzes commuting distance, time, transportation costs, and related expenses for on-site and hybrid positions.

### Housing Analysis Plugin

Provides optional housing market data for more detailed cost-of-living analysis.

### Mentorship Plugin

Connects candidates with volunteer, professional, or employer-sponsored mentors.

### Community Moderation Plugin

Provides additional moderation models, rules, reporting workflows, and community safety tools.

### Localization Plugin

Provides support for additional countries, currencies, languages, employment systems, and labor regulations while preserving the core architecture.

### Mobile Application Plugin

Provides native or cross-platform mobile clients.

### Data Export Plugin

Provides structured exports using interoperable formats for candidates, employers, administrators, and authorized third parties.

### Federation Plugin

Allows independently operated PayInsight instances to exchange compatible public employment information without requiring a centralized platform.

## AI Governance

AI systems within PayInsight shall operate as assistive systems rather than unquestionable decision makers.

The platform shall support:

- Explainable recommendations
- Human review
- Model transparency
- Model version tracking
- Assessment transparency
- Bias monitoring
- Performance monitoring
- Error reporting
- User correction
- User appeal
- Data provenance
- AI-generated content labeling
- Configurable AI providers
- Local model support

AI shall not be permitted to make consequential employment decisions solely on the basis of protected characteristics or inferred sensitive information.

## Data Governance

PayInsight shall establish clear distinctions between:

- Public job information
- Employer information
- Candidate professional information
- Protected identity information
- Private communications
- Assessment information
- Analytics data
- AI-generated information
- External data sources

Users shall have meaningful control over their information.

The platform shall support:

- Data minimization
- Purpose limitation
- Consent management
- Data portability
- Data deletion
- Access controls
- Encryption
- Auditability
- Retention policies
- Source attribution
- Data provenance

## Security Requirements

Security shall be treated as a core platform capability.

The platform should support:

- End-to-end encryption where technically applicable
- Encryption at rest
- Encryption in transit
- Secure authentication
- Multi-factor authentication
- Secure session management
- Key management
- Access control
- Audit logging
- Security monitoring
- Dependency auditing
- Vulnerability management
- Secure software development practices
- Regular security review

Security-sensitive features shall be designed to minimize the amount of information accessible to platform operators.

## Employer Transparency Requirements

A job posting shall not be considered complete until the required compensation and time commitment information has been supplied.

The platform shall distinguish between:

- Guaranteed compensation
- Conditional compensation
- Estimated compensation
- Bonuses
- Commission
- Equity
- Benefits
- Reimbursements
- Overtime
- Unpaid time expectations
- Required availability

Employers shall not be permitted to disguise required labor as optional availability or omit material compensation information.

## Candidate Empowerment

PayInsight shall give candidates tools to evaluate an opportunity before committing personal information.

Candidates should be able to answer questions such as:

- What does this job actually pay?
- How many hours am I expected to work?
- What is the effective hourly compensation?
- What will this compensation support in the job's location?
- How does this offer compare with similar jobs?
- What skills do I have?
- What skills am I missing?
- What should I negotiate?
- What benefits are actually valuable?
- What career opportunities could this position create?

## Employer Empowerment

PayInsight shall also help employers create better and more transparent hiring processes.

Employer tools should help answer:

- Is the compensation competitive?
- Are the job requirements clear?
- Are the expected hours accurately represented?
- Which skills are actually necessary?
- Where is the candidate pool located?
- Which candidates demonstrate the required skills?
- Where are candidates falling out of the hiring process?
- How can the hiring process become more efficient and equitable?

## Interoperability

The platform shall favor open standards and interoperable interfaces.

Where practical, PayInsight should provide:

- Documented APIs
- Structured data formats
- Import and export capabilities
- Plugin interfaces
- Authentication interfaces
- AI provider interfaces
- Search interfaces
- Assessment interfaces
- Video conferencing interfaces
- Calendar interfaces
- Data federation interfaces

No core feature should require permanent dependence on a single vendor.

## Deployment

PayInsight shall support self-hosted deployments and may support hosted deployments.

Deployment configurations should allow organizations to select:

- Database providers
- Search providers
- AI providers
- Video infrastructure
- Storage providers
- Authentication systems
- Cost-of-living datasets
- Labor market datasets
- Monitoring systems

## Testing and Quality

The platform shall include testing for:

- Core functionality
- Security
- Privacy
- Encryption
- Search
- Compensation calculations
- Cost-of-living calculations
- AI recommendations
- Skill assessments
- Accessibility
- API compatibility
- Plugin compatibility
- Data migration
- Performance
- Failure recovery

AI systems shall be evaluated for accuracy, consistency, bias, and inappropriate recommendations before production deployment.

## Open-Source Extensibility

PayInsight is designed to support community-developed extensions without requiring changes to the core platform.

Plugins may provide:

- New AI models
- New datasets
- New assessment systems
- New employment taxonomies
- New integrations
- New analytics
- New communication systems
- New learning providers
- New credential systems
- New geographic markets
- New accessibility capabilities

Core functionality shall remain usable without optional proprietary plugins.

## Future Expansion

The initial implementation is focused on employment within the United States. The architecture shall support future expansion into additional regions without requiring a redesign of the core platform.

Future localization may address:

- Languages
- Currencies
- Labor regulations
- Employment classifications
- Tax systems
- Benefits systems
- Compensation conventions
- Regional cost-of-living data
- Regional occupation taxonomies

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
  - [https://roxanneardary.com/payinsight/](https://roxanneardary.com/payinsight/)

---

## License & Notice Requirements

PayInsight is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- PayInsight specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
