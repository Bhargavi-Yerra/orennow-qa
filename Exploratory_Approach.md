# Exploratory Testing Approach Document

## 1. Objective
The objective of this exploratory testing session was to validate the end-to-end functionality of the application by simulating real user behavior. The focus was on verifying authentication flows, user management, report creation and approval workflows, and collaboration features including comments and role-based actions.

---

## 2. Approach Followed
An exploratory testing approach was adopted, where test design, execution, and learning were performed simultaneously. The application was navigated in a user-centric manner without predefined test cases, allowing dynamic discovery of functional issues and workflow gaps.

---

## 3. Test Execution Steps

### 3.1 Authentication & Login Validation
- Logged into the application using email and password credentials.
- Verified login using email OTP-based authentication.
- Validated successful login and session creation.
- Executed **Forgot Password** flow and confirmed password reset functionality.

### 3.2 Settings Module Validation
- Navigated to the **Settings** screen post-login.
- Reviewed all available tabs within settings.
- Attempted updates to user and configuration details.
- Verified whether changes were successfully saved and reflected.


### 3.3 User Management Functionality
- Navigated to the **User Management** section.
- Created the following entities:
  - Business Units
  - Collaborators
  - Auditors
- Verified role assignments and creation success messages.


### 3.4 Access Control & User Status Validation
- Deactivated a collaborator account.
- Attempted login using the deactivated account to verify access restrictions.
- Reactivated the collaborator account.
- Successfully logged in to confirm restoration of access.


### 3.5 Report Creation & Workflow Validation
- Initiated a new report creation process.
- Completed and submitted a report for auditor review.
- Verified submission status and workflow transition.


### 3.6 Multi-Role Report Collaboration
- Created an additional report.
- Assigned a section of the report to a collaborator.
- Verified collaborator access to assigned section.
- Collaborator successfully submitted responses to section questions.
- Verified workflow transition to report owner for review.

### 3.7 Commenting and Communication Feature
- Explored the comment/chat functionality.
- Tested communication between:
  - Report owner
  - Collaborator
- Verified real-time message exchange and visibility on both ends.


### 3.8 Approval Workflow Validation
- Approved the submitted section.
- Confirmed successful submission to the report owner.


### 3.9 Final Report Submission
- Completed remaining report details.
- Submitted the final report successfully.
- Verified final status update in the system.


### 3.10 Auditor Review Process
- Logged in as auditor.
- Reviewed submitted reports and verified entered details in the second report.
- Checked report review summary section.
- Validated correctness and completeness of report data.

---

## 4. Observations
- Authentication flows (password + OTP) worked as expected.
- Role-based access control (collaborator, auditor, owner) was functioning correctly.
- Report workflow transitions were smooth across multiple roles.
- Collaboration and comment features supported real-time interaction effectively.
- Report review and summary sections provided accurate data visibility.
