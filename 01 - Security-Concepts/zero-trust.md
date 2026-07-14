
# Zero Trust Security Model

## What is Zero Trust?

Zero Trust is a modern cybersecurity framework based on a simple principle:

> **"Never trust, always verify."**

Unlike traditional security models that assume everything inside the corporate network is safe, Zero Trust assumes that breaches can happen anywhere — both inside and outside the organization's environment.

Every access request must be continuously validated before access is granted to applications, data, devices, or infrastructure.

---

## Why Zero Trust Matters

Organizations no longer operate exclusively from on-premises networks.

Today, users access company resources from:

- Remote locations
- Personal devices
- Cloud applications
- Mobile devices
- Partner and third-party environments

Because of this, the traditional network perimeter is no longer sufficient.

Modern security focuses on **identity as the new security perimeter**.

---

## Core Principles of Zero Trust

### 1. Verify Explicitly

Always authenticate and authorize access based on all available signals.

Examples:

- User identity
- Device compliance
- Location
- Risk level
- Application sensitivity
- Data classification

**Example:**

Even after logging into a banking application, you may still be required to enter an MFA code before transferring money.

---

### 2. Use Least Privilege Access

Users should receive only the permissions necessary to perform their tasks.

This minimizes the impact of compromised accounts and reduces the attack surface.

Common implementations:

- Role-Based Access Control (RBAC)
- Just-In-Time (JIT) Access
- Just-Enough Access (JEA)

**Example:**

An employee temporarily receives administrative rights only when performing a specific task and loses those permissions immediately afterward.

---

### 3. Assume Breach

Operate under the assumption that attackers may already be present somewhere in the environment.

Security controls should be designed to:

- Minimize blast radius
- Prevent lateral movement
- Detect threats quickly
- Protect sensitive data

Examples:

- Data encryption at rest
- Data encryption in transit
- Network segmentation
- Security monitoring
- Threat detection

---

## Zero Trust Pillars

### Identity

Verify and protect every identity.

Controls include:

- Multi-Factor Authentication (MFA)
- Passwordless Authentication
- Risk-Based Authentication
- Identity Protection

### Devices

Ensure devices are healthy and compliant before granting access.

Controls include:

- Device compliance policies
- Endpoint management
- Security baselines

### Applications

Control how applications are accessed and used.

Controls include:

- Single Sign-On (SSO)
- Application permissions
- Application governance

### Data

Protect sensitive information regardless of where it is stored.

Controls include:

- Encryption
- Data Loss Prevention (DLP)
- Data Classification
- Information Protection

### Infrastructure

Protect servers, cloud resources, and networks.

Controls include:

- Monitoring
- Threat detection
- Vulnerability management
- Network segmentation

---


## Microsoft and Zero Trust

Microsoft implements Zero Trust across its security platform through solutions such as:

- Microsoft Entra ID
- Microsoft Defender
- Microsoft Intune
- Microsoft Purview
- Microsoft Sentinel

These services work together to continuously verify identities, devices, applications, and data across cloud and hybrid environments.

---

## Key Takeaways

✅ Never trust by default

✅ Continuously verify users and devices

✅ Grant the minimum permissions required

✅ Assume attackers may already be inside the environment

✅ Protect identities, devices, applications, data, and infrastructure

✅ Use monitoring and threat detection to quickly identify suspicious activity
