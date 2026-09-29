# Lab 03: Software Deployment & Integrity Verification — Safe and Guided Software Installation

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

### Out of Scope

* Enterprise software licensing or procurement
* Microsoft Intune or other centralized software deployment platforms
* Active Directory/GPO-based software deployment
* Automated deployment through SCCM/MECM
* Software packaging or repackaging
* Enterprise application lifecycle management
* Production endpoint deployment
* Application vulnerability assessment or penetration testing
* Source-code auditing of GIMP
* Reverse engineering of the installer

---

## 🏢 Simulated Enterprise Scenario

* **Company:** NexaCorp Solutions Ltd.
* **Industry:** Cloud Financial Services
* **Department:** Creative & Brand
* **Workstation:** `NX-WS-CRT03`
* **Employee:** Olivia Bennett
* **Username:** `o.bennett`
* **Job Title:** Graphic Designer
* **Ticket:** `INC-804512`

The Creative & Brand team requires an approved image-editing application for work-related design activities on workstation `NX-WS-CRT03`.

As part of the organization's endpoint security and software deployment procedures, the requested application must be obtained from an official and trusted source, verified for file integrity, scanned for potential security threats, and installed using only the required components and appropriate installation scope.

For this lab, **GIMP (GNU Image Manipulation Program)** is used as the approved software package to demonstrate the controlled deployment process.

The complete business scenario, software acquisition procedure, integrity verification, installation evidence, validation results, troubleshooting activities, and lessons learned are documented in the project Wiki.

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

## 📖 Full Lab Documentation

The complete hands-on procedure, verification evidence, screenshots, command-line operations, troubleshooting records, and lessons learned are documented in the project Wiki.

* 📖 [Full Lab Guide — Software Deployment & Integrity Verification Wiki](https://github.com/rafaelribeiro-s/it-support-sysadmin-portfolio/wiki/03-%E2%80%94-Software-Deployment-&-Integrity-Verification-%E2%80%94-Safe-and-Guided-Software-Installation)

---

## 🔎 Expected Outcome

At the end of the lab, the approved GIMP installation should be successfully deployed and validated on the Windows workstation.

The documentation should provide evidence that the installer:

* Came from a trusted source.
* Matched the vendor-published integrity value.
* Was checked for security detections.
* Was installed using appropriate configuration choices.
* Did not introduce unnecessary components.
* Was successfully validated after deployment.

