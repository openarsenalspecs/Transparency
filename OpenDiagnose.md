# OpenDiagnose

**OpenDiagnose — A commons for real-world problem solving.**

OpenDiagnose is a modular, AGPL-3.0+ diagnostic system that combines wearable vision hardware, edge AI, and structured reasoning to identify real-world problems and generate actionable fixes. It is designed as a fully open, composable system where hardware and software can be independently replaced while preserving a shared diagnostic specification.

---

## Overview

OpenDiagnose turns real-world visual input into structured diagnostic output. It captures images or video through wearable devices, processes them using interchangeable AI and rule-based systems, and returns clear, actionable repair guidance in real time via HUD display, audio, or printed output.

The system is built for field use across mechanical, electrical, agricultural, and infrastructure environments.

---

## Full Feature List

### Core System Features
- Real-time image and video capture
- Wearable heads-up display (HUD) output
- Structured diagnostic generation from visual input
- Confidence scoring for all diagnoses
- Severity classification (low, medium, high)
- Step-by-step repair instructions
- Multi-modal output (HUD, audio, print)

---

### Diagnostic Intelligence
- Hybrid reasoning system:
  - Computer vision models (YOLO, segmentation, detection)
  - Rule-based diagnostic packs
  - Optional LLM explanation layer
- Root-cause analysis (not just symptom detection)
- Domain-specific diagnostic packs:
  - Automotive systems
  - Electrical systems
  - Agriculture and crop health
  - HVAC and building systems
  - General machinery and tools
- Replaceable AI models (ONNX / TensorFlow Lite / PyTorch compatible)

---

### Hardware System (Modular Design)
- Swappable vision modules (camera systems)
- Compute tiers:
  - Embedded low-power devices (ESP32-S3)
  - Edge compute (Raspberry Pi Zero / Pi 5)
  - High-performance GPU-assisted nodes
- Heads-up display support:
  - Micro-OLED
  - Optical combiner HUD
- Portable battery modules with hot-swap capability
- Optional LTE/5G connectivity modules
- Bluetooth thermal printer support for physical diagnostic output

---

### Software Architecture
- Fully modular pipeline:
  - Capture Engine
  - Vision Processing Engine
  - Diagnostic Engine
  - Knowledge Retrieval Layer
  - Explanation Generator
  - Output Router
- Standardized diagnostic schema (machine + human readable)
- Offline-first operation with optional cloud sync
- Plugin-based system for models and tools
- Emulator and simulation environment for testing without hardware

---

### Knowledge System
- Versioned diagnostic knowledge packs
- Domain-specific rule libraries
- Vector-based similarity search (optional)
- Community-contributed fix database
- Field feedback loop to improve diagnostic accuracy
- Cross-domain failure pattern matching

---

### Output & Interaction
- HUD overlays:
  - Bounding boxes
  - Fault highlighting
  - Live annotations
- Audio feedback via text-to-speech
- Printable diagnostic reports with QR code extensions
- Mobile companion interface for monitoring and configuration

---

### Developer & Ecosystem Features
- AGPL-3.0+ network copyleft enforcement
- Fully modular plugin architecture
- Open hardware interface specification (HMI-BUS)
- JSON-over-serial communication standard
- Dataset and model training toolkit
- Field simulation and debugging tools
- Extensible domain pack system

---

### Future Capabilities
- Multi-device swarm diagnostics
- Peer-to-peer anomaly sharing network
- Self-updating diagnostic knowledge layers
- AR spatial mapping of system failures
- Community-verified repair reputation system
- Distributed field intelligence networks

---

## Architecture Principle

> The spec is the system. Implementations are interchangeable.

OpenDiagnose is designed so that no single model, hardware configuration, or vendor stack becomes required. Every layer is replaceable as long as it conforms to the shared diagnostic specification.

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
  - [https://roxanneardary.com/opendiagnose/](https://roxanneardary.com/opendiagnose/)  

---

## License & Notice Requirements

OpenDiagnose is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- OpenDiagnose specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

**Open Arsenal Hub**  
[https://gitlab.com/Roxanne_Ardary/open-arsenal-specs](https://gitlab.com/Roxanne_Ardary/open-arsenal-specs)
