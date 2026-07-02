# OU Design, User Provisioning & Access Control

## Description

Designed and implemented an Active Directory environment featuring Organizational Unit (OU) design, automated user provisioning, role-based access control, administrative delegation, and fine-grained password policies.

## Objectives

* Design a scalable and manageable OU hierarchy
* Automate user provisioning using PowerShell and CSV imports
* Implement Role-Based Access Control using AGDLP
* Delegate administrative tasks following the principle of least privilege
* Apply Fine-Grained Password Policies to privileged accounts

## Tasks Performed

#### Organizational Unit Design

Configuration:

* Designed an OU hierarchy for users, computers, groups, and administrative accounts
* Separated user and computer objects into dedicated OUs to simplify administration
* Structured department-specific OUs for IT, HR, Finance, and Sales
* Improved scalability and maintainability through logical object organization

Screenshots:

---

#### Bulk User Provisioning with PowerShell

Configuration:

* Created PowerShell scripts to automate user creation from CSV files
* Reduced manual administrative effort and improved provisioning consistency
* Configured the script to dynamically determine the target OU for each user
* Constructed distinguished names using the CSV `Path` value and domain information

Screenshots:

---

#### Role-Based Access Control with AGDLP

Configuration:

* Implemented the AGDLP model for permission management
* Created Global groups to represent job roles and departments
* Assigned permissions to Domain Local groups that manage resource access
* Simplified onboarding by granting access through group membership rather than individual permissions

Screenshots:

---

#### Administrative Delegation

Configuration:

* Delegated password reset and account unlock permissions to the Helpdesk group
* Scoped delegated permissions to the Users OU only
* Implemented least privilege principles by avoiding Domain Administrator access for routine support tasks
* Verified that delegated administrators could perform assigned tasks without elevated privileges

Screenshots:

---

#### Fine-Grained Password Policies

Configuration:

* Created Fine-Grained Password Policies for privileged administrative accounts
* Applied stronger password and lockout requirements to sensitive accounts
* Configured policy assignment through security group membership
* Demonstrated how FGPPs provide greater flexibility than domain-wide password policies

Screenshots:

## Key Concepts Learned

* Organizational Unit design and hierarchy planning
* Bulk user provisioning using PowerShell automation
* Distinguished Names and LDAP paths
* Role-Based Access Control using AGDLP
* Administrative delegation and least privilege
* Fine-Grained Password Policies
* Enterprise Active Directory administration practices
