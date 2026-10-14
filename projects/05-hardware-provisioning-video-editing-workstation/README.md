# Lab 05: Hardware Provisioning — Video Editing Workstation

## 📌 Executive Summary

This project simulates an enterprise IT support request to assess, plan, and recommend a workstation for a new video editor working with 4K video and high-resolution visual content.

The objective is to translate business and application requirements into a technically justified workstation specification while balancing performance, compatibility, scalability, and cost.

The assessment will use official software documentation as the primary reference for hardware requirements. Proposed components will be evaluated for compatibility, storage capacity, network connectivity, and future expansion before a purchasing recommendation is made.

This project focuses on **requirements assessment and workstation planning**. No physical workstation will be purchased, assembled, or deployed during the initial phase.

---

## 🎯 Objectives & Scope

This project demonstrates the following IT support and systems administration practices:

- Identify role-based workstation requirements.
- Assess the technical requirements of Adobe Premiere Pro and the target operating system.
- Research official software documentation and record relevant requirements.
- Translate application requirements into a balanced hardware specification.
- Evaluate CPU, RAM, GPU, motherboard, storage, power supply, cooling, and display requirements.
- Validate component compatibility using manufacturer documentation.
- Estimate storage capacity based on expected media production and project retention.
- Assess Ethernet connectivity, cloud collaboration, and shared-storage requirements.
- Compare workstation configurations using verifiable pricing and documented assumptions.
- Evaluate upgrade paths and avoid unnecessary hardware expenditure.
- Define a workstation provisioning plan and acceptance criteria.
- Document findings, supporting evidence, risks, and the final recommendation.

### Out of Scope

The following activities are outside the initial scope of this project:

- Purchasing physical hardware.
- Assembling or deploying a physical workstation.
- Installing Windows or Adobe Premiere Pro on a production computer.
- Performing physical hardware benchmarks.
- Conducting production video-editing performance tests.
- Implementing an enterprise NAS or 10 GbE network.
- Purchasing software licences or cloud-storage subscriptions.
- Deploying enterprise-wide endpoint management.
- Establishing a production backup infrastructure.

These activities may be considered in a future implementation phase if required.

---

## 🏢 Simulated Enterprise Scenario

- **Company:** NexaCorp Solutions Ltd.
- **Department:** Marketing & Growth
- **Employee:** John
- **Job Title:** Video Editor
- **Request:** New workstation provisioning
- **Ticket:** TBD
- **Workstation:** TBD
- **Primary Application:** Adobe Premiere Pro
- **Target Operating System:** Windows 11
- **Project Status:** Requirements Assessment and Hardware Planning

### Business Context

A new employee has joined the marketing team and will be responsible for producing promotional videos, 4K content, and high-resolution visual assets for online campaigns.

The existing standard workstation profile has not yet been demonstrated to meet this role's requirements.

IT Support must assess the employee's workflow, identify the application's technical requirements, and recommend a suitable workstation without unnecessarily increasing the organization's hardware expenditure.

The proposed solution must support productive editing, reliable access to large media files, appropriate colour representation, secure data handling, and a practical upgrade path.

The final recommendation will be submitted for management review before any hardware acquisition takes place.

---

## 🧩 Project Approach

The assessment follows a requirements-driven process:

**Business Requirements → Software Requirements → Hardware Selection → Compatibility Validation → Cost Analysis → Provisioning Plan → Acceptance Criteria**

Hardware selection will be based on documented requirements and expected workloads rather than isolated component specifications.

Official vendor documentation will take priority over third-party summaries when establishing application compatibility and minimum or recommended system requirements.

Where requirements are not yet known, assumptions will be documented and validated before a final purchasing decision.

---

## 🖥️ Initial Workstation Profile

The following values represent the initial configuration under evaluation. They are planning targets, not a final purchasing decision.

| Component | Initial Planning Target | Assessment Focus |
|---|---|---|
| CPU | Modern processor with strong general and multicore performance | Application requirements, codec acceleration, compatibility, and value |
| RAM | 32 GB, with a possible upgrade to 64 GB | 4K editing workload, multitasking, and memory expansion |
| GPU | Dedicated graphics card with 8 GB VRAM | Application support, GPU acceleration, drivers, and workload suitability |
| Primary Storage | 1 TB NVMe SSD | Operating system, applications, cache, and active projects |
| Additional Storage | Capacity to be determined | Media files, active projects, archive, and backup |
| Display | 4K monitor with suitable colour characteristics | Resolution, colour gamut, calibration, bit depth, and HDR requirements |
| Network | Gigabit Ethernet as an initial baseline | Internet connectivity and local collaboration requirements |
| Operating System | Windows 11 | Application compatibility, security, and support lifecycle |

The final configuration may differ from these initial targets if official requirements, compatibility checks, workload estimates, or cost comparisons justify a change.

---

## 🔬 Assessment Workstreams

### 1. Requirements Assessment

Document the employee's expected workload, including:

- Video resolution and formats.
- Typical project size and duration.
- Expected weekly media production.
- Effects, colour grading, and graphics requirements.
- Concurrent applications and multitasking needs.
- Collaboration and file-sharing requirements.
- Project retention and recovery expectations.

### 2. Official Software Requirements Research

Review the official requirements for Adobe Premiere Pro and the target operating system.

Record:

- Source URL and publisher.
- Date of consultation.
- Relevant software version.
- Minimum and recommended requirements.
- Supported hardware and operating-system constraints.
- Implications for the proposed workstation.

Reference:

- [Adobe Premiere Pro Technical Requirements](https://helpx.adobe.com/br/premiere/desktop/get-started/technical-requirements/adobe-premiere-pro-technical-requirements.html)
- [Adobe Processor, Memory, and GPU Recommendations](https://helpx.adobe.com/br/premiere/desktop/get-started/technical-requirements/processor-memory-and-gpu-recommendations.html)

Requirements must be rechecked against the version selected for the final assessment.

### 3. Hardware Selection and Compatibility

Evaluate candidate components against the documented requirements.

Compatibility checks will include:

- CPU socket and motherboard support.
- Motherboard chipset and firmware requirements.
- RAM type, capacity, supported speeds, and expansion limits.
- GPU compatibility, physical dimensions, power requirements, and display outputs.
- SSD interface, form factor, and available storage slots.
- Power supply capacity and required connectors.
- Case dimensions and cooling requirements.
- Monitor resolution, colour characteristics, and connectivity.

A component will not be considered compatible solely because its headline specifications appear suitable.

### 4. Storage and Data Lifecycle Planning

Estimate storage requirements using expected media production, project duration, cache usage, exports, retention periods, and available capacity.

Distinguish between:

- **Operational storage:** Active projects, applications, and temporary files.
- **Archive storage:** Completed projects retained for future access.
- **Backup storage:** Independent recovery copies.

OneDrive will be assessed for appropriate collaboration and file-sharing use. Cloud synchronisation will not be treated as a substitute for fast local editing storage or an independent backup strategy.

### 5. Network and Collaboration Assessment

Evaluate the required network connectivity according to the intended workflow.

The assessment will consider:

- Gigabit Ethernet for the initial workstation baseline.
- Internet upload and download requirements.
- Large-file transfer times.
- Cloud collaboration and synchronisation behaviour.
- Shared-storage access requirements.
- Whether a future NAS or 10 GbE infrastructure is justified.

Higher network capacity will be recommended only when the workload and cost-benefit assessment support the investment.

### 6. Cost-Benefit Analysis

Compare at least three workstation configurations:

- **Budget-oriented:** Meets the documented requirements at the lowest reasonable cost.
- **Balanced:** Provides suitable performance, practical scalability, and a controlled initial investment.
- **Higher-capacity:** Offers additional resources for demonstrably more demanding workloads.

Record component models, prices, vendors, source URLs, currency, consultation dates, warranty information, and relevant assumptions.

The comparison will include the cost of the complete proposed solution rather than the processor and graphics card alone.

### 7. Provisioning and Acceptance Planning

Define the steps required to provision the workstation after management approval.

The plan will cover:

- Hardware acquisition and compatibility verification.
- Operating-system installation and updates.
- Approved application installation and licensing.
- Endpoint security configuration.
- Network and storage configuration.
- Backup and recovery arrangements.
- Performance and operational validation.
- Asset inventory and handover documentation.

Acceptance criteria will be defined before implementation so that the completed workstation can be assessed objectively.

---

## 🛠️ Skills & Technologies Applied

- IT Support Requirements Assessment
- Hardware Provisioning
- Workstation Specification
- Software Requirements Analysis
- Hardware Compatibility Assessment
- Cost-Benefit Analysis
- CPU, RAM, and GPU Selection
- Storage Capacity Planning
- SSD and Data Lifecycle Planning
- Network Connectivity Assessment
- Microsoft Windows 11
- Adobe Premiere Pro
- Microsoft OneDrive
- Backup and Recovery Planning
- Technical Documentation
- Evidence-Based Decision Making

---

## 📂 Project Deliverables

| Deliverable | Purpose |
|---|---|
| Requirements Assessment | Documents business needs and expected workloads |
| Software Requirements Matrix | Records official application and operating-system requirements |
| Workstation Specification | Defines the proposed hardware configuration |
| Compatibility Matrix | Documents component compatibility checks |
| Storage and Network Plan | Estimates capacity and defines the intended data workflow |
| Cost Comparison | Compares budget-oriented, balanced, and higher-capacity configurations |
| Provisioning Plan | Defines the future implementation sequence |
| Acceptance Checklist | Establishes criteria for verifying the completed workstation |
| Evidence Register | Tracks sources, screenshots, and supporting documentation |
| Final Recommendation | Summarises the recommended configuration and approval conditions |

---

## 📋 Evidence and Validation

Evidence will be collected and recorded throughout the project.

| Evidence ID | Description | Status |
|---|---|---|
| EV-01 | Business and workload requirements | Pending |
| EV-02 | Official software requirements research | Pending |
| EV-03 | Initial workstation specification | Pending |
| EV-04 | Hardware compatibility assessment | Pending |
| EV-05 | Storage and network capacity assessment | Pending |
| EV-06 | Cost comparison and pricing sources | Pending |
| EV-07 | Provisioning and acceptance plan | Pending |
| EV-08 | Final recommendation | Pending |

Evidence will distinguish between vendor-published specifications, planning assumptions, analytical estimates, and observed test results.

No physical implementation or performance test will be reported as completed unless it has actually been performed and documented.

---

## ⚠️ Risks, Assumptions, and Limitations

The assessment depends on several factors that must be confirmed:

- The final Adobe Premiere Pro version and licensing arrangement.
- The actual media formats, codecs, and editing workload.
- Expected weekly media production and project retention.
- Available budget and local component availability.
- Required monitor colour accuracy and HDR capabilities.
- Existing network infrastructure and cloud-storage entitlements.
- The organization's backup, retention, and data-security requirements.

The initial hardware profile is provisional. The final recommendation will be updated if the evidence indicates that a different configuration is more appropriate.

Pricing is subject to change and must be verified at the time of assessment.

---

## 📖 Full Lab Documentation

The detailed assessment, official requirements research, compatibility validation, cost comparison, supporting evidence, and final recommendation will be documented in the project Wiki.

**Wiki documentation:** To be published after the project assessment has been completed.

---

## 🔎 Expected Outcome

At the end of this project, IT Support should have a documented and defensible workstation recommendation that:

- Addresses the employee's role-specific requirements.
- Aligns with the relevant official software requirements.
- Demonstrates hardware compatibility.
- Balances performance, cost, and future scalability.
- Provides a practical storage, network, and backup strategy.
- Defines a repeatable provisioning and acceptance process.
- Supports a management decision based on documented evidence.

The project demonstrates the ability to translate business requirements into a practical IT infrastructure recommendation while avoiding unnecessary expenditure and unsupported technical assumptions.

---

## 📚 References

- [Adobe Premiere Pro Technical Requirements](https://helpx.adobe.com/br/premiere/desktop/get-started/technical-requirements/adobe-premiere-pro-technical-requirements.html)
- [Adobe Processor, Memory, and GPU Recommendations](https://helpx.adobe.com/br/premiere/desktop/get-started/technical-requirements/processor-memory-and-gpu-recommendations.html)
- [Microsoft Windows 11 Specifications and System Requirements](https://www.microsoft.com/windows/windows-11-specifications)

Additional manufacturer documentation and pricing sources will be added as candidate components are evaluated.

---

## 📝 Lessons Learned

To be completed after the requirements assessment, compatibility analysis, and cost comparison.

The final review will document the main technical findings, purchasing trade-offs, limitations, and improvements identified during the project.
