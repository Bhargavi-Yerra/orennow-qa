# Test case - Comments and communication

| TC ID | Scenario                             | Steps                              | Expected Output                 | Type       |
| ----- | ------------------------------------ | ---------------------------------- | ------------------------------- | ---------- |
| 1 | Add comment in report                | Open comment section → Add message | Comment posted                  | Functional |
| 2 | Two-way communication                | Owner & collaborator chat          | Messages visible both sides     | Functional |
| 3 | Comment visibility                   | Add comment in section             | Visible to relevant users       | Functional |
| 4 | Timestamp validation                 | Add comment                        | Correct timestamp displayed     | UI         |
| 5 | Multiple comments                    | Add multiple messages              | All messages saved sequentially | Functional |
| 6 | Empty comment submission             | Submit blank comment               | Validation shown                | Negative   |
| 7 | Role-based commenting                | Different roles comment            | Access maintained per role      | Security   |
| 8 | Comment persistence                  | Refresh page                       | Comments remain                 | Functional |
| 9 | Comment during review                | Add comment in review stage        | Allowed and saved               | Functional |
| 10 | Notification trigger | Post comment                       | Relevant user notified via email         | Functional |
