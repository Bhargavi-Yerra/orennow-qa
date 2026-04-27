# Test case - Review & approval flow

| TC ID | Scenario                              | Steps                          | Expected Output           | Type       |
| ----- | ------------------------------------- | ------------------------------ | ------------------------- | ---------- |
| 1 | Owner reviews collaborator submission | Open submitted section         | Data visible correctly    | Functional |
| 2 | Approve section                       | Click Approve                  | Section approved          | Functional |
| 3 | Reject section                        | Click Reject                   | Sent back to collaborator | Functional |
| 4 | Add review comments                   | Enter comments → Submit        | Comment saved             | Functional |
| 5 | Auditor receives report               | Submit report                  | Auditor access enabled    | Functional |
| 6 | Auditor reviews report                | Login as auditor → Open report | All details visible       | Functional |
| 7 | Auditor validates information         | Verify entered data            | Data matches submission   | Functional |
| 8 | Prevent approval without review       | Approve without opening        | System restricts action   | Negative   |
| 9 | Final report submission               | Complete approvals             | Report marked Completed   | Functional |
