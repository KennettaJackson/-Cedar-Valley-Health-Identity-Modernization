# Phase 1 – Cloud Identity Foundation & Zero Trust Implementation

## Overview

This phase establishes the Microsoft Entra ID cloud identity foundation for Cedar Valley Health.

The objective was to create a secure identity environment by provisioning users, implementing role-based access control, configuring authentication security, and validating identity operations using Zero Trust principles.

---

# Objectives

The goals of Phase 1 were:

- Deploy Microsoft Entra ID
- Create cloud-only identities
- Import users using CSV bulk provisioning
- Create department-based security groups
- Assign administrative roles
- Configure MFA
- Validate access permissions
- Review audit logs

---

# Environment

| Component | Technology |
|---|---|
| Identity Platform | Microsoft Entra ID |
| Identity Type | Cloud-only users |
| Authentication | Microsoft Authenticator |
| Access Model | RBAC |
| Security Model | Zero Trust |

---

# Implementation

## 1. User Provisioning

Created 10 Cedar Valley Health employee accounts using Microsoft Entra ID bulk user creation.

User attributes included:

- Name
- Department
- Job Title
- Location
- User Principal Name

Documentation:
`Documentation/User-Provisioning.md`

---

## 2. Security Groups

Created department-based security groups:

- CVH-Executives
- CVH-Finance-Team
- CVH-HR-Team
- CVH-IT-Department
- CVH-Sales-Team

Groups were used to support RBAC and Least Privilege access.

Documentation:
`Documentation/Security-Groups.md`

---

## 3. Administrative Roles

Assigned Microsoft Entra roles:

| User | Role |
|-|-|
| Ethan Hughes | Global Administrator |
| Michael Rivera | User Administrator |
| James Walker | Helpdesk Administrator |

Documentation:
`Documentation/RBAC-Role-Assignments.md`

---

## 4. MFA Implementation

Configured Microsoft Authenticator MFA.

Validated:

- Registration
- Enrollment
- Authentication

Documentation:
`Documentation/MFA-Implementation.md`

---

## 5. Audit Logging

Reviewed Microsoft Entra audit logs to verify:

- User creation
- Group changes
- Role assignments

Documentation:
`Documentation/Zero-Trust-Validation.md`

---

# Phase 1 Outcome

Phase 1 successfully established a secure cloud identity foundation for Cedar Valley Health.

The environment now supports:

- Centralized identity management
- RBAC
- MFA
- Least Privilege
- Audit visibility
- Zero Trust security practices
