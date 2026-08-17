# PureScript
**Human Writing. Human Privacy.**
- HTML Mirror: [https://roxanneardary.com/purescript-specification/](https://roxanneardary.com/purescript-specification/)

---

PureScript is an open-source, privacy-first document writer designed to combine the capabilities of a modern office document editor with document-level encryption, secure sharing, cryptographic identity, and human-centered privacy protections.

The specification defines a modular writing platform in which document creation, formatting, rendering, encryption, identity, permissions, storage, sharing, and collaboration operate as coordinated core modules. PureScript is designed so that an encrypted document remains protected when transferred through email, text messaging, social media, cloud storage, removable media, or other untrusted transport systems.

## Specification Goals

PureScript is designed around the following goals:

- Provide a complete modern document writing environment.
- Make document encryption a default security property.
- Keep document content under the control of its authorized users.
- Separate document security from the security of the transport platform.
- Support professional typography, fonts, formatting, and page layout.
- Provide cryptographic document authenticity and integrity.
- Support secure local and offline document creation.
- Support optional encrypted collaboration without requiring trusted infrastructure.
- Provide a modular architecture that can evolve without compromising the security core.
- Avoid unnecessary dependence on proprietary platforms or cloud services.
- Preserve user control over encryption keys and document access.

# Core Architecture

PureScript uses a modular architecture. Core modules provide the fundamental writing, document, security, rendering, and storage capabilities. Optional plugin modules extend functionality without requiring changes to the fundamental security model.

Modules should communicate through defined interfaces and should not bypass the document security layer.

Security-sensitive operations must remain within audited core modules or explicitly trusted security plugins.

---

# Core Modules

## Document Engine

The Document Engine provides the fundamental document model.

Features include:

- Rich text documents
- Paragraphs
- Headings
- Lists
- Tables
- Footnotes
- Endnotes
- Sections
- Columns
- Page breaks
- Headers
- Footers
- Page numbering
- Document metadata
- Embedded objects
- Document styles
- Templates
- Revision-aware document structures

The document model should separate content, presentation, metadata, and security information so that each layer can be independently managed.

## Writing Editor

The Writing Editor provides the primary human writing interface.

Features include:

- Rich text editing
- Text selection
- Find and replace
- Undo and redo
- Spell checking
- Grammar assistance
- Word counting
- Character counting
- Paragraph controls
- Formatting controls
- Style management
- Keyboard shortcuts
- Accessibility controls
- Writing assistance
- Drag and drop editing

The editor must never expose decrypted document content to unauthorized processes or services.

## Typography and Font Engine

The Typography and Font Engine provides professional document typography.

Features include:

- OpenType font support
- TrueType font support
- Variable fonts
- Font families
- Font weights
- Font styles
- Kerning
- Ligatures
- Character spacing
- Line spacing
- Text alignment
- Advanced text shaping
- Multilingual typography
- Right-to-left text
- Script-specific rendering
- Embedded document fonts

Fonts may be packaged with documents when licensing permits.

The system should provide a broad selection of open-source fonts while allowing users to install additional compatible fonts.

## Layout Engine

The Layout Engine converts document content into structured pages and rendered views.

Features include:

- Automatic pagination
- Page dimensions
- Margins
- Columns
- Text flow
- Image placement
- Table layout
- Headers and footers
- Section breaks
- Print layout
- Screen layout
- Export layout
- Accessibility-aware layout

Layout calculations should remain deterministic wherever practical so that documents render consistently across supported platforms.

## Rendering Engine

The Rendering Engine displays document content to the user.

Features include:

- High-resolution text rendering
- GPU acceleration where available
- Vector-based glyph rendering
- Zoom controls
- Page previews
- Continuous document view
- Print preview
- Accessibility rendering
- High contrast modes
- Display scaling

The rendering system should minimize unnecessary exposure of decrypted document content to external applications.

## Encryption Engine

The Encryption Engine provides document confidentiality.

Features include:

- Encryption by default
- Strong authenticated encryption
- Per-document encryption keys
- Key wrapping
- Secure key generation
- Secure key storage
- Key rotation
- Recipient key management
- Secure deletion of temporary plaintext data
- Cryptographic verification
- Encryption state verification

The encryption architecture should use established, peer-reviewed cryptographic primitives rather than custom cryptography.

The system should support modern authenticated encryption such as AES-256-GCM and provide an architecture capable of supporting additional algorithms as cryptographic standards evolve.

## Identity and Key Management

The Identity and Key Management module controls cryptographic identities.

Features include:

- User identities
- Public and private key pairs
- Key generation
- Key import and export
- Key rotation
- Key verification
- Recipient identification
- Device identity
- Trusted device management
- Key revocation
- Recovery mechanisms

Private keys must remain under user control.

The system must not require a centralized identity provider to operate.

## Document Signature Module

The Document Signature Module establishes document authenticity and integrity.

Features include:

- Author signatures
- Document signatures
- Revision signatures
- Signature verification
- Tamper detection
- Author identity verification
- Signature timestamps
- Verification status

Cryptographic signatures should distinguish between document authorship, document ownership, and authorization to modify a document.

## Access Control Module

The Access Control Module manages document permissions.

Supported permissions may include:

- Read
- Edit
- Comment
- Review
- Export
- Print
- Share
- Copy
- Administrative control

Permissions must be enforced by the application and cryptographic access layer rather than relying exclusively on the transport platform.

Access rules should support:

- Individual recipients
- Groups
- Multiple devices
- Temporary access
- Revocation
- Expiration
- Read-only access
- Editing access

## Secure Document Container

The Secure Document Container defines how encrypted documents are packaged.

The container should support:

- Version information
- Encryption metadata
- Recipient key information
- Encrypted document content
- Encrypted formatting information
- Encrypted embedded media
- Encrypted font resources where permitted
- Document signatures
- Revision information
- Access policies

The container should minimize unencrypted metadata.

The proposed document extension is `.psdoc`.

## Secure Storage Module

The Secure Storage Module manages local document storage.

Features include:

- Encrypted local storage
- Document locking
- Automatic save
- Crash recovery
- Temporary file protection
- Secure deletion
- Version recovery
- Local document indexing
- Encrypted document metadata

Plaintext temporary files should not be created unnecessarily.

## Secure Sharing Module

The Secure Sharing Module allows encrypted documents to be transmitted through untrusted systems.

Supported transport methods may include:

- Email attachments
- Text messaging
- Direct messaging
- Social media messaging
- Cloud storage
- USB storage
- Local network transfer
- Peer-to-peer transfer

The transport system must be treated as untrusted.

Document confidentiality must depend on document encryption and authorization rather than on the security promises of the transport provider.

## Collaboration Module

The Collaboration Module provides optional encrypted multi-user editing.

Features include:

- Multi-user editing
- Encrypted synchronization
- Conflict resolution
- Revision tracking
- Comments
- Review workflows
- Document locking
- Cryptographically verified revisions

Collaboration infrastructure should not require access to document plaintext.

Where collaborative synchronization requires server infrastructure, the architecture should use end-to-end encryption so that servers cannot routinely access document content.

## Revision and History Module

The Revision and History Module maintains document changes.

Features include:

- Revision history
- Author identification
- Revision timestamps
- Change tracking
- Restore points
- Revision comparison
- Signed revisions
- Tamper detection

Users should be able to determine whether a document has changed since a previous verified state.

## Import and Export Module

The Import and Export Module allows users to work with established document formats.

Potential formats include:

- OpenDocument Text
- Microsoft Word formats
- Rich Text Format
- Plain text
- HTML
- PDF
- Markdown

Import and export operations should clearly indicate when content is leaving the encrypted PureScript environment.

Exported plaintext documents must never be represented as equivalent to encrypted `.psdoc` documents.

## Accessibility Module

The Accessibility Module provides accessible document creation and reading.

Features include:

- Screen reader support
- Keyboard navigation
- Adjustable text size
- High contrast modes
- Accessible document structure
- Alternative text
- Accessibility metadata
- Reduced motion options
- Assistive technology compatibility

Accessibility features must not require disclosure of document content to external services.

## Offline Module

The Offline Module provides full local functionality without requiring network access.

Features include:

- Offline document creation
- Offline document editing
- Offline encryption
- Offline decryption
- Local key management
- Local document search
- Local revision history
- Offline export

Internet connectivity should be optional rather than a prerequisite for core writing functionality.

## Privacy Module

The Privacy Module provides system-wide privacy controls.

Features include:

- Minimal telemetry
- No mandatory cloud account
- Local-first operation
- User-controlled data storage
- Privacy-preserving diagnostics
- Secure temporary data handling
- Configurable network access
- External service controls

PureScript should not transmit document content for analytics, advertising, model training, or unrelated diagnostics.

## Security Audit Module

The Security Audit Module provides visibility into security-sensitive operations.

Features include:

- Encryption status
- Key status
- Signature status
- Access status
- Document integrity status
- Security warnings
- Configuration review
- Audit events

Security information should be understandable to ordinary users while also providing detailed information for technical reviewers.

# Optional Plugin Modules

Optional plugins may extend PureScript without becoming mandatory dependencies for the core document editor.

## Spreadsheet Plugin

Provides spreadsheet functionality including:

- Worksheets
- Formulas
- Charts
- Tables
- Cell formatting
- Encrypted spreadsheet documents

## Presentation Plugin

Provides presentation authoring including:

- Slides
- Themes
- Speaker notes
- Transitions
- Embedded media
- Presentation export

## PDF Plugin

Provides advanced PDF functionality including:

- PDF creation
- PDF annotation
- PDF import
- PDF export
- Encrypted PDF workflows
- Document verification

## Research Plugin

Provides research-oriented tools including:

- Citation management
- Bibliographies
- Research notes
- Source organization
- Reference metadata
- Encrypted research libraries

## Writing Assistant Plugin

Provides optional local writing assistance including:

- Grammar checking
- Spelling assistance
- Style analysis
- Readability analysis
- Writing suggestions
- Custom dictionaries

Writing assistance should support local processing whenever practical.

## Local AI Plugin

Provides optional locally executed AI functionality.

Features may include:

- Summarization
- Classification
- Editing assistance
- Outline generation
- Document analysis
- Search assistance

The plugin must not transmit document content to external AI services unless the user explicitly enables such functionality.

## Secure OCR Plugin

Provides optional optical character recognition for:

- Scanned documents
- Images
- PDFs
- Photographs of printed material

OCR processing should support local execution.

## Translation Plugin

Provides optional document translation.

Local translation engines should be supported where available.

External translation services must require explicit user authorization before encrypted document content is transmitted.

## Template Plugin

Provides document templates for:

- Letters
- Reports
- Contracts
- Research papers
- Business documents
- Academic documents
- Personal documents

Templates should be separated from private document content.

## Publishing Plugin

Provides publishing workflows for:

- HTML
- EPUB
- PDF
- Print-ready documents
- Accessible publications

Publishing must clearly distinguish secure encrypted storage from intentionally published content.

## Secure Clipboard Plugin

Provides enhanced clipboard protection.

Features may include:

- Encrypted clipboard contents
- Automatic clipboard expiration
- Clipboard clearing
- Copy restrictions
- Paste restrictions
- Clipboard access notifications

## Secure Screen Plugin

Provides optional screen privacy features.

Potential capabilities include:

- Privacy overlays
- Screen capture warnings
- Screenshot deterrence
- Sensitive document indicators
- Automatic privacy mode

Operating system limitations must be clearly disclosed. No application should claim to prevent screenshots or cameras in situations where the operating system cannot enforce such restrictions.

## Plugin Security Requirements

All plugins must:

- Declare required permissions.
- Clearly identify access to document content.
- Respect the core encryption architecture.
- Avoid unauthorized plaintext transmission.
- Avoid weakening key protection.
- Provide auditable source code when distributed as open-source software.
- Document external services and network requirements.
- Maintain compatibility with the project's licensing requirements.

Plugins must not silently bypass core security controls.

# Human Privacy Model

PureScript is designed around the principle that the person creating a document should control who can read it.

The system should distinguish between:

- Human-readable content
- Machine-readable metadata
- Cryptographic metadata
- Application state
- Transport data

PureScript should minimize machine-readable information wherever practical.

The project may provide privacy-enhancing rendering techniques designed to make automated extraction more difficult. Such techniques must never be described as guaranteeing that humans alone can read a document. A determined recipient can potentially photograph, screenshot, transcribe, or otherwise capture information displayed on a screen.

The security model therefore focuses on cryptographic confidentiality, access control, key ownership, and minimizing unnecessary exposure.

# Transport Independence

PureScript does not assume that email providers, messaging platforms, social media platforms, cloud storage providers, or network operators are trustworthy.

A `.psdoc` file should remain encrypted when:

- Attached to an email
- Uploaded to cloud storage
- Sent through a messaging application
- Sent through a social media platform
- Copied to removable storage
- Stored on a shared filesystem
- Transferred over an untrusted network

The receiving user must possess the appropriate cryptographic authorization to decrypt the document.

# Security Principles

PureScript follows these principles:

- Encryption by default
- Least privilege
- Zero-trust transport
- User-controlled keys
- Local-first operation
- Minimal metadata
- Secure defaults
- Explicit permissions
- Cryptographic verification
- Transparent security design
- Open-source auditability
- No security through obscurity

The project should never claim absolute security.

Security claims must be based on documented technical properties and independently verifiable implementation details.

# Cross-Platform Design

PureScript is intended to support:

- Linux
- Windows
- macOS
- Android
- iOS

Platform-specific security capabilities should be implemented through isolated interfaces so that the core document and cryptographic model remains consistent across platforms.

# Performance Requirements

PureScript should prioritize:

- Fast startup
- Responsive editing
- Efficient document rendering
- Low memory usage
- Efficient encryption
- Efficient local search
- Large-document support
- Reliable autosave
- Crash recovery

Security operations should be optimized without weakening cryptographic protections.

# Data Ownership

Users retain control over their documents and encryption keys.

PureScript should not require:

- A mandatory cloud account
- A proprietary storage provider
- A mandatory subscription
- A centralized document repository
- External AI processing

Optional services may be provided through plugins or self-hosted infrastructure.

# Interoperability

PureScript should support standards-based interoperability wherever practical.

The project should prioritize:

- Open document formats
- Open font standards
- Open cryptographic standards
- Portable encrypted documents
- Accessible document structures
- Document conversion without vendor lock-in

# Extensibility

The plugin architecture should allow new functionality to be added without requiring modifications to unrelated core modules.

Plugins should communicate with the core through documented interfaces.

Security-sensitive APIs should require explicit permission declarations.

# Development Principles

Development should prioritize:

- Security
- Privacy
- Reliability
- Accessibility
- Interoperability
- Maintainability
- Performance
- User control
- Open-source transparency

New functionality should not be accepted solely because it adds convenience if it creates unnecessary privacy or security risks.

# Future Development

Potential future capabilities include:

- Post-quantum cryptographic support
- Hardware security key integration
- Advanced key recovery
- Decentralized identity
- Secure document notarization
- Cryptographically verifiable publication
- Encrypted distributed collaboration
- Secure document synchronization
- Advanced document provenance
- Privacy-preserving local AI
- Additional open document format support

Future cryptographic capabilities must be implemented only after appropriate technical review and validation.

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
  - [https://roxanneardary.com/purescript/](https://roxanneardary.com/purescript/)

---

## License & Notice Requirements

PureScript is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- PureScript specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
