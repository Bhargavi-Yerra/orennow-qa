# Test case - Login

## Pre-read document
[Exploratory approach]()


TC ID | Steps | Expected output | Actual output | Tester status | Bug ID (If actual output is differnt) |
-- | -- | -- | -- | -- | -- |
TC001 | Open the application login page | Login screen should be displayed with Email, Password fields and Login button | | 
TC002 | Enter valid email and password → click Login button | User should be successfully authenticated and redirected to the dashboard screen | | 
TC003 | Enter invalid email or password → click Login button | System should display appropriate error message (e.g., invalid credentials) | | 
TC004 | Leave email and password empty → click Login button | System should show validation messages for required fields | |
TC005 | Click on “Get OTP” button on login screen | User should be navigated to Email Address screen for OTP flow | |
TC006 | Enter valid email address on OTP email screen → click “Send Code” button | OTP should be sent successfully to the entered email address and confirmation message should be displayed | | 
TC007 | Enter unregistered or invalid email → click “Send Code” button | System should display error message indicating email is not registered/invalid | | 
TC008 | Click “Send Code” without entering email address | System should show validation message for required email field | | 
TC009 | Verify OTP received in email inbox | OTP should be delivered successfully to the registered email address | | 
TC010 | Enter correct OTP (after email verification flow) | User should be successfully authenticated and redirected to dashboard screen  | | 
TC011 | Enter incorrect OTP | System should display error message indicating invalid OTP | | 
TC012 | Enter expired OTP | System should reject OTP and show expiry error message | |
TC013 | Re-send OTP from email screen | A new OTP should be generated and sent to the email address, invalidating previous OTP | | 
