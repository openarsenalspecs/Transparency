# GitPatrol

**AI that keeps your repo on the right side of the law.**

GitPatrol is an open-source, license-aware AI platform designed to continuously analyze Git repositories for licensing conflicts, attribution requirements, compliance risks, and legally inconsistent recommendations. It scans source code, documentation, configuration files, metadata, dependencies, generated content, and repository instructions to help ensure that project activity remains consistent with applicable licenses.

GitPatrol uses a modular architecture so repositories can deploy only the functionality they need. Core modules provide repository analysis, license intelligence, compliance enforcement, legal-safe recommendations, and token-efficient file construction. Optional plugin modules extend GitPatrol with integrations, editors, CI/CD systems, external license databases, notifications, historical analysis, and other specialized capabilities.

---

## Specification

GitPatrol is designed around several principles:

- **License-aware by design**
- **Repository-wide analysis**
- **Compliance before recommendation**
- **Human review for uncertain legal conclusions**
- **Minimal-character and token-efficient construction**
- **Modular and extensible architecture**
- **Local-first operation where practical**
- **Vendor-neutral integrations**
- **Machine-readable compliance results**
- **Automated enforcement with configurable controls**
- **Transparent findings and remediation**
- **No recommendation should intentionally conflict with applicable license terms**

GitPatrol should distinguish between confirmed license requirements, detected risks, compatibility questions, and matters requiring human or legal review. It should not represent uncertain interpretations as definitive legal conclusions.

---

## Core Modules

### Repository Scanner

The Repository Scanner provides comprehensive repository analysis.

Features include:

- Recursive repository scanning
- Source-code scanning
- Documentation scanning
- Configuration-file scanning
- Metadata scanning
- Manifest scanning
- Script scanning
- Example and sample-code scanning
- Template scanning
- Generated-file detection
- Binary and unsupported-file identification
- Hidden-file detection
- Ignore-rule support
- File classification
- Repository structure analysis
- Changed-file scanning
- Full-repository scanning
- Incremental scanning
- Scan caching
- File hashing
- Duplicate-content detection

---

### License Detection Engine

The License Detection Engine identifies licenses and licensing statements throughout the repository.

Features include:

- SPDX identifier detection
- License text recognition
- License-header detection
- File-level license detection
- Repository-level license detection
- Documentation license detection
- Dependency license detection
- Multiple-license detection
- Dual-license detection
- License exception detection
- Custom-license detection
- Unknown-license detection
- Conflicting-license detection
- License metadata comparison
- License confidence scoring

The engine should distinguish between a detected license identifier and the complete legal terms governing a work.

---

### License Rules Engine

The License Rules Engine converts known license requirements into machine-readable compliance rules.

Features include:

- License obligation mapping
- Attribution requirements
- Copyright-notice requirements
- Source-disclosure requirements
- Copyleft requirements
- Network-use requirements
- Notice requirements
- Modification requirements
- Distribution requirements
- License-preservation requirements
- Patent-related provisions
- Trademark-related provisions
- License-exception handling
- Custom repository license rules
- Project-specific compliance rules
- Rule precedence
- Rule conflict detection

The Rules Engine serves as the authoritative compliance layer used by other GitPatrol modules.

---

### Attribution Manager

The Attribution Manager identifies, verifies, constructs, and maintains attribution information.

Features include:

- Copyright attribution detection
- Contributor attribution tracking
- Required attribution detection
- NOTICE file analysis
- Attribution-header verification
- Attribution consistency checks
- Missing-attribution detection
- Duplicate-attribution detection
- Attribution consolidation
- Contributor contribution records
- Attribution history
- Minimal attribution generation
- Repository-wide attribution auditing

---

### Dependency Compliance Engine

The Dependency Compliance Engine evaluates third-party components and their relationship to the repository's licensing requirements.

Features include:

- Dependency discovery
- Manifest analysis
- Transitive dependency analysis
- Dependency license detection
- License compatibility analysis
- Copyleft interaction detection
- Incompatible-license warnings
- License exception detection
- Dependency attribution tracking
- Dependency notice tracking
- Version-specific license records
- Dependency compliance reports
- Unlicensed dependency detection

---

### Code and Content Compliance Analyzer

The Code and Content Compliance Analyzer examines repository content for licensing risks that simple header checks cannot identify.

Features include:

- License-related instruction analysis
- Documentation analysis
- README analysis
- Comment analysis
- Example-code analysis
- Embedded-license detection
- Third-party-content indicators
- Copied-content indicators
- License-conflicting instructions
- Redistribution instructions
- Relicensing instructions
- Attribution-removal instructions
- Source-disclosure avoidance instructions
- Content-policy conflicts
- Compliance-sensitive natural-language analysis

---

### License-Aware AI Reasoning Engine

The AI Reasoning Engine provides contextual analysis while remaining constrained by detected licensing requirements.

Features include:

- License-aware reasoning
- Repository-context analysis
- Natural-language license interpretation
- Compliance question answering
- License conflict identification
- Recommendation validation
- Instruction conflict detection
- Safe alternative generation
- Uncertainty detection
- Human-review escalation
- Evidence-based explanations
- Source-file references
- Rule-based reasoning constraints

The reasoning engine must evaluate applicable license requirements before generating recommendations.

---

### Safe Recommendation Engine

The Safe Recommendation Engine prevents GitPatrol from recommending actions that conflict with known licensing obligations.

Features include:

- License-aware recommendations
- Compliance-safe remediation
- Recommendation validation
- Conflicting-instruction detection
- Unsafe-action blocking
- Alternative recommendation generation
- Human-review recommendations
- Legal uncertainty warnings
- Evidence references
- Minimal remediation suggestions

Recommendations should never override known license requirements merely because an alternative is easier, shorter, or technically preferable.

---

### Minimal File Construction Engine

The Minimal File Construction Engine creates repository files using the smallest practical amount of text while preserving required legal meaning.

Features include:

- Minimal license headers
- Minimal attribution headers
- Minimal NOTICE entries
- Minimal README sections
- Minimal compliance notices
- Boilerplate reduction
- Redundancy removal
- Duplicate-text consolidation
- Whitespace optimization
- Character-count optimization
- Token-count optimization
- Semantic-preservation checks
- Legal-requirement preservation
- Language-specific header generation
- File-type-specific formatting

Optimization must never remove information that is legally required by the applicable license or project requirements.

---

### Compliance Scanner

The Compliance Scanner combines the repository, license, attribution, dependency, and AI analysis systems into a unified compliance assessment.

Features include:

- Full compliance scans
- Incremental scans
- Pre-commit scans
- Pre-push scans
- Pull-request scans
- Merge-request scans
- Release scans
- Dependency scans
- Documentation scans
- Attribution scans
- License compatibility scans
- Compliance regression detection
- Configurable enforcement levels

---

### Risk Analysis Engine

The Risk Analysis Engine prioritizes detected issues.

Features include:

- Compliance risk scoring
- File-level risk scores
- Repository-level risk scores
- Dependency risk scores
- Attribution risk scores
- License-conflict severity
- Confidence scoring
- Uncertainty scoring
- Critical-issue detection
- Compliance trend analysis
- Remediation prioritization

Risk scores should clearly distinguish technical detection confidence from legal certainty.

---

### Auto-Fix Engine

The Auto-Fix Engine provides controlled repository remediation.

Features include:

- Missing-header insertion
- Header correction
- Attribution correction
- NOTICE updates
- License metadata correction
- Documentation correction
- Minimal-text replacement
- Redundant-text removal
- Dependency notice updates
- Configuration updates
- Preview mode
- Dry-run mode
- Approval-required mode
- Automatic application mode
- Change logging
- Rollback support

---

### Compliance Reporting Engine

The Compliance Reporting Engine produces both human-readable and machine-readable results.

Features include:

- Repository compliance reports
- File-level findings
- License inventories
- Attribution reports
- Dependency reports
- Risk reports
- Remediation reports
- Change reports
- Historical reports
- Compliance summaries
- JSON output
- YAML output
- Markdown output
- CI-friendly output
- Exit-code enforcement

---

### Policy Engine

The Policy Engine allows repository maintainers to define project-specific requirements.

Features include:

- Allowed-license policies
- Restricted-license policies
- Required-attribution policies
- Required-header policies
- Dependency policies
- File-specific policies
- Directory-specific policies
- Documentation policies
- Contribution policies
- Enforcement thresholds
- Custom compliance rules
- Organization-wide policies
- Repository-specific overrides

---

### Audit Trail

The Audit Trail records compliance decisions and automated changes.

Features include:

- Scan history
- Finding history
- Rule history
- Auto-fix history
- Recommendation history
- Configuration history
- License-detection history
- Attribution changes
- Dependency changes
- Compliance status changes
- User approvals
- Human overrides
- Exportable audit records

---

### CLI

The command-line interface provides direct access to GitPatrol functionality.

Example commands may include:

- `gitpatrol scan`
- `gitpatrol licenses`
- `gitpatrol dependencies`
- `gitpatrol attribution`
- `gitpatrol check`
- `gitpatrol fix`
- `gitpatrol report`
- `gitpatrol audit`
- `gitpatrol policy`
- `gitpatrol generate`

The CLI should support machine-readable output for automation.

---

### Configuration System

The Configuration System centralizes GitPatrol behavior.

Features include:

- Repository configuration
- License configuration
- Attribution configuration
- Policy configuration
- Ignore rules
- File-type rules
- Plugin configuration
- AI configuration
- Scan configuration
- Enforcement configuration
- Output configuration
- Privacy configuration
- Local-model configuration
- Environment-variable support

---

### API

The API exposes GitPatrol functionality to external applications.

Features include:

- Repository scanning
- File analysis
- License detection
- Dependency analysis
- Compliance checks
- Risk assessment
- Report generation
- Auto-fix previews
- Policy evaluation
- Plugin communication
- Machine-readable responses

---

## Optional Plugin Modules

GitPatrol can be extended through optional plugins without adding unnecessary functionality to the core installation.

### Git Hosting Plugins

Optional integrations may support:

- GitLab
- GitHub
- Codeberg
- Gitea
- Forgejo
- Self-hosted Git services
- Pull requests
- Merge requests
- Repository webhooks
- Commit status reporting

---

### CI/CD Plugins

Optional CI/CD integrations may support:

- GitLab CI/CD
- GitHub Actions
- Codeberg CI
- Jenkins
- Drone
- Woodpecker
- Generic pipeline runners
- Pre-commit automation
- Pre-push automation
- Release validation

---

### Editor Plugins

Optional editor integrations may support:

- Visual Studio Code
- JetBrains IDEs
- Sublime Text
- Neovim
- Vim
- Emacs

Features may include:

- Inline compliance warnings
- License-header generation
- Attribution suggestions
- Quick fixes
- File-level scans
- Repository-level scans

---

### License Database Plugins

Optional plugins may connect GitPatrol to external license information sources.

Features may include:

- SPDX data
- License metadata
- License identifiers
- License text references
- License exceptions
- Versioned license information
- Custom organizational license databases

External legal data should be treated as an information source rather than an automatic substitute for legal review.

---

### Notification Plugins

Optional notification integrations may support:

- Email
- Slack
- Discord
- Microsoft Teams
- Webhooks
- Repository comments
- Issue creation
- Dashboard alerts

---

### Historical Analysis Plugins

Historical plugins can analyze repository history for compliance changes.

Features include:

- Commit analysis
- Contributor history
- License changes
- Attribution changes
- Dependency changes
- Compliance regressions
- Historical risk analysis
- First-detection tracking

---

### Similarity and Provenance Plugins

Optional provenance plugins can identify potential third-party or previously published material.

Features include:

- Code similarity analysis
- Documentation similarity analysis
- Snippet matching
- Provenance indicators
- Duplicate-content detection
- Source-reference tracking
- Potential copied-content alerts

Findings should be presented as indicators requiring verification rather than definitive ownership conclusions.

---

### AI Model Plugins

GitPatrol may support multiple AI backends.

Possible capabilities include:

- Local language models
- Remote language models
- Embedding models
- Specialized legal-text models
- Code models
- Classification models
- Model routing
- Model fallback
- Offline analysis

The compliance rules layer should remain independent of any particular AI provider.

---

### Storage Plugins

Optional storage integrations may support:

- SQLite
- PostgreSQL
- MySQL-compatible databases
- Object storage
- Local filesystem
- Remote repositories
- Compliance archives

---

### Dashboard Plugin

An optional web dashboard may provide:

- Repository overview
- Compliance status
- License inventory
- Attribution status
- Dependency status
- Risk visualization
- Scan history
- Remediation tracking
- Policy management
- Audit history
- Plugin management

---

### Organization Plugin

Optional organization-level functionality may provide:

- Multi-repository monitoring
- Centralized policies
- Shared license rules
- Shared attribution rules
- Organization dashboards
- Team permissions
- Compliance reporting
- Repository grouping
- Organization-wide audit trails

---

## Modular Architecture

GitPatrol should maintain clear boundaries between modules.

The architecture should support:

- Independent module development
- Independent module testing
- Plugin discovery
- Plugin enablement and disablement
- Module configuration
- Dependency injection
- Event-driven communication
- API-based module communication
- Replaceable AI providers
- Replaceable storage providers
- Replaceable Git providers
- Local-first operation
- Offline-capable core analysis

Core functionality should not depend on optional external services unless explicitly enabled by the repository administrator.

---

## Event Bus

GitPatrol can use an internal event bus to connect modules without tightly coupling them.

Example events include:

- Repository scanned
- File discovered
- License detected
- License conflict detected
- Attribution missing
- Dependency discovered
- Compliance issue detected
- Risk score changed
- Recommendation generated
- Auto-fix proposed
- Auto-fix applied
- Pull request analyzed
- Compliance status changed

Plugins can subscribe to supported events without modifying core modules.

---

## Service Interfaces

Core services should expose stable interfaces for:

- Repository access
- File analysis
- License detection
- License rules
- Attribution management
- Dependency analysis
- AI reasoning
- Recommendation validation
- File generation
- Compliance reporting
- Policy evaluation
- Audit logging
- Plugin communication

This allows individual implementations to be replaced without redesigning the entire system.

---

## Security and Privacy

GitPatrol should prioritize repository security and privacy.

Features include:

- Local scanning
- Optional offline AI operation
- No mandatory external repository upload
- Configurable telemetry
- Secret-aware scanning
- Credential redaction
- Sensitive-file exclusion
- Permission-aware integrations
- Plugin permissions
- Audit logging
- Secure configuration
- Least-privilege integration
- Explicit external-service authorization

Repository contents should not be transmitted to external AI or analysis services unless the administrator explicitly enables such functionality.

---

## Compliance Philosophy

GitPatrol is designed to reduce accidental licensing violations, not to replace qualified legal counsel.

The system should:

- Identify applicable license information
- Explain detected obligations
- Detect potential conflicts
- Preserve required notices and attribution
- Prevent obviously conflicting recommendations
- Identify uncertainty
- Provide evidence for findings
- Escalate ambiguous legal questions
- Avoid claiming certainty where the underlying license interpretation is unclear

---

## Development

GitPatrol is designed as an open-source project with modular development in mind.

Contributors can develop:

- Core modules
- Compliance rules
- License adapters
- Repository adapters
- AI providers
- Storage providers
- CI/CD integrations
- Editor plugins
- Reporting formats
- Notification plugins
- Dashboard components

New functionality should be implemented as a plugin when it is not required by the core compliance architecture.

---

## Contributing

Contributions are welcome.

Before submitting changes:

- Review the project's contribution requirements.
- Preserve license and attribution requirements.
- Ensure new files contain applicable license information.
- Test compliance-related changes.
- Avoid introducing unnecessary dependencies.
- Keep implementations modular.
- Preserve token-efficient file construction.
- Document new compliance rules.
- Update relevant documentation.
- Update `notice.md` when required.

See `contributing.md` for complete contribution requirements.  

---

## Project Goal

GitPatrol aims to make license compliance a continuous part of software development rather than a manual review performed after a repository has already accumulated risk.

**Scan everything. Understand the license. Preserve the obligations. Recommend safely. Build minimally.**

---

## Specification Branding License (SBL)

- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/gitpatrol/](https://roxanneardary.com/gitpatrol/)

---

## License & Notice Requirements

GitPatrol is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- GitPatrol specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
