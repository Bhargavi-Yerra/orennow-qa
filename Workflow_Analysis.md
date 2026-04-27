# Workflow Analysis

**Product:** Oren Sustainability Hub (OSH)
**Testing Type:** Workflow & Role-Based Analysis
**Objective:** Analyze the end-to-end sustainability reporting workflow involving multiple users, role permissions, collaboration, and approval lifecycle.

---

## 1. Overview

Oren Sustainability Hub (OSH) follows a **multi-user collaborative reporting workflow** designed to collect sustainability data across organizational departments and consolidate it into a company-level sustainability report.

The workflow operates on a **role-based access model** supported by task delegation, notifications, and staged approvals.

The system workflow primarily involves three roles:

* Admin
* Collaborator
* Auditor


## 2. Role-Based Workflow Structure

### 2.1 Sustainability Team (Admin)

**Primary Responsibilities**

* Configure company profile and system settings
* Define organizational structure (Business Units)
* Add and manage users
* Create sustainability reports
* Delegate questions/sections
* Review collaborator submissions
* Submit reports for audit review

**System Position**
👉 Workflow initiator and controller.


### 2.2 Collaborator

**Primary Responsibilities**

* Receive assigned questions or report sections
* Enter sustainability data for assigned business units
* Upload supporting information
* Submit responses for review

**System Position**
👉 Data contributor.


### 2.3 Auditor

**Primary Responsibilities**

* Review completed reports
* Validate submitted data
* Provide feedback or approval
* Ensure report accuracy before finalization

**System Position**
👉 Independent reviewer and validator.


## 3. Multi-User Interaction Flow

```
Admin Setup
      ↓
User Creation
      ↓
Report Creation
      ↓
Question Delegation
      ↓
Collaborator Submission
      ↓
Admin Review
      ↓
Auditor Validation
      ↓
Dashboard Visualization
```


## 4. Email & Notification Workflow Analysis

The workflow progression depends heavily on communication triggers.

Expected notification sequence:

1. User Invitation Email → Collaborator/Auditor onboarding
2. Task Assignment Notification → Delegated questions
3. Submission Notification → Admin informed
4. Review Request Notification → Auditor engagement

These notifications ensure continuous workflow movement between roles.


## 6. Role Access Validation Observations

Key workflow expectations:

| Role         | Allowed Actions                |
| ------------ | ------------------------------ |
| Admin        | Full system control            |
| Collaborator | Answer assigned questions only |
| Auditor      | Review without editing data    |

