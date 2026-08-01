# 🏥 Phase 1 – Cloud Identity Foundation & Zero Trust Implementation

## Overview

Cedar Valley Health (CVH) is a fictional small-to-midsize healthcare organization undergoing an **Identity Modernization Initiative** to improve security, simplify identity administration, and prepare for future growth.

Phase 1 focused on establishing CVH's **Microsoft Entra ID cloud identity foundation** by implementing:

- ☁️ Centralized identity management
- 👤 Cloud user provisioning
- 🔐 Role-Based Access Control (RBAC)
- 📱 Multi-Factor Authentication (MFA)
- 🛡️ Zero Trust security principles

In this simulation, I served as the **Cloud IAM Administrator**, responsible for designing, implementing, securing, and documenting the organization's cloud identity environment.

The goal of this phase was to create a scalable identity foundation that could support future IAM capabilities, including:

- Identity Governance
- Conditional Access
- Hybrid Identity
- Automation

---

## 🏢 Business Context

Before the modernization initiative, CVH operated as a growing healthcare organization supporting:

- Clinical services
- Administrative operations
- Finance
- Human Resources
- Information Technology
- Executive leadership

As the organization expanded, leadership identified the need for stronger identity controls, improved authentication security, and a more structured access management model.

Microsoft Entra ID was selected as the organization's cloud identity platform to support this transformation.

---

## 🚀 Phase 1 Scenario

Rather than migrating the entire organization at once, CVH adopted a phased identity modernization approach.

Phase 1 focused on corporate business departments to establish a secure identity foundation before expanding IAM services to additional departments.

The implementation included:

- Creating cloud-only identities
- Importing users through CSV bulk provisioning
- Organizing users with security groups
- Assigning administrative roles
- Configuring MFA
- Validating authentication and authorization
- Reviewing audit activity

---

## 👨‍💻 IAM Administrator Responsibilities

As the Cloud IAM Administrator, responsibilities included:

- Designing the Microsoft Entra ID environment
- Provisioning employee identities
- Creating department-based security groups
- Implementing RBAC
- Assigning administrative permissions
- Configuring authentication security
- Validating user access
- Documenting implementation procedures
---

# 🛠 Technologies Used

| Component | Technology |
|-----------|------------|
| Identity Platform | Microsoft Entra ID |
| Identity Type | Cloud-Only Identities |
| Authentication | Microsoft Authenticator |
| Provisioning | CSV Bulk User Import |
| Access Model | Role-Based Access Control (RBAC) |
| Security Strategy | Zero Trust |
| Documentation | GitHub |

---

# 🏢 Business Departments

Phase 1 migrated Cedar Valley Health's corporate business departments into Microsoft Entra ID.

The following security groups were created to organize identities and support Role-Based Access Control.

- CVH-Executives
- CVH-Finance-Team
- CVH-HR-Team
- CVH-IT-Department
- CVH-Sales-Team

Using department-based security groups simplifies administration, improves scalability, and supports the Principle of Least Privilege by assigning permissions to groups instead of individual users.

---

# 🔨 Implementation

## 1. User Provisioning

Created **10 Cedar Valley Health employee accounts** using Microsoft Entra ID CSV bulk user provisioning.

Each user account included:

- First Name
- Last Name
- Display Name
- User Principal Name (UPN)
- Department
- Job Title
- Office Location

### Validation

- Successfully imported all users
- Verified account creation
- Confirmed successful sign-in capability

📄 Documentation:
`Documentation/User-Provisioning.md`

---

## 2. Security Group Administration

Created department-based security groups to simplify access management and support Role-Based Access Control.

### Groups Created

- CVH-Executives
- CVH-Finance-Team
- CVH-HR-Team
- CVH-IT-Department
- CVH-Sales-Team

Users were assigned to groups according to their department and business responsibilities.

📄 Documentation:
`Documentation/Security-Groups.md`

---

## 3. Administrative Role Assignments

Assigned Microsoft Entra administrative roles following the Principle of Least Privilege.

| User | Administrative Role |
|------|----------------------|
| Ethan Hughes | Global Administrator |
| Michael Rivera | User Administrator |
| James Walker | Helpdesk Administrator |

Only users requiring elevated privileges received administrative permissions.

📄 Documentation:
`Documentation/RBAC-Role-Assignments.md`

---

## 4. Multi-Factor Authentication (MFA)

Configured Multi-Factor Authentication (MFA) using Microsoft Authenticator for all cloud user identities within the Phase 1 environment.

This implementation strengthens account security by requiring users to verify their identity with a second authentication factor before access is granted.

### Validation

- Registered Microsoft Authenticator for all user accounts
- Completed MFA enrollment
- Verified successful user authentication
- Validated password and mobile approval authentication
- Confirmed users could securely access assigned resources after MFA verification

📄 Documentation:
`Documentation/MFA-Implementation.md`

---

## 5. User Access Validation & Audit Logging

Validated that users could:

- Successfully authenticate
- Access resources appropriate to their assigned roles
- Complete Multi-Factor Authentication
- Operate within least-privilege permissions

Microsoft Entra audit logs were reviewed to verify:

- User provisioning
- Security group membership changes
- Administrative role assignments
- Authentication events

📄 Documentation:
`Documentation/Zero-Trust-Validation.md`

---

# 🔐 Zero Trust Principles Applied

## Verify Explicitly

Every user was required to authenticate using secure credentials and Multi-Factor Authentication before access was granted.

## Use Least Privilege

Administrative permissions were assigned only when required through Role-Based Access Control and department-based security groups.

## Assume Breach

Identity was treated as the organization's primary security perimeter by validating authentication events, monitoring administrative changes, and reviewing audit logs.

---

# ✅ Phase 1 Outcomes

At the completion of Phase 1, Cedar Valley Health successfully established a secure cloud identity foundation.

### Completed Deliverables

- ✅ Deployed Microsoft Entra ID
- ✅ Provisioned 10 cloud user accounts
- ✅ Created 5 department security groups
- ✅ Assigned Microsoft Entra administrative roles
- ✅ Configured Multi-Factor Authentication
- ✅ Validated user authentication and authorization
- ✅ Reviewed Microsoft Entra audit logs
- ✅ Applied Zero Trust security principles
- ✅ Produced enterprise-style technical documentation

The environment now supports:

- Centralized cloud identity management
- Role-Based Access Control (RBAC)
- Multi-Factor Authentication (MFA)
- Least Privilege administration
- Audit visibility
- Zero Trust security practices

---

# 📷 Supporting Documentation

Detailed implementation guides are available throughout this phase.

```
Documentation/
│
├── User-Provisioning.md
├── Security-Groups.md
├── RBAC-Role-Assignments.md
├── MFA-Implementation.md
└── Zero-Trust-Validation.md
```

Supporting screenshots are available in the **Screenshots** folder.

---

# 📚 Lessons Learned

This phase strengthened my understanding of enterprise cloud identity administration by demonstrating how organizations provision users, organize identities using security groups, implement Role-Based Access Control, configure Multi-Factor Authentication, assign administrative permissions, validate secure access, and monitor identity operations through Microsoft Entra audit logs.

It also reinforced the importance of designing scalable identity solutions that align with Microsoft's Zero Trust security model.
