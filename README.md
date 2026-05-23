# Medical Device Software Lifecycle Framework (IEC 62304 & ISO 13485)

This repository serves as a practical implementation framework for a Software Quality Management System (QMS) and Software Development Lifecycle (SDLC) conforming to **IEC 62304 (Class B)** and **ISO 13485** standards. 

## 📌 Overview
Unlike standard consumer software, Biomedical Software as a Medical Device (SaMD) requires rigorous documentation, risk mitigation tracing, and strict verification before deployment. This framework models the required Design History File (DHF) artifacts.

## 🗂️ Repository Structure
* `/regulatory-compliance/` — High-level compliance mapping for FDA regulations.
* `/software-requirements/` — Software Requirements Specification (SRS) documentation template.
* `/risk-management/` — Hazard analysis, software safety classification, and risk control verification logs (ISO 14971).

## 🛡️ Core Regulatory Competencies Demonstrated

### 1. Software Safety Classification (IEC 62304 Clause 4.3)
This framework assumes a **Class B** software classification (injury is possible before risk controls are applied). 
* **Requirement Tracing:** Every software requirement must map directly to a system-level user need.
* **Regression Testing:** Automated validation pipelines are required for all minor and major releases to prevent software regression.

### 2. Risk Management & Hazard Analysis (ISO 14971)
Below is the standard risk mitigation workflow implemented within this framework's documentation protocols:
* **Identify Hazard:** (e.g., Software loop freezes, stopping heart rate data transmission).
* **Mitigate Risk:** (e.g., Implement an independent hardware watchdog timer to reset software if frozen).

### 3. Verification vs. Validation Protocol
* **Verification:** Did we build the system right? Handled via unit testing and static code analysis tracking tools.
* **Validation:** Did we build the right system? Handled via cross-referencing final user needs against actual system performance metrics.
