# Lab 06: Hardware Upgrade & Troubleshooting Case — Hardware Diagnostics, Root Cause Analysis, Component Upgrades & Post-Upgrade Validation

## 📌 Executive Summary

This lab documents a hardware troubleshooting and performance optimization case within a simulated IT support environment.

The objective is to demonstrate a structured troubleshooting process for identifying hardware-related performance limitations, analyzing system resource utilization, determining a likely root cause, applying corrective actions, and validating the resulting configuration.

The case focuses on a Windows workstation experiencing performance degradation during multitasking activities involving Microsoft Excel, Microsoft Teams, and Microsoft Edge.

The initial investigation identified limited memory capacity as the primary suspected bottleneck. The original case documented approximately 87–90% memory utilization with 4 GB of allocated RAM. The corrective actions included system maintenance and increasing the virtual machine's allocated memory to 8 GB.

The post-change report recorded lower memory utilization and improved system responsiveness. These observations are documented as results from the original case and are not presented as independently reproduced benchmark results.

This lab reorganizes the existing troubleshooting case into the standardized structure of the IT Support & Systems Administration portfolio. It emphasizes evidence-based diagnosis, root cause analysis, corrective action, post-change validation, and technical documentation.

The project documents a virtualized workstation resource upgrade rather than a physical RAM installation.

---

## 🎯 Objectives & Scope

This lab demonstrates the following IT support and troubleshooting practices:

* Document the initial workstation hardware and operating system configuration.
* Assess reported performance symptoms and the affected business workload.
* Collect baseline information about CPU, memory, storage, and system behavior.
* Identify the most likely hardware resource bottleneck using available measurements.
* Perform documented system maintenance as a supplementary corrective action.
* Increase the memory allocated to a virtual workstation from 4 GB to 8 GB.
* Compare recorded resource utilization before and after the intervention.
* Validate the resulting virtual machine configuration.
* Distinguish the primary root cause from secondary maintenance activities.
* Document corrective actions, technical observations, and preventive recommendations.
* Organize screenshots and supporting material using a consistent evidence structure.
* Produce a clear troubleshooting report suitable for an IT support portfolio.

### Out of Scope

* Physical workstation assembly or physical RAM installation
* Replacement of the host computer's physical memory
* Claims of independently reproduced performance benchmarks
* Enterprise-wide hardware procurement
* Active Directory or Group Policy implementation
* Microsoft Intune or centralized endpoint deployment
* BIOS or firmware updates not documented in the original case
* CPU or GPU replacement
* Enterprise monitoring platform deployment
* Claims that every possible CPU, storage, or application bottleneck has been ruled out
* Claims that system maintenance alone resolved the reported performance issues
* Performance improvements beyond those supported by the available evidence

---

## 🏢 Simulated Enterprise Scenario

* **Company:** NexaLog Logistics
* **Department:** Operations
* **Employee Role:** Business Operations Employee
* **Primary Workload:** Microsoft Excel, Microsoft Teams, and Microsoft Edge
* **Virtualization Platform:** Oracle VirtualBox
* **Guest Operating System:** Windows 10 Home, 64-bit
* **OS Build:** 19045
* **Initial Allocated Memory:** 4 GB RAM
* **Target Allocated Memory:** 8 GB RAM
* **Virtual CPU Allocation:** 2 vCPUs
* **Reported CPU:** AMD Ryzen 7 1700X
* **Virtual Storage:** 80 GB
* **Case Type:** Hardware Resource Troubleshooting and Virtual Machine Upgrade

An employee reported significant system slowdowns and intermittent freezes while working with large Excel spreadsheets, participating in Teams calls, and keeping multiple Edge tabs open.

IT Support was assigned to investigate the workstation's resource utilization and determine whether the existing configuration could support the employee's multitasking workload.

The initial assessment focused on available memory, CPU utilization, and storage capacity. The original case recorded high memory utilization while multiple applications were running, suggesting that the available 4 GB of RAM was insufficient for the observed workload.

The corrective plan included supplementary system maintenance and an increase in the virtual machine's allocated memory to 8 GB.

The original service report recorded improved memory availability and responsiveness after the change. The final portfolio documentation will preserve the available evidence and distinguish recorded observations from conclusions and recommendations.

For this lab, the scenario is documented for educational and portfolio purposes. The project describes the original troubleshooting case and does not claim that a new physical workstation was assembled or upgraded.

The complete diagnostic process, root cause assessment, corrective actions, validation results, and supporting screenshots will be documented in the project Wiki.

---

## 🛠️ Skills & Technologies Applied

* IT Support and Hardware Troubleshooting
* Hardware Inventory and Configuration Assessment
* Windows 10 Administration
* Oracle VirtualBox
* Virtual Machine Resource Allocation
* CPU and Memory Utilization Analysis
* Performance Baseline Assessment
* Root Cause Analysis
* PowerShell-Based System Maintenance
* Memory Capacity Planning
* Before-and-After Configuration Comparison
* Post-Change Validation
* Technical Evidence Collection
* IT Service Ticket Documentation
* Troubleshooting Methodology
* Preventive Maintenance Recommendations
* Evidence-Based Technical Reporting

---

## 🔐 Technical Controls Demonstrated

The lab focuses on identifying a resource bottleneck, applying a targeted corrective action, and validating the resulting configuration.

### Workload and Symptom Assessment

Workload and Symptom Assessment

The investigation begins with the reported symptoms and the applications used during normal business activities.

The workload includes large Excel spreadsheets, Teams calls, and multiple Edge tabs. These applications can compete for memory when used simultaneously.

The assessment uses this workload as the context for evaluating resource utilization rather than assuming that a single hardware component is responsible before collecting evidence.

Hardware and System Inventory

The initial configuration is documented to establish the workstation's baseline.

The inventory includes the operating system, processor information, virtual CPU allocation, available memory, and virtual storage configuration.

This information provides the context required to interpret the performance observations and document the change applied during troubleshooting.

### Baseline Performance Assessment

The original case recorded memory utilization of approximately 87–90% while the employee's multitasking workload was active.

With 4 GB of allocated RAM, this indicated limited memory headroom and supported further investigation into memory pressure.

The recorded percentage is treated as an observation from the original case. It does not independently establish that memory was the only possible cause of every reported freeze.

### Root Cause Analysis

The working root cause was insufficient memory capacity for the observed multitasking workload.

The diagnosis was based on the combination of reported symptoms, the initial 4 GB memory allocation, and the recorded high memory utilization.

CPU and storage resources were also considered during the investigation. The available evidence did not identify them as the primary bottleneck in the original report.

The conclusion is therefore limited to the most likely root cause supported by the recorded observations.

### System Maintenance

The original case documented a PowerShell-based cleanup of selected temporary and maintenance-related directories.

This activity was treated as a supplementary maintenance measure intended to address unnecessary temporary files where appropriate.

Temporary-file cleanup does not directly increase physical RAM or the memory allocated to a virtual machine. It is therefore documented separately from the memory-capacity change.

Any cleanup commands and their effects will be described according to the original evidence.

### Memory Capacity Upgrade

The original case documented an increase in allocated memory from 4 GB to 8 GB.

Because the environment uses Oracle VirtualBox, the change represents an adjustment to the virtual machine's configured memory allocation.

The configuration change is intended to provide more memory headroom for concurrent applications and reduce the likelihood of memory pressure under the observed workload.

The documentation does not describe this action as a physical RAM installation.

### Post-Upgrade Validation

The original service report recorded approximately 55% memory utilization after the memory allocation was increased.

It also recorded approximately 4.4 GB of memory in use and 3.6 GB available in the reported post-change state.

These figures are retained as observations from the original report and will be checked against the corresponding screenshots during evidence organization.

The results suggest improved memory headroom. A controlled test using the same applications and workload before and after the change would provide stronger evidence of the magnitude of the performance improvement.

### Configuration and Evidence Verification

The final evidence review will confirm that the documented initial and resulting configurations match the screenshots.

The evidence should distinguish between:

* Initial hardware and operating system information
* Baseline resource utilization
* Observations supporting the root cause
* Documented maintenance activities
* The virtual machine memory allocation change
* Post-change resource utilization and configuration

This separation helps ensure that each technical conclusion is supported by relevant evidence.

### Preventive Recommendations

The case supports several practical recommendations:

* Monitor memory utilization when investigating recurring performance issues.
* Close unnecessary applications and browser tabs when appropriate.
* Evaluate resource requirements against the employee's actual workload.
* Review virtual machine resource allocations when performance limitations persist.
* Use supported Windows maintenance methods rather than relying on indiscriminate file deletion.
* Record baseline and post-change measurements during future troubleshooting.
* Reassess CPU, storage, and application behavior if performance issues continue after the memory change.

### Evidence-Based Documentation

The project will use screenshots from the original service report to support the diagnostic process and resulting configuration.

Each evidence item will have a unique identifier, a descriptive filename, and a caption explaining what it demonstrates.

The report will distinguish between recorded measurements, diagnostic conclusions, corrective actions, and recommendations. This approach avoids presenting assumptions as confirmed technical facts.

---

## 📖 Full Lab Documentation

The complete troubleshooting case, initial hardware inventory, baseline performance observations, root cause analysis, corrective actions, memory allocation change, post-upgrade validation, and supporting screenshots will be documented in the project Wiki.

* 📖 [Full Lab Guide — Hardware Upgrade & Troubleshooting Case Wiki](https://github.com/rafaelribeiro-s/it-support-sysadmin-portfolio/wiki/06-%E2%80%94-Hardware-Upgrade-and-Troubleshooting--%E2%80%94-Hardware-Diagnostics)

---

## 🔎 Expected Outcome

At the end of the lab documentation, the project should provide a structured record of the troubleshooting investigation and the corrective actions documented in the original case.

The documentation should demonstrate that:

* The initial workstation configuration was recorded.
* The employee's performance symptoms and multitasking workload were documented.
* Baseline memory utilization was assessed.
* A likely memory-capacity bottleneck was identified from the available observations.
* Supplementary system maintenance was documented separately from the primary corrective action.
* The virtual machine's allocated memory was increased from 4 GB to 8 GB.
* Post-change resource utilization was recorded and compared with the initial observations.
* The validation results were linked to the corresponding screenshots.
* The diagnostic conclusion was limited to what the available evidence supports.
* Preventive recommendations were identified for future workstation troubleshooting.
* The report distinguishes virtual machine resource allocation from physical hardware installation.

The final report will distinguish between the original case's recorded results, the interpretation of those results, and any additional validation that would be required to reproduce the performance comparison under controlled conditions.

**Final recommendation:** Retain the documented 8 GB virtual machine memory configuration as the corrective configuration recorded in this case, subject to the available validation evidence and the workload's ongoing resource requirements.
