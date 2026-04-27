# Test case - Create report

| TC ID | Scenario                           | Steps                               | Expected Output                   | Type       |
| ----- | ---------------------------------- | ----------------------------------- | --------------------------------- | ---------- |
| 1 | Create new report                  | Navigate → Reports → Add Report  | New report created successfully   | Functional |
| 2 | Mandatory fields validation        | Leave mandatory fields empty → Save | Validation message displayed      | Negative   |
| 3 | Lock data with valid details     | Enter all required data → Save      | Report saved successfully and the details of the respective session details are locked.        | Functional |
| 4 | Unlock data with valid/ invalid details |click the unlock data | The section questions are editable. | functional | 
| 5 | Verify report visible in list      | Create report → Go to report list   | Newly created report visible year wise     | Functional |
| 6 | Edit report details                | Open report → Modify fields → locak data  | Updated data saved                | Functional |
| 7 | Auto-save behavior (if applicable) | Enter data → Navigate away          | Draft retained                    | Functional |
| 8 | Report ownership assigned          | Create report                       | Logged-in user who added report set as owner       | Functional |
| 9 | Report status after creation       | Create report                       | Status shows In Progress    | Functional |
| 10 | Submit report                      | Click Submit                        | Report moves to Review stage      | Functional |
| 11 | Submit the report and check the status when auditor reviews | click submit | Report moves to In audit | Fucntional |
| 12 | Check the status when auditor review is completed and approved | -- | Report moves to Completed | Fucntional |
| 13 | Submit incomplete report           | Submit without required sections    | Submission blocked                | Negative   |
| 14 | Multiple report creation           | Create multiple reports             | Each report created independently | Edge       |
