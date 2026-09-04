# Vetora
**Early Insight for Better Outcomes.**
- HTML Mirror:  [https://roxanneardary.com/vetora-specification/](https://roxanneardary.com/vetora-specification/)  

---

Vetora is an open-source AI veterinary health intelligence platform designed to help pet owners organize, understand, and monitor their animals' health information. Vetora combines veterinary record keeping, symptom analysis, risk assessment, medication intelligence, side-effect comparison, and veterinary care support within a modular system.

## Purpose

Vetora provides a centralized health intelligence layer for animal care. The system is designed to transform veterinary records and ongoing health observations into structured, understandable information that can help users recognize changes, identify potential concerns, prepare for veterinary visits, and make more informed decisions about animal health.

Vetora does not replace a veterinarian or independently diagnose, prescribe, change medication dosages, or discontinue prescribed treatment. Its purpose is to provide information, identify possible explanations, assess potential risks, and encourage appropriate veterinary involvement when circumstances warrant professional care.

## Design Principles

- Open-source and modular design
- Veterinary-first decision support
- Local-first and privacy-conscious operation
- Human oversight for health decisions
- Evidence-based information
- Transparent recommendations
- Explainable risk assessment
- Medication safety and comparison
- Data portability and user control
- Vendor independence
- Extensible plugin architecture
- Auditable AI-assisted analysis
- Clear distinction between verified information and AI-generated interpretation

---

## Core Modules

### Animal Profile Module

The Animal Profile Module maintains the foundational identity and health context for each animal.

Features include:

- Species
- Breed
- Age and date of birth
- Sex and reproductive status
- Weight history
- Allergies
- Known conditions
- Previous surgeries and procedures
- Vaccination history
- Veterinary information
- Emergency contacts
- Dietary information
- Behavioral observations
- Relevant genetic or hereditary information
- Individual health preferences and care requirements

The module provides contextual information to other Vetora modules so that analysis can account for the individual animal rather than relying solely on generalized information.

### Veterinary Record Module

The Veterinary Record Module maintains a structured longitudinal record of veterinary care.

Features include:

- Veterinary visits
- Diagnoses and suspected conditions
- Laboratory results
- Imaging records
- Procedures
- Surgeries
- Vaccinations
- Prescriptions
- Treatment plans
- Clinical notes
- Discharge instructions
- Referral records
- Hospitalization records
- Specialist consultations
- Historical medical events

Records should preserve original information while allowing structured data to be extracted for analysis.

### Document Intelligence Module

The Document Intelligence Module converts veterinary documents into structured information.

Features include:

- Veterinary report processing
- Laboratory report extraction
- Prescription extraction
- Discharge instruction extraction
- Medical history extraction
- Date and event recognition
- Medication recognition
- Dosage and frequency recognition
- Abnormal result identification
- Source preservation
- Confidence scoring
- Human verification

Extracted information must remain distinguishable from information entered or verified directly by the user.

### Symptom Journal Module

The Symptom Journal Module allows users to continuously document changes in an animal's health.

Features include:

- Symptom entry
- Symptom severity
- Duration
- Frequency
- Onset
- Progression
- Associated symptoms
- Appetite changes
- Drinking changes
- Urination changes
- Defecation changes
- Vomiting
- Mobility changes
- Behavior changes
- Respiratory observations
- Pain observations
- Weight changes
- User notes
- Photographic and document attachments
- Historical symptom comparison

The module creates a timeline that can be evaluated alongside veterinary records and medication history.

### AI Veterinary Assistant Module

The AI Veterinary Assistant Module provides conversational assistance for understanding animal health information.

Features include:

- Health record questions
- Symptom questions
- Medical history questions
- Medication questions
- Veterinary visit preparation
- Questions to discuss with a veterinarian
- Explanation of medical terminology
- Identification of potentially relevant health information
- Summarization of veterinary records
- Identification of changes over time
- Context-aware responses based on available animal records

The assistant must clearly communicate uncertainty and must not represent speculation as a confirmed diagnosis.

### Differential Reasoning Module

The Differential Reasoning Module identifies possible explanations for symptoms and health changes.

Features include:

- Possible causes
- Differential condition generation
- Symptom relationship analysis
- Historical context analysis
- Medication-related considerations
- Age and species considerations
- Relevant risk factors
- Supporting observations
- Contradicting observations
- Missing information
- Recommended questions
- Veterinary discussion prompts

Possible causes must be presented as considerations rather than definitive diagnoses.

### Risk Scoring Module

The Risk Scoring Module evaluates the potential urgency of reported symptoms and health changes.

The system should support a transparent risk scale such as:

- Level 0: Routine
- Level 1: Low concern
- Level 2: Veterinary evaluation recommended
- Level 3: Prompt veterinary evaluation
- Level 4: Urgent veterinary attention
- Level 5: Emergency veterinary attention

Risk assessments should consider:

- Symptom severity
- Symptom combination
- Duration
- Progression
- Animal age
- Species
- Existing conditions
- Medication history
- Recent procedures
- Laboratory abnormalities
- Behavioral changes
- Hydration indicators
- Breathing concerns
- Pain indicators
- Neurological changes
- Other recognized warning signs

The system must explain the factors contributing to each risk score.

### Emergency Alert Module

The Emergency Alert Module identifies circumstances that may require immediate veterinary attention.

Features include:

- Red-flag symptom detection
- Emergency risk overrides
- Immediate veterinary care recommendations
- Emergency hospital guidance
- User confirmation prompts
- Escalation messaging
- Emergency contact access

Critical red flags must be capable of overriding a lower calculated score when appropriate.

### Veterinary Escalation Module

The Veterinary Escalation Module translates risk assessments into recommended levels of professional care.

Features include:

- Routine veterinary appointment recommendation
- Prompt appointment recommendation
- Same-day veterinary recommendation
- Urgent care recommendation
- Emergency care recommendation
- Specialist referral prompts
- Veterinary question generation
- Appointment preparation

The system should favor appropriate professional evaluation when available information indicates meaningful risk.

### Medication Record Module

The Medication Record Module maintains a complete history of medications used by an animal.

Features include:

- Brand name
- Generic name
- Active ingredients
- Manufacturer
- Strength
- Form
- Dosage
- Administration frequency
- Treatment duration
- Prescribing veterinarian
- Start date
- End date
- Reason for treatment
- Current status
- Previous medications
- Medication reactions
- Treatment outcomes

### Medication Intelligence Module

The Medication Intelligence Module provides structured information about veterinary medications.

Features include:

- Brand-name lookup
- Active ingredient identification
- Medication purpose
- Species information
- Approved uses
- Warnings
- Contraindications
- Known interactions
- Administration information
- Available formulations
- Manufacturer information
- Regulatory information
- Evidence sources

### Generic and Alternative Medication Module

The Generic and Alternative Medication Module identifies potentially lower-cost medication options while clearly distinguishing different types of alternatives.

Categories include:

- Approved generic equivalent
- Same active ingredient
- Same therapeutic class
- Therapeutic alternative
- Combination alternative
- Non-equivalent alternative

The system must never present a non-equivalent medication as a generic equivalent.

Medication substitutions must be presented as information for discussion with a veterinarian rather than as autonomous prescribing decisions.

### Medication Side Effect Comparison Module

The Medication Side Effect Comparison Module compares the adverse-effect profiles of medically appropriate medication options.

Features include:

- Side-effect identification
- Side-effect frequency comparison
- Side-effect severity comparison
- Serious adverse-event identification
- Reversibility assessment
- Expected duration
- Species-specific considerations
- Age-related considerations
- Existing-condition considerations
- Interaction considerations
- Contraindication analysis
- Regulatory warnings
- Evidence quality
- Post-market safety information
- Patient-specific risk factors

Side effects should use a consistent severity scale such as:

- Level 0: Minimal
- Level 1: Mild
- Level 2: Moderate
- Level 3: Significant
- Level 4: Severe
- Level 5: Critical

The system should prioritize the medication with the most favorable safety-adjusted profile among medically appropriate options rather than automatically selecting the medication with the lowest price or the fewest reported side effects in isolation.

### Medication Safety Scoring Module

The Medication Safety Scoring Module calculates a safety-adjusted assessment for each medically appropriate medication option.

Factors may include:

- Known adverse effects
- Adverse-effect severity
- Adverse-effect frequency
- Patient-specific risk
- Existing medical conditions
- Current medications
- Drug interactions
- Contraindications
- Age
- Species
- Weight
- Evidence quality
- Treatment relevance
- Regulatory warnings
- Historical patient reactions

The system should separately expose safety, effectiveness relevance, price, and evidence rather than combining them into an opaque single recommendation.

### Patient Adverse Reaction Module

The Patient Adverse Reaction Module maintains a permanent history of medication-related reactions.

Features include:

- Previous adverse reactions
- Suspected medication
- Active ingredient
- Reaction description
- Severity
- Date
- Resolution
- Veterinary confirmation
- Related medications
- Cross-medication warnings

Previous serious reactions should automatically influence future medication safety assessments.

### Veterinary Medication Price Search Module

The Veterinary Medication Price Search Module searches available sources for medication pricing.

Features include:

- Brand-name searches
- Generic searches
- Retailer comparison
- Pharmacy comparison
- Manufacturer comparison
- Prescription requirement identification
- Availability
- Quantity
- Strength
- Formulation
- Shipping cost
- Coupons
- Membership pricing
- Autoship pricing
- Promotional pricing
- Estimated treatment cost

Prices should be normalized so users can compare the actual cost of equivalent quantities, doses, treatment periods, or monthly use.

### Price Intelligence Engine

The Price Intelligence Engine analyzes medication prices across available sources.

Features include:

- Price normalization
- Cost per dose
- Cost per treatment period
- Monthly cost
- Generic versus brand comparison
- Coupon analysis
- Subscription price comparison
- Shipping analysis
- Price history
- Lowest verified price
- Price-change detection
- Availability monitoring

The system should distinguish advertised prices from final estimated purchase costs.

### Price Alert Module

The Price Alert Module allows users to monitor medication costs.

Features include:

- Price-drop alerts
- Generic availability alerts
- Coupon alerts
- Promotional pricing alerts
- Availability alerts
- Prescription requirement changes
- Preferred retailer alerts

### Drug Interaction Module

The Drug Interaction Module evaluates potential interactions between medications and other known treatments.

Features include:

- Medication-to-medication interactions
- Medication-to-condition considerations
- Duplicate active ingredients
- Therapeutic duplication
- Contraindication warnings
- Severity classification
- Evidence source tracking
- Veterinary review prompts

### Evidence and Source Module

The Evidence and Source Module maintains source information supporting health and medication analysis.

Features include:

- Source attribution
- Regulatory information
- Veterinary references
- Published evidence
- Evidence dates
- Evidence quality
- Source type
- Source relevance
- Conflicting evidence identification
- Source history

Users should be able to determine where important health or medication information originated.

### Knowledge Confidence Module

The Knowledge Confidence Module identifies the certainty of information used by Vetora.

Confidence levels may include:

- Very High
- High
- Moderate
- Low
- Insufficient

The module should distinguish between:

- Verified veterinary records
- User-entered information
- AI-extracted information
- Evidence-supported information
- AI-generated interpretation
- Unconfirmed possibilities

The system should identify important missing information that could materially affect an assessment.

### Human-in-the-Loop Module

The Human-in-the-Loop Module ensures that important health decisions remain subject to human and veterinary judgment.

Features include:

- User confirmation
- Record verification
- Recommendation review
- Uncertainty disclosure
- Veterinary review prompts
- Correction workflows
- Rejection of inaccurate extracted information
- Manual overrides
- Decision history

### Veterinary Visit Preparation Module

The Veterinary Visit Preparation Module helps users prepare useful information for veterinary appointments.

Features include:

- Health history summaries
- Current medication lists
- Symptom timelines
- Risk summaries
- Recent changes
- Laboratory summaries
- Questions for the veterinarian
- Possible causes to discuss
- Medication questions
- Side-effect concerns
- Printable or shareable visit summaries

### Longitudinal Health Intelligence Module

The Longitudinal Health Intelligence Module evaluates health information across time.

Features include:

- Trend detection
- Weight trends
- Symptom recurrence
- Medication response
- Laboratory trends
- Condition progression
- Treatment history
- Behavioral changes
- Emerging patterns
- Significant historical events

The system should distinguish meaningful trends from isolated observations.

### Preventive Care Module

The Preventive Care Module supports ongoing animal health management.

Features include:

- Vaccination reminders
- Preventive medication reminders
- Veterinary visit reminders
- Routine screening reminders
- Weight monitoring
- Dental care reminders
- Preventive health schedules
- Age-related care recommendations

Recommendations should account for the individual animal and should not be presented as universally applicable medical requirements.

### Privacy and Security Module

The Privacy and Security Module protects animal health information and associated user data.

Features include:

- Local data control
- Data minimization
- Access controls
- Encryption support
- Export and deletion capabilities
- Consent management
- Sharing controls
- Audit history
- Data portability
- Separation of personal information from health analysis where practical

### AI Audit Module

The AI Audit Module records important AI-assisted activity.

Features include:

- Input context
- Information sources
- Model identification
- Analysis timestamp
- Risk factors
- Confidence level
- Recommendation
- Escalation decision
- Source references
- User corrections
- Human review
- Final outcome when available

Audit records should make it possible to understand how an AI-assisted recommendation was generated.

---

## Optional Plugin Modules

### Veterinary Clinic Integration Plugin

Connects Vetora with participating veterinary clinics for record exchange, appointment information, and care coordination.

### Electronic Veterinary Records Plugin

Provides interoperability with supported electronic veterinary record systems.

### Veterinary Pharmacy Plugin

Connects Vetora with veterinary pharmacies for medication availability, pricing, prescription fulfillment, and product information.

### Retailer Integration Plugin

Connects to supported medication retailers and provides current pricing, availability, coupons, and purchasing information.

### Laboratory Integration Plugin

Imports laboratory results and supports longitudinal laboratory monitoring.

### Imaging Integration Plugin

Imports veterinary imaging records and optionally supports analysis tools provided by compatible services.

### Wearable Integration Plugin

Imports health and activity information from supported animal wearables.

### Smart Collar Plugin

Connects supported smart collars and monitoring devices to provide activity, location, behavioral, and other available measurements.

### Home Diagnostic Device Plugin

Connects supported home animal-health diagnostic devices and imports their results into the veterinary record.

### Pet Insurance Plugin

Organizes insurance information and optionally assists with claim preparation and coverage documentation.

### Veterinary Specialist Plugin

Supports information sharing and collaboration with veterinary specialists.

### Emergency Hospital Plugin

Provides integration with participating emergency veterinary hospitals and supports emergency escalation workflows.

### Voice Assistant Plugin

Allows users to record symptoms, ask questions, and interact with Vetora using voice input.

### Mobile Application Plugin

Provides mobile access to records, symptom logging, alerts, medication information, and veterinary visit preparation.

### Multi-Veterinarian Collaboration Plugin

Allows multiple veterinary professionals to participate in an animal's care record where authorized by the user.

### Household Sharing Plugin

Allows authorized household members to share access to selected animal records and care responsibilities.

### Pet Food Intelligence Plugin

Provides structured information about pet food products and allows users to compare ingredients, nutritional information, and dietary considerations.

### Nutrition Analysis Plugin

Analyzes recorded diets and nutritional information in conjunction with the animal's health profile.

### Breed Knowledge Plugin

Adds breed-specific health information and considerations where reliable evidence is available.

### Genetic Information Plugin

Allows authorized genetic and hereditary information to be incorporated into health assessments.

### Shelter and Rescue Records Plugin

Supports import and management of historical records from shelters, rescues, breeders, and other authorized organizations.

---

## Safety Requirements

Vetora shall not represent AI-generated information as a confirmed veterinary diagnosis.

Vetora shall not independently prescribe medication, change a prescribed dosage, recommend discontinuation of prescribed treatment, or instruct a user to substitute a medication without appropriate veterinary involvement.

Medication comparisons shall clearly distinguish equivalent medications from therapeutic alternatives and non-equivalent products.

Risk assessments shall communicate uncertainty and should escalate appropriately when available information indicates potentially serious or emergency conditions.

The system shall prioritize medically appropriate and safety-adjusted options rather than automatically ranking medications according to price, popularity, or a single adverse-effect measurement.

All recommendations should identify important limitations, missing information, and circumstances in which professional veterinary evaluation is appropriate.

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
  - [https://roxanneardary.com/vetora/](https://roxanneardary.com/vetora/)  

---

## License & Notice Requirements

Vetora is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Vetora specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
