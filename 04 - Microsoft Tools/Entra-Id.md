# Microsoft Entra ID

## Overview

Microsoft Entra ID is Microsoft's cloud-based identity and directory service. It acts as a centralized platform for managing identities, groups, applications, and devices across cloud and hybrid environments.

Formerly known as Azure Active Directory (Azure AD), Microsoft Entra ID is a core component of Microsoft's identity and access ecosystem and serves as the identity backbone for services such as Microsoft 365, Azure, Dynamics 365, and thousands of third-party applications.

---

## Core Components

### Users

Users represent identities within a tenant.

Typical user categories include:

- Internal employees
- Contractors
- External collaborators
- Service accounts

User objects contain attributes such as:

- Display name
- User Principal Name (UPN)
- Email address
- Department
- Job title

---

### Groups

Groups simplify the management of users and resources.

Common group types:

#### Security Groups

Used to assign permissions and control access to resources.

#### Microsoft 365 Groups

Provide collaboration capabilities for:

- Microsoft Teams
- SharePoint
- Outlook
- Planner

Benefits include:

- Simplified administration
- Centralized membership management
- Easier resource assignment

---

### Enterprise Applications

Enterprise Applications represent external or internal applications integrated with Entra ID.

Examples:

- Salesforce
- ServiceNow
- GitHub
- AWS
- Custom business applications

Administrators can:

- Manage user assignments
- Configure application access
- Monitor sign-in activity
- Review application usage

---

### App Registrations

App Registrations allow developers to integrate applications with Microsoft Identity Platform.

Typical use cases:

- Web applications
- Mobile applications
- APIs
- Background services

Key elements include:

- Client ID
- Tenant ID
- Redirect URIs
- Certificates
- Client secrets

---

## Tenant Architecture

A tenant is a dedicated instance of Microsoft Entra ID for an organization.

Each tenant contains:

- Users
- Groups
- Applications
- Devices
- Administrative configurations

Example:


Organization
     │
     ▼
Microsoft Entra Tenant
     ├── Users
     ├── Groups
     ├── Devices
     └── Applications


---

## Hybrid Identity

Many organizations maintain both on-premises and cloud environments.

Microsoft Entra ID supports hybrid identity scenarios through synchronization technologies that connect on-premises Active Directory with cloud-based identity services.

Benefits:

- Unified identity management
- Consistent user experience
- Centralized administration
- Gradual cloud adoption

---

## Device Identities

Devices can be registered or joined to Microsoft Entra ID.

Common scenarios:

### Registered Devices

Typically employee-owned devices accessing organizational resources.

### Entra Joined Devices

Cloud-managed devices directly connected to Entra ID.

### Hybrid Entra Joined Devices

Devices connected to both Active Directory and Entra ID.

Organizations use device identities to strengthen security and improve resource management.

---

## Administrative Units

Administrative Units allow organizations to delegate administration to specific teams without granting tenant-wide permissions.

Examples:

- HR Department
- Finance Department
- Regional Offices
- Business Units

Benefits:

- Scoped administration
- Reduced operational risk
- Improved governance

---

## External Identities

External Identities enables collaboration with users outside the organization.

Common scenarios:

- Business partners
- Vendors
- Consultants
- Customers

Organizations can securely invite and manage external users while maintaining visibility and control.

---

## Identity Governance

Identity Governance helps organizations manage the lifecycle of identities and access rights.

Capabilities include:

- Access reviews
- Lifecycle workflows
- Entitlement management
- Access certifications

Goals:

- Improve compliance
- Reduce excessive permissions
- Maintain access visibility

---

## Monitoring and Reporting

Microsoft Entra ID provides various monitoring capabilities.

Administrators can review:

- Sign-in logs
- Audit logs
- Application activity
- Directory changes

These insights help support operational management, compliance, and troubleshooting activities.

---

## Microsoft Ecosystem Integration

Microsoft Entra ID integrates with multiple Microsoft services:

- Azure
- Microsoft 365
- Microsoft Teams
- SharePoint Online
- Exchange Online
- Intune
- Power Platform

This integration allows organizations to manage identities consistently across their cloud environment.

---

## Benefits of Microsoft Entra ID

- Centralized directory management
- Support for cloud and hybrid environments
- Simplified user and group administration
- Scalable identity platform
- Integration with Microsoft services
- Secure external collaboration
- Identity lifecycle management
- Comprehensive monitoring and reporting

---

## Learning Summary

Microsoft Entra ID is the foundation of identity management within the Microsoft ecosystem. It provides a centralized directory service for managing users, groups, devices, applications, and external identities while supporting both cloud-native and hybrid environments.

Understanding Entra ID is essential for roles such as:

- Cloud Administrator
- Azure Administrator
- Cloud Engineer
- Security Engineer
- IAM Specialist
- DevOps Engineer