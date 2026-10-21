# Lab 07: Disk Management & Storage Partitioning — Disk Management, Partitioning, File Systems, and Storage Validation

## 📌 Executive Summary

This lab documents a removable storage management task within a simulated enterprise Windows environment.

The objective is to demonstrate a structured IT support process for identifying a physical storage device, planning partition capacity, selecting appropriate file systems, configuring volume labels, and validating the resulting storage layout.

The lab uses **Windows 11**, the native **Disk Management** utility, and a **SanDisk Ultra USB 3.0 flash drive marketed as 32 GB**.

The proposed storage configuration divides the USB drive into three logical volumes dedicated to images and videos, applications, and documents. Each volume receives a different capacity allocation based on its intended use.

The initial design allocates 16 GB to Images & Videos, 10 GB to Applications, and 6 GB to Documents. exFAT is proposed for multimedia storage, while NTFS is proposed for applications and documents intended primarily for Windows environments.

The lab emphasizes safe disk identification, data protection before destructive operations, storage capacity planning, file system selection, volume configuration, and post-configuration validation.

The project documents a practical storage management procedure using a physical USB device. It does not claim enterprise storage deployment, data recovery testing, or hardware reliability certification.

---

## 🎯 Objectives & Scope

This lab demonstrates the following IT support and Windows storage management practices:

* Identify a physical USB storage device using its reported capacity, device information, and existing volume layout.
* Inspect the current storage configuration using Windows Disk Management.
* Apply data protection precautions before deleting existing volumes or formatting the device.
* Plan storage capacity according to the expected requirements of different content categories.
* Create three logical volumes with different capacity allocations.
* Select appropriate file systems based on file size requirements and compatibility considerations.
* Configure descriptive volume labels and record the assigned drive letters.
* Verify volume capacities, file systems, partition layout, and accessibility.
* Document the technical rationale behind the selected partition sizes.
* Capture screenshots demonstrating the configuration and validation process.
* Record actual results, implementation differences, and troubleshooting observations.
* Establish a repeatable procedure for preparing and validating removable storage.

### Planned Partition Layout

| **Volume** | **Planned Capacity** | **Allocation** | **File System** | **Intended Purpose** |
|:---|---:|---:|:---|:---|
| Images & Videos | 16 GB | 50% | exFAT | Photographs, videos, and multimedia assets |
| Applications | 10 GB | 31.25% | NTFS | Software installers and technical utilities |
| Documents | 6 GB | 18.75% | NTFS | Technical documentation and office files |
| **Total** | **32 GB** | **100%** | | |

The capacity allocation represents the initial design based on the manufacturer's nominal capacity. Windows currently reports approximately 28.6 GB of available capacity on the connected device. The actual volume sizes will be adjusted to the capacity reported by Disk Management, and the final values will be recorded after implementation.

### Storage Allocation Rationale

**Images & Videos — 16 GB**

The largest allocation is assigned to multimedia content because high-resolution photographs, video recordings, and screen captures can consume substantial storage space.

The exFAT file system supports files larger than 4 GiB and offers broad compatibility with modern operating systems and devices.

Intended content includes:

* Digital photographs and image assets.
* Video recordings and screen captures.
* Multimedia resources used in technical documentation.
* Other large media files.

**Applications — 10 GB**

This volume is intended for Windows software installers, portable utilities, and diagnostic tools. The allocation supports a practical collection of IT support resources while reserving the largest portion of the drive for multimedia content.

NTFS is selected for its support for large files and Windows-oriented storage features.

Intended content includes:

* Windows application installers (`.exe` and `.msi`).
* Portable diagnostic utilities.
* System administration tools.
* Software packages and associated verification files.

**Documents — 6 GB**

This volume is dedicated to technical documentation, reference materials, and office files.

NTFS provides suitable storage for a Windows-oriented workflow, including support for access permissions and journaling.

Intended content includes:

* PDF reference materials.
* Word documents and spreadsheets.
* Technical reports and operating procedures.
* Checklists, inventories, and project documentation.

The proposed allocation is a planning decision based on the simulated use case rather than measured storage consumption.

### Out of Scope

* Data recovery or restoration of deleted partitions.
* Advanced physical storage diagnostics or hardware failure analysis.
* Storage performance benchmarking.
* BitLocker implementation or other encryption deployment.
* Creation of bootable operating system installation media.
* RAID, NAS, SAN, or enterprise storage infrastructure deployment.
* Third-party partition management tools.
* PowerShell-based storage automation.
* Enterprise backup platform implementation.
* Secure data sanitization and forensic data recovery.
* Claims of completed validation before the practical exercise has been performed.

---

## 🏢 Simulated Enterprise Scenario

* **Company:** NexaCorp Solutions Ltd.
* **Industry:** IT Services and Digital Operations
* **Department:** IT Support & Systems Administration
* **Workstation:** `NX-WS-IT07`
* **Requester:** IT Support Department
* **Assigned Analyst:** Rafael Ribeiro
* **Ticket:** `SR-807014`
* **Request Type:** Removable Storage Preparation
* **Operating System:** Windows 11
* **Storage Device:** SanDisk Ultra USB 3.0
* **Nominal Capacity:** 32 GB

The IT Support department requires a reusable USB storage device for organizing multimedia assets, Windows software installers, diagnostic utilities, and technical documentation.

The technician has been assigned to prepare the device using a structured partitioning and formatting procedure.

The proposed configuration separates the storage into three volumes: Images & Videos, Applications, and Documents. Each volume receives a capacity allocation based on its expected workload and a file system selected according to its intended purpose.

Before modifying the device, the technician must verify its identity, confirm that required data has been backed up, and ensure that the selected disk is not the workstation's internal system drive.

After configuration, the technician must validate the partition layout, verify the volume properties, and confirm that all three volumes are accessible through Windows File Explorer.

The procedure and its results will be documented to support reproducibility, troubleshooting, and future storage preparation tasks.

For this lab, the scenario is simulated for educational and portfolio purposes. The project demonstrates a structured storage management workflow; it does not represent an actual enterprise service ticket or a deployment performed for a real organization.

---

## 🛠️ Skills & Technologies Applied

* IT Support and Windows Systems Administration
* Removable Storage Management
* Windows 11 Disk Management
* Physical Disk Identification and Verification
* Partition Planning and Capacity Allocation
* Volume Creation and Formatting
* File System Selection: exFAT and NTFS
* Volume Labeling and Drive Letter Assignment
* Storage Capacity Verification
* File Explorer Storage Validation
* Data Protection Before Destructive Operations
* File System Compatibility Assessment
* Storage Troubleshooting
* Technical Documentation and Evidence Collection
* Operational Procedure Development
* Configuration Validation and Acceptance Criteria

---

## 🔐 Technical Controls Demonstrated

The lab focuses on operational controls that reduce the risk of accidental data loss and improve the reliability of removable storage configuration.

### Device Identification and Verification

The target USB drive must be identified using its reported capacity, device information, and existing partition layout.

The technician must verify that the selected disk corresponds to the intended SanDisk USB device before performing destructive operations.

Drive letters alone are insufficient for identification because Windows can assign different letters when devices are reconnected.

### Data Protection Before Partitioning

Important files must be backed up to another suitable storage location before existing volumes are deleted or the device is reformatted.

The backup must be verified before proceeding with destructive operations.

This control reduces the risk of accidental data loss but does not guarantee recovery if the backup itself is incomplete or inaccessible.

### Storage Capacity Planning

The partition layout is planned according to the expected storage requirements of each content category.

The initial allocation assigns 16 GB to multimedia files, 10 GB to applications, and 6 GB to documents.

The rationale considers typical file sizes and intended usage rather than assuming that all categories require equal capacity.

The final configuration must be adjusted to the actual capacity reported by Windows.

### File System Selection

The proposed design uses exFAT for Images & Videos and NTFS for Applications and Documents.

exFAT is selected for multimedia storage because it supports large files and provides broad compatibility with modern systems.

NTFS is selected for the Windows-oriented application and document volumes because it supports large files, journaling, and access control features.

The choice of file systems reflects the simulated use case. Compatibility requirements must be reconsidered if the device will be used with older systems or specialized equipment.

### Volume Labeling and Identification

Each partition receives a descriptive label to distinguish its intended purpose.

The labels `Images & Videos`, `Applications`, and `Documents` support easier identification in Disk Management and File Explorer.

Drive letters are recorded during validation rather than assumed in advance.

### Post-Configuration Validation

The completed layout must be inspected in Disk Management to confirm that all three volumes exist and use the expected file systems.

File Explorer is used to verify that the volumes are visible and accessible.

Actual capacities, drive letters, volume labels, and any deviations from the planned layout must be recorded.

Where appropriate, a small test file can be created and removed to confirm basic write access.

### Operational Limitations and Data Protection

Partitioning creates separate logical volumes on a single physical device. It does not provide physical redundancy, independent failure domains, or a backup mechanism.

If the USB drive is lost or fails, all three volumes may become inaccessible.

Quick formatting is not equivalent to secure data sanitization. Sensitive information must be handled according to applicable organizational data protection and sanitization procedures.

### Evidence-Based Documentation

Screenshots will be collected to demonstrate the relevant stages of the practical exercise, including device identification, unallocated space, volume configuration, the final partition layout, and File Explorer validation.

The documentation will distinguish the planned configuration from the actual results and will record any limitations encountered during execution.

---

### 📖 Full Lab Documentation

The complete practical walkthrough, including the lab environment, device identification, partition preparation, volume creation, file system configuration, storage allocation rationale, implementation evidence, troubleshooting, lessons learned, and final validation results, will be documented in the project Wiki.

* 📖 [Full Lab Guide — Disk Management & Storage Partitioning Wiki](https://github.com/rafaelribeiro-s/it-support-sysadmin-portfolio/wiki/07-%E2%80%94-Disk-Management-and-Storage-Partitioning)

---

## 🔎 Expected Outcome

At the end of the lab, the project documentation should demonstrate a structured approach to preparing and validating a removable USB storage device in Windows 11.

The documentation should demonstrate that:

* The SanDisk USB device was identified before destructive operations.
* The reported capacity and existing volume configuration were recorded.
* Data protection precautions were considered before modifying existing volumes.
* A three-volume storage layout was planned according to the intended workload.
* The capacity allocation was justified for multimedia files, applications, and documents.
* The Images & Videos volume was configured with exFAT, subject to successful implementation.
* The Applications and Documents volumes were configured with NTFS, subject to successful implementation.
* Descriptive volume labels and actual drive letters were recorded.
* The final partition layout and actual capacities were verified in Disk Management.
* File Explorer was used to confirm volume visibility and accessibility.
* Screenshots and technical observations were collected as supporting evidence.
* Differences between the planned and actual configuration were documented.
* Operational safety, file system limitations, and data protection considerations were addressed.
