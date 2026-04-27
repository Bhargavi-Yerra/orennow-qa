# Test scenarios User Management 

TC ID | Steps | Expected output | Type | 
-- | -- | -- | -- |
1 | Navigate to User Management module | User should be able to access User Management screen successfully |Functional
2 | Observe User Management screen | Two tabs must be displayed: My Company, Auditors | UI / Functional
3 | Click on "My Company" tab | User should be navigated to My Company tab | Functional
4 | Click on "Auditors" tab | User should be navigated to Auditors tab | | Functional
5 | In My Company tab, observe available options | Two view options must be displayed: By Business Unit, By User |  UI / Functional
6 | Select "By Business Unit" option | Business Unit view should be displayed |  Functional
7 | Select "By User" option | User/Collaborator list view should be displayed | Functional
8 | Switch between views multiple times | View should switch correctly without UI/data issues |  Functional / Usability
9 | Select "By Business Unit" | System should display all required buttons and Business Unit table |  UI / Functional
10 | Click "Add Business Unit" | User should be able to initiate creation of a Business Unit |  Functional
11 | Click "Add Multiple Business Units" | Bulk upload flow should be triggered |  Functional
12 | Click "Add Multiple Collaborators" | User should be able to add multiple collaborators |  Functional
13 | Observe Business Unit table | Table should display correct list of business units | Functional / Data Validation
14 | Verify empty state for Business Units | Proper empty state message should be displayed |  UI / Usability
15 | Perform actions on Business Unit list | Actions should work correctly and reflect updates |  Functional
16 | Select "By User" option | Collaborator list should be displayed |  Functional
17 | Observe By User screen | Collaborator list and Add Collaborator button must be visible | UI / Functional
18 | Click "Add Collaborator" | User should be able to add a collaborator | Functional
19 | Verify collaborator list data | Data should be displayed correctly | Data Validation
20 | Verify empty state for collaborators | Proper empty state message should be displayed | UI / Usability
21 | Switch views after adding collaborator | Data should reflect correctly across views | Functional / Integration
22 | Navigate to Auditors tab | Auditor screen should be displayed | Functional
23 | Observe Auditors screen | "Add Auditor" button must be visible | UI / Functional
24 | Click "Add Auditor" | User should be able to initiate auditor creation | Functional
25 | Verify auditor list | Auditor data should be displayed correctly | Data Validation
26 | Verify empty state for auditors | Proper empty state message should be displayed | UI / Usability
27 | Rapidly switch between tabs | System should remain stable without crashes | Stability / Exploratory
28 | Switch views with unsaved changes | System should handle state properly (warn/retain) | Usability / Exploratory
29 | Load screen with large data | System should handle without performance degradation | Performance
30 | Perform multiple add operations | System should not create duplicate or inconsistent data | Functional / Data Integrity
31 | Refresh page after changes | Data should persist and display correctly | Functional / Persistence
32 | Verify role-based access | Only authorized users should manage users/auditors | Security / Functional
