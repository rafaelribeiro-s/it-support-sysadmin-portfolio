# Lab 02: Endpoint Security — Automatic Screen Lock & Inactivity Policy

## 📌 Executive Summary

This lab simulates an enterprise endpoint security request involving the automatic protection of an unattended Windows workstation.

The objective is to configure and validate an automatic screen lock after a defined period of user inactivity, requiring user authentication before the existing session can be accessed again.

The scenario demonstrates practical endpoint security controls designed to reduce the risk of unauthorized access to an unattended corporate workstation.

---

## 🎯 Objectives & Scope

* Configure an automatic screen lock after one minute of inactivity.
* Require authentication when the workstation session is resumed.
* Validate the configured security behavior through a controlled test.
* Document the implementation and verification evidence.
* Record troubleshooting activities and lessons learned.

This laboratory focuses on workstation-level endpoint security and physical access protection.

### Out of Scope

It does not include centralized Group Policy management, Active Directory, Microsoft Entra ID, or enterprise-wide endpoint management platforms.

---

## 🏢 Simulated Enterprise Scenario

* **Company:** NexaCorp Solutions Ltd.
* **Department:** Finance Operations
* **Ticket:** `INC-804367`
* **Workstation:** `NX-WS-FIN02`
* **Employee:** Daniel Carter
* **Username:** `d.carter`

A Finance Operations workstation is used to access corporate and financial information.

As part of the organization's endpoint security baseline, unattended workstations must automatically enter a protected state after one minute of inactivity and require authentication before the existing user session can be accessed again.

---

## 🛠️ Skills & Technologies Applied

* Windows 11 Enterprise Evaluation
* Oracle VirtualBox
* Endpoint Security
* Workstation Security
* Automatic Screen Lock
* Inactivity Timeout
* Authentication on Resume
* Security Control Validation
* Technical Documentation
* Troubleshooting

---

## 📖 Full Lab Documentation

The complete implementation procedure, configuration evidence, validation tests, troubleshooting records, and lessons learned are documented in the project Wiki:

* 📖 [Full Lab Guide — Endpoint Security & Automatic Screen Lock](https://github.com/rafaelribeiro-s/it-support-sysadmin-portfolio/wiki/02-%E2%80%94-Endpoint-Security-%E2%80%94-Automatic-Screen-Lock-&-Inactivity-Policy)

---

## 🔐 Security Control Demonstrated

The laboratory implements the following security control:

```text
User inactivity
      ↓
1 minute
      ↓
Automatic screen lock
      ↓
User interaction
      ↓
Authentication required
      ↓
Existing session restored
```

The control is validated through both configuration evidence and an observed behavioral test.

---

## 🔎 Key Outcome

At the end of the laboratory:

* The workstation activates the configured screen saver after one minute of inactivity.
* The workstation requires authentication when the user attempts to resume the session.
* The existing user session remains protected while the workstation is unattended.
* Configuration and validation evidence is documented in the project Wiki.
