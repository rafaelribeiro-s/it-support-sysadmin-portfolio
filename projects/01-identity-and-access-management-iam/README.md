# Lab 01: Identity and Access Management (IAM) — Local User Provisioning & Least Privilege

## 📌 Executive Summary
This lab simulates a new employee onboarding request within a fictional enterprise environment.

The objective is to provision a local Windows user account, assign the appropriate account type, apply the principle of least privilege, and validate that administrative privileges are not granted unnecessarily.

The lab uses **Windows 11 Enterprise** running in **Oracle VirtualBox** and focuses on endpoint-level identity and access control.

---

## 🎯 Objectives & Scope
* Local Windows user provisioning
* Standard user account configuration
* Administrative privilege restriction
* Least Privilege Principle (PoLP)
* Basic account and group membership verification
* Windows privacy and application permission review
* Administrative elevation validation
* Technical evidence collection and documentation

### Out of Scope

The following technologies are intentionally outside the scope of this lab:

* Active Directory Domain Services
* Domain Controllers
* Microsoft Entra ID
* Centralized identity federation
* Multi-Factor Authentication (MFA)
* Enterprise-wide RBAC implementation

These capabilities are planned as future extensions of the portfolio.

---

## 🏢 Simulated Enterprise Scenario
* **Company:** NexaCorp Solutions Ltd.
* **Department:** Marketing & Growth
* **Ticket:** ``INC-804291``
* **Workstation:** ``NX-WS-MKT04``
* **Employee:** Sarah Jenkins
* **Username:** ``s.jenkins``

The complete business scenario, implementation procedure, validation evidence, and lessons learned are documented in the project Wiki.

---

## 🛠️ Skills & Technologies Applied
* **Identity:** Local Windows User Management
* **Access Control:** Standard User Configuration, Least Privilege
* **Endpoint:** Windows 11 Enterprise
* **Virtualization:** Oracle VirtualBox
* **Administration:** Windows Settings, Command Prompt
* **Validation:** ``whoami``, ``whoami /groups``, privilege verification
* **Documentation:** Technical Evidence, Troubleshooting, Lessons Learned

---

## 📖 Full Lab Documentation
The complete step-by-step walkthrough, command-line operations, execution logs, and configuration screenshots are fully documented in the repository Wiki:

* 📖 [Full Lab Guide — IAM User Provisioning & Access Control Wiki]([https://github.com/rafaelribeiro-s/it-support-sysadmin-portfolio/wiki/01-%E2%80%94-Identity-and-Access-Management](https://github.com/rafaelribeiro-s/it-support-sysadmin-portfolio/wiki/01-%E2%80%94-Identity-and-Access-Management-(IAM)-%E2%80%94-Local-User-Provisioning-&-Least-Privilege#-enterprise-environment-context)

---

## 🔎 Key Outcome
The final configuration provides Sarah Jenkins with a dedicated local Windows account operating as a **Standard User**, while administrative privileges remain restricted to authorized administrative accounts.

The implementation demonstrates how endpoint-level access controls can reduce unnecessary privileges and support a least-privilege security model.
