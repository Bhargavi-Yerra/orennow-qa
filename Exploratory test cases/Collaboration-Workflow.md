# Test Scenarios - Collaboration workflow

| TS ID | Scenario                            | Steps                                 | Expected Output                      | Type       |
| ----- | ----------------------------------- | ------------------------------------- | ------------------------------------ | ---------- |
| 1 | Assign collaborator to section      | Select section → Assign collaborator  | Collaborator assigned successfully   | Functional |
| 2 | Collaborator access validation      | Login as collaborator                 | Only assigned sections visible       | Security   |
| 3 | Collaborator edits assigned section | Modify answers → Save                 | Data saved successfully              | Functional |
| 4 | Unauthorized section access         | Collaborator opens unassigned section | Access restricted                    | Negative   |
| 5 | Submit section by collaborator      | Complete answers → Submit             | Section sent for review              | Functional |
| 6 | Owner receives submission           | Collaborator submits section          | Owner notified/visible status change | Functional |
| 7 | Reassign collaborator               | Change collaborator                   | Access updated correctly             | Functional |
| 8 | Deactivated collaborator access     | Deactivate collaborator → Login       | Access denied                        | Security   |
| 9 | Reactivated collaborator login      | Activate collaborator                 | Login successful                     | Functional |
| 10 | Multiple collaborators in report    | Assign different collaborators        | Each accesses respective sections    | Functional |
| 11 | Section submission status           | Submit section                        | Status updated correctly             | Functional |
