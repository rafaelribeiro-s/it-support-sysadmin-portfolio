
# Lab 05: Hardware Provisioning & Video Editing Workstation — Workstation Requirements and Hardware Selection

## 📌 Executive Summary

This lab documents a hardware provisioning and workstation specification task within a simulated enterprise Windows environment.

The objective is to demonstrate a structured IT support process for assessing business requirements, identifying software and hardware constraints, selecting suitable workstation components, planning storage capacity, and documenting a recommended configuration for a demanding video editing workload.

The lab uses **Adobe Premiere Pro**, **Windows 11 Pro**, and published manufacturer specifications to support the proposed workstation design.

The recommended configuration targets 4K video editing, high-resolution graphics, local NVMe media storage, and access to shared company storage through a 10 Gigabit Ethernet connection.

The configuration is documented as a requirements-based IT support recommendation rather than as a completed physical deployment or benchmarked workstation.

---

## 🎯 Objectives & Scope

This lab demonstrates the following IT support and workstation provisioning practices:

* Assess business and application requirements for a dedicated video editing workstation.
* Review Adobe Premiere Pro's published hardware and storage recommendations.
* Consider Windows 11 hardware compatibility and supported processor requirements.
* Select a suitable CPU, GPU, memory configuration, motherboard, storage devices, power supply, cooling solution, and display.
* Separate operating system storage from active media storage.
* Estimate storage capacity requirements based on incoming media volume.
* Evaluate the need for 10 Gigabit Ethernet in a shared 4K media workflow.
* Define a controlled workflow for active projects, approved deliverables, and revisions.
* Document data retention, backup, and recovery considerations.
* Establish procurement checks and future deployment acceptance criteria.
* Collect official vendor documentation as supporting evidence.
* Present a clear hardware recommendation with documented technical justification.

### Out of Scope

* Physical workstation assembly or deployment
* Claims of completed hardware testing or performance benchmarking
* Enterprise-wide hardware procurement
* Active Directory or Group Policy implementation
* Microsoft Intune or centralized endpoint deployment
* NAS installation or enterprise storage infrastructure implementation
* Enterprise backup platform configuration
* Actual production media migration
* Adobe Premiere Pro performance benchmarking
* HDR production workflow
* GPU overclocking or performance tuning
* Numerical procurement budget or supplier price comparison
* Claims that planned acceptance tests have already passed

---

## 🏢 Simulated Enterprise Scenario

* **Company:** NexaCorp Solutions Ltd.
* **Industry:** Cloud Financial Services
* **Department:** Marketing & Growth
* **Workstation:** `NX-WS-MKT05`
* **Employee:** John Mitchell
* **Username:** `j.mitchell`
* **Employee ID:** `NX-9052`
* **Job Title:** Video Editor
* **Reporting Manager:** Anita Roberts
* **Ticket:** `SR-805217`
* **Primary Application:** Adobe Premiere Pro
* **Operating System:** Windows 11 Pro

The Marketing & Growth department requires a dedicated workstation for editing 4K video and high-resolution graphics.

The employee receives approximately 500 GB of incoming media per week. Active projects may remain in progress for several days or up to approximately two weeks.

The intended workflow uses local NVMe storage for active editing and the company's designated NAS or file server for approved project packages and deliverables.

IT Support has been assigned to assess the workload and document a hardware configuration that provides sufficient processing capacity, memory, GPU resources, local storage, and network connectivity.

The proposed workstation includes an Intel Core Ultra 7 265K processor, an NVIDIA GeForce RTX 5070 12 GB graphics card, 64 GB of DDR5 memory, separate system and media NVMe SSDs, and a compatible 10 GbE network adapter.

The hardware selection is supported by published Adobe, Microsoft, and manufacturer documentation. Exact component compatibility and availability remain subject to procurement review.

For this lab, the scenario is simulated for educational and portfolio purposes. The project demonstrates a structured hardware provisioning and specification workflow; it does not claim that a physical workstation has been assembled, deployed, or tested.

The complete business scenario, workload assessment, hardware selection, storage planning, operational workflow, acceptance criteria, and supporting evidence will be documented in the project Wiki.

---

## 🛠️ Skills & Technologies Applied

* IT Support and Hardware Provisioning
* Workstation Requirements Assessment
* Enterprise Endpoint Planning
* Windows 11 Compatibility Review
* Adobe Premiere Pro System Requirements
* CPU and GPU Specification Analysis
* Memory Capacity Planning
* NVMe Storage Planning
* Media Storage Capacity Calculations
* Network Storage Requirements
* 10 Gigabit Ethernet Planning
* Hardware Compatibility Review
* Data Retention and Backup Considerations
* Procurement Documentation
* Technical Research and Vendor Documentation
* Acceptance Criteria Definition
* Evidence-Based Technical Documentation
* IT Asset and Configuration Planning

---

## 🔐 Technical Controls Demonstrated

The lab focuses on requirements-based hardware selection and operational controls that support a reliable workstation for professional video editing.

### Workload and Requirements Assessment

The employee's editing workload is assessed before selecting hardware. The assessment considers 4K source media, high-resolution graphics, application requirements, weekly media intake, project duration, and shared storage needs.

### CPU and GPU Selection

The proposed CPU and GPU are evaluated against the requirements of a demanding editing workload.

The selected NVIDIA GeForce RTX 5070 provides 12 GB of GPU memory, exceeding Adobe's published 8 GB recommendation for 4K and higher-resolution work.

The processor and graphics card are selected as a balanced workstation configuration rather than as isolated components.

### Memory Capacity Planning

The workstation is specified with 64 GB DDR5 memory.

This exceeds Adobe's published recommendation of 32 GB or more for 4K work and provides additional capacity for application activity, larger projects, and multitasking.

### Storage Separation

The proposed design separates the operating system and application drive from the active media drive.

The 1 TB system SSD is intended for Windows and applications, while the 4 TB media SSD is intended for active project files and source media. The media cache should use fast local storage.

This arrangement supports a clearer separation of operating system activity and media workloads.

### Media Capacity Planning

The storage assessment uses an estimated incoming media volume of 500 GB per week.

The calculations demonstrate how quickly media requirements can grow and why active local storage must be managed through an approved project transfer and retention workflow.

The 4 TB media SSD is intended for active work rather than indefinite storage of all incoming media.

### Network Storage Planning

The proposed workstation includes a PCIe 10 GbE network adapter to support the intended shared 4K storage workflow.

The motherboard's integrated network connection is 2.5 GbE, so a separate adapter is included in the recommendation.

The NAS, switch, cabling, and network configuration must also support 10 GbE. The adapter alone does not guarantee a particular file transfer speed.

### Project Transfer and Integrity

Approved project packages should be transferred to the designated NAS or file server.

The destination must be checked before eligible local copies are removed. File counts, sizes, checksums where appropriate, and successful destination access can be used to support verification.

### Data Retention and Recovery

The workflow distinguishes between active local media, approved shared deliverables, and organizational backups.

A NAS is not automatically a backup. Backup coverage, retention periods, recovery procedures, and access permissions must be defined separately.

### Procurement and Compatibility Review

The selected components must be checked for CPU socket support, firmware requirements, memory compatibility, GPU dimensions, cooler and case clearance, power connectors, SSD installation requirements, and PCIe expansion availability.

This review is required before purchase and physical assembly.

### Evidence-Based Documentation

Official vendor documentation will be used to support the hardware selection.

Screenshots of the relevant Adobe, Microsoft, NVIDIA, and motherboard specification pages will document the requirements behind the proposed configuration.

The documentation will distinguish published specifications from physical test results and planned acceptance checks.

---

### 📖 Full Lab Documentation

The complete workstation provisioning case study, workload assessment, recommended hardware configuration, storage calculations, project management workflow, compatibility considerations, acceptance criteria, and supporting evidence will be documented in the project Wiki.

* 📖 [Full Lab Guide — Hardware Provisioning & Video Editing Workstation Wiki](https://github.com/rafaelribeiro-s/it-support-sysadmin-portfolio/wiki)

---

## 🔎 Expected Outcome

At the end of the lab documentation, the project should provide a justified workstation recommendation for the Marketing & Growth department.

The documentation should demonstrate that:

* The employee's workload and business requirements were identified.
* Adobe Premiere Pro's published 4K requirements were reviewed.
* Windows 11 processor support was considered.
* A CPU, GPU, memory, motherboard, storage, power supply, cooling solution, and monitor were selected.
* Separate system and active media storage were incorporated into the design.
* Incoming media capacity was estimated using the 500 GB per week workload.
* 10 GbE connectivity was included for the intended shared-storage workflow.
* Project approval, transfer verification, revision handling, and local copy retention were documented.
* Backup and recovery were treated as separate data protection requirements.
* Procurement compatibility checks and future acceptance criteria were defined.
* Official vendor documentation was identified as supporting evidence.

The final report will distinguish between the proposed hardware configuration, published manufacturer specifications, and validation activities that would need to be performed during physical deployment.

**Final recommendation:** Proceed with the documented configuration as the proposed workstation baseline for procurement review.
