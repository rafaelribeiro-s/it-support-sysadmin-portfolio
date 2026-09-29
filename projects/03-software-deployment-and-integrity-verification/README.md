# Lab 03: Software Deployment & Integrity Verification

## 📌 Executive Summary

This lab simulates the secure deployment of approved software to an enterprise Windows workstation.

The objective is to demonstrate a controlled software installation process that incorporates trusted software sourcing, installer integrity verification, malware scanning, installation scope assessment, and post-installation validation.

The lab uses **GIMP (GNU Image Manipulation Program)** as the approved software package for the simulated business requirement.

The installation process is documented as an enterprise IT support workflow rather than as a simple application installation.

---

## 🎯 Objectives & Scope

This lab demonstrates the following software deployment and security practices:

* Obtain software from an official and trusted vendor source.
* Identify the correct installer for the target operating system.
* Record the installer version and file metadata.
* Verify the installer SHA-256 hash against the vendor-published value.
* Submit the installer to a malware-scanning service for additional analysis.
* Review installation scope and privilege requirements.
* Review the software license agreement before installation.
* Select only the required installation components.
* Install the approved software using the appropriate installation scope.
* Validate the software installation after deployment.
* Document the evidence collected throughout the process.

---

## 🏢 Simulated Enterprise Scenario

This lab simulates a software deployment request within the fictional organization **NexaCorp Solutions Ltd.**

A business user requires an approved image-editing application for work-related activities.

The IT Support & Systems Administration team is responsible for:

1. Validating the software request.
2. Obtaining the installer from the official vendor source.
3. Verifying installer integrity.
4. Checking the installer for potential security detections.
5. Reviewing installation options.
6. Installing only the required software components.
7. Verifying successful deployment.

The objective is to demonstrate a controlled and auditable software installation process.

---

## 🛠️ Skills & Technologies Applied

* Software Deployment
* Windows Endpoint Administration
* SHA-256 Integrity Verification
* File Hash Verification
* Malware Scanning
* Trusted Software Sources
* Installation Scope Management
* Least Privilege
* Security Validation
* Technical Documentation
* Troubleshooting

---

## 💻 Lab Environment

|        Component        | Configuration                    |
| :---------------------: | :------------------------------- |
| Virtualization Platform | Oracle VirtualBox                |
|  Guest Operating System | Windows 11 Enterprise Evaluation |
|       Architecture      | x64                              |
|       Workstation       | NX-WS-CRT03                      |
|         Software        | GIMP                             |
|     Software Source     | Official GIMP distribution       |
|     Deployment Type     | Local software installation      |


---

## 🔐 Security Controls Demonstrated

The lab focuses on several controls that reduce the risk associated with software deployment:

### Trusted Source

The installer is obtained directly from the official GIMP distribution rather than from an unknown third-party download site.

### Integrity Verification

The installer SHA-256 hash is calculated locally and compared against the value published by the software vendor.

### Malware Analysis

The installer is submitted for additional security analysis before installation.

### Installation Scope

The installation scope is reviewed to determine whether the application should be installed for all users or only for the intended user.

### Component Selection

Installation components are reviewed so that unnecessary software or functionality is not deployed.

### Post-Installation Validation

The completed installation is verified to ensure that the approved application was installed successfully and is operational.

---

## 📖 Documentation

The complete hands-on procedure, verification evidence, screenshots, command-line operations, troubleshooting records, and lessons learned are documented in the project Wiki.

* 📖 [Full Lab Guide — Software Deployment & Integrity Verification Wiki](../../wiki/03-Software-Deployment-and-Integrity-Verification)

---

## 🧠 Expected Outcome

At the end of the lab, the approved GIMP installation should be successfully deployed and validated on the Windows workstation.

The documentation should provide evidence that the installer:

* Came from a trusted source.
* Matched the vendor-published integrity value.
* Was checked for security detections.
* Was installed using appropriate configuration choices.
* Did not introduce unnecessary components.
* Was successfully validated after deployment.

---

## 📋 Evidence Strategy

The Wiki documentation will contain evidence for:

* Workstation baseline.
* Software deployment request.
* Official vendor download source.
* Installer identification.
* SHA-256 hash calculation.
* Vendor hash comparison.
* Malware scanning results.
* Installation scope selection.
* License agreement review.
* Component selection.
* Installation completion.
* Post-installation validation.
* Troubleshooting.
* Lessons learned.

---

## ✅ Final Result

This lab demonstrates a repeatable software deployment workflow that combines operational IT support practices with basic endpoint security controls.

Rather than treating software installation as a simple executable launch, the process demonstrates how an IT support technician can establish software provenance, verify file integrity, assess security risk, control installation scope, and document the final deployment state.
