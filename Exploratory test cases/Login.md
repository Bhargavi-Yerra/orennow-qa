# Test scenarios - Login

### Email + Password login

| TS ID    | Scenario                            | Steps                                        | Expected Output                        | Type       |
| -------- | ----------------------------------- | -------------------------------------------- | -------------------------------------- | ---------- |
| 1 | Login with valid Email + Password   | Enter valid email and password → Click Login | User navigates to Dashboard            | Positive   |
| 2 | Login with incorrect password       | Enter valid email + wrong password           | Error message displayed                | Negative   |
| 3 | Login with unregistered email       | Enter unregistered email                     | Login denied with error message        | Negative   |
| 4 | Login with empty email              | Leave email blank → Click Login              | Email required validation shown        | Validation |
| 5 | Login with empty password           | Leave password blank                         | Password required validation           | Validation |
| 6 | Login with both fields empty        | Click Login without input                    | Mandatory field validations shown      | Validation |
| 7 | Password length validation          | Enter password < 8 characters                | Validation error displayed             | Validation |
| 8 | Invalid email format                | Enter invalid email format                   | Email format validation displayed      | Validation |
| 9 | Successful login redirection        | Login successfully                           | User lands on Dashboard screen         | Functional |
| 10 | Session persistence                 | Refresh browser after login                  | User remains logged in                 | Functional |
| 11 | Browser back navigation after login | Click browser back button                    | User should not return to login screen | Security   |

### Email + OTP login
| TC ID    | Scenario                     | Steps                                       | Expected Output                       | Type       |
| -------- | ---------------------------- | ------------------------------------------- | ------------------------------------- | ---------- |
| 12 |Email + OTP flow navigation | Click the `Get OTP` button. | Navigates to teh Email + OTP login screen. | Positive |
| 13 | Login using Email + OTP      | Enter email → Request OTP → Enter valid OTP | User logged in successfully           | Positive   |
| 14 | OTP sent to registered email | Request OTP                                 | OTP email received                    | Functional |
| 15 | Invalid OTP entry            | Enter wrong OTP                             | Error message displayed               | Negative   |
| 16 | Expired OTP validation       | Enter OTP after 15 minutes                  | OTP expired message shown             | Edge       |
| 17 | Resend OTP                   | Click Resend OTP                            | New OTP generated and sent            | Functional |
| 18 | Multiple OTP requests        | Click resend OTP multiple times             | System handles requests without crash | Edge       |
| 19 | Empty OTP submission         | Click Verify without OTP                    | Validation message shown              | Validation |

### Forgot Password Flow

| TC ID    | Scenario                           | Steps                      | Expected Output              | Type       |
| -------- | ---------------------------------- | -------------------------- | ---------------------------- | ---------- |
| 20 | Access Forgot Password             | Click Forgot Password link | Forgot Password page opens   | Functional |
| 21 | Submit valid email for reset       | Enter registered email     | Reset link email sent        | Positive   |
| 22 | Forgot password with invalid email | Enter unregistered email   | Error message displayed      | Negative   |
| 23 | Forgot password empty field        | Submit without email       | Validation message displayed | Validation |
| 24 | Reset email delivery check         | Trigger reset              | Email received successfully  | Functional |

### Reset Password Flow
| TC ID    | Scenario                       | Steps                                | Expected Output                   | Type       |
| -------- | ------------------------------ | ------------------------------------ | --------------------------------- | ---------- |
| 25 | Reset password using link      | Open reset link → Enter new password | Password updated successfully     | Positive   |
| 26 | Password length validation     | Enter password < 8 chars             | Validation error displayed        | Validation |
| 27 | Confirm password mismatch      | Enter different confirm password     | Error message displayed           | Validation |
| 28 | Reset password success login   | Login with new password              | Login successful                  | Regression |
| 29 | Old password login after reset | Login with old password              | Login denied                      | Security   |
| 30 | Reuse same password            | Reset using same password            | System behavior verified          | Edge       |
| 31 | Reset link reuse               | Use reset link twice                 | Link should expire or block reuse | Security   |


