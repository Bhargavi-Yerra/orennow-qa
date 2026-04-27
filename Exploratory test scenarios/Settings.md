# Test scenarios - Settings

### Settings navigation

| TS ID  | Scenario                          | Steps                                  | Expected Output                                                                                                                                                                   | Type        |
| ------ | --------------------------------- | -------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| 1 | Open Settings screen              | Click **Preferences** tab from sidebar | User navigates to Settings screen                                                                                                                                                 | Functional  |
| 2 | Verify Settings tabs visibility   | Open Settings screen                   | Following tabs displayed:<br>Preferences<br>Personal Profile<br>Company Profile<br>Emission Configuration Fuels<br>Emission Configuration Gases<br>Scope 2 Emission Configuration | UI          |
| 3 | Default landing tab               | Open Settings                          | Preferences tab loads by default                                                                                                                                                  | Functional  |
| 4 | Navigate to Personal Profile      | Click Personal Profile tab             | Personal Profile screen opens                                                                                                                                                     | Navigation  |
| 5 | Navigate to Company Profile       | Click Company Profile tab              | Company Profile screen opens                                                                                                                                                      | Navigation  |
| 6 | Navigate to Emission Fuels        | Click Emission Configuration Fuels     | Fuels configuration screen opens                                                                                                                                                  | Navigation  |
| 7 | Navigate to Emission Gases        | Click Emission Configuration Gases     | Gases configuration screen opens                                                                                                                                                  | Navigation  |
| 8 | Navigate to Scope 2 Configuration | Click Scope 2 emission configuration   | Scope 2 screen opens                                                                                                                                                              | Navigation  |
| 9 | Switch tabs without saving        | Modify data → switch tab               | Unsaved changes are not saved                                                                                                                                    | Exploratory |

### Settings - Preferences

| TC ID  | Scenario                     | Steps                   | Expected Output                                                                                                                                                                                                                                                                                                         | Type       |
| ------ | ---------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| 10 | Open Preferences tab         | Click Preferences       | Preferences tab loads                                                                                                                                                                                                                                                                                                   | Functional |
| 11 | Verify Preferences fields    | Open Preferences tab    | Fields displayed:<br>Date Format<br>Time Format<br>Currency<br>Data Capture Frequency<br>Reporting Cycle<br>Number Format<br>Email Reminders<br>Reporting Updates<br>Auto Validation<br>Comment Notifications<br>Review Reminders<br>Product Code<br>Working Days<br>Air Emission Measurement<br>Data Anomaly Bandwidth | UI         |
| 22 | Modify preferences           | Update values           | Updated values saved successfully                                                                                                                                                                                                                                                                                       | Functional |
| 13 | Verify persistence           | Refresh page            | Saved preferences remain                                                                                                                                                                                                                                                                                                | Regression |

### Settings - Company profile

| TC ID  | Scenario                      | Steps                     | Expected Output                                                                                                                         | Type       |
| ------ | ----------------------------- | ------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| 14 | Open Company Profile          | Click Company Profile tab | Company Profile screen opens                                                                                                            | Functional |
| 15 | Verify Company Profile fields | Load screen               | Fields displayed:<br>Profile Photo<br>Edit Photo Icon<br>Company Name*<br>Country*<br>Location*<br>Industry*<br>Website*<br>TIN Number* | UI         |
| 16 | Verify prefilled data         | Open page                 | Previously saved data displayed                                                                                                         | Functional |
| 17 | Verify editable fields        | Inspect fields            | Editable:<br>Company Name<br>Industry<br>Website                                                                                        | UI         |
| 18 | Verify non-editable fields    | Inspect fields            | Non-editable:<br>Country<br>Location<br>TIN Number                                                                                      | UI         |
| 19 | Save button disabled   | Leave mandatory fields empty | Save button disabled                 | Validation  |
| 20 | Enable save button     | Fill valid inputs            | Save button enabled                  | Functional  |
| 21 | Update company details | Modify data → Save           | Updated details reflected everywhere | Integration |
| 22 | Verify updated company details reflected across platform | 1. Navigate to **Settings → Company Profile**.<br>2. Update Company Name / Website / Industry.<br>3. Click **Save**.<br>4. Navigate to Dashboard.<br>5. Open Reporting module.<br>6. Open existing report.<br>7. Check headers, report summary, dashboard widgets, and profile references. | Updated company details must be reflected consistently across all applicable modules and screens without mismatch or delay. | Integration |

### Settings - Personal profile

| TC ID | Scenario                     | Steps                                 | Expected Output                                                                                          | Type       |
| ----- | ---------------------------- | ------------------------------------- | -------------------------------------------------------------------------------------------------------- | ---------- |
| 23 | Navigate to Personal Profile | Click **Settings → Personal Profile** | Personal Profile screen opens successfully                                                               | Functional |
| 24 | Verify fields displayed      | Open Personal Profile                 | Fields displayed:<br>Full Name<br>Role<br>Phone Number<br>Email<br>Update Password button<br>Save button | UI         |
| 25 | Verify pre-filled data       | Load Personal Profile page            | Existing user details displayed correctly                                                                | Functional |
| 26 | Verify role visibility       | Check Role field                      | Correct role displayed and should be read-only                                                     | Role-Based |
| 27 | Verify editable fields       | Inspect fields                        | Full Name & Phone editable                                                                               | UI         |
| 28 | Verify non-editable email    | Attempt editing email                 | Email field should be read-only                                                         | Validation |

### Settings - Emission configuration fuels

| TC ID | Scenario                                 | Steps                                                 | Expected Output                                                                           | Type       |
| ----- | ---------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------------- | ---------- |
| 29 | Navigate to Emission Configuration Fuels | Go to Settings → Click *Emission Configuration Fuels* | User lands on Fuels configuration screen                                                  | Functional |
| 30 | Verify page elements                     | Open screen                                           | Fuel table, Database dropdown, Emission Factor, Unit column, Save Settings button visible | UI         |
| 31 | Verify financial year display            | Check top right section                               | Selected Financial Year displayed correctly                                               | UI         |
| 32 | Change financial year                    | Select different year                                 | Fuel configuration updates accordingly                                                    | Functional |
| 33 | Verify fuel list loaded  | Open screen        | Fuel types displayed (Diesel, Petrol, CNG, Coal, etc.) | Functional |
| 34 | Scroll fuel list         | Scroll vertically  | Smooth scrolling without UI break                      | UI         |
| 35 | Pagination check         | Click page numbers | Data loads correctly per page                          | Functional |
| 36 | Next/Previous pagination | Click Next/Prev    | Correct page navigation                                | Functional |
| 37 | Open database dropdown             | Click dropdown for any fuel   | Database options displayed                    | Functional  |
| 38 | Verify dropdown options            | Expand dropdown               | Legacy DB, EF DEFRA (Year variants) displayed | UI          |
| 39 | Select database value              | Choose EF DEFRA (2024)        | Emission factor auto-populates                | Functional  |
| 40 | Change database repeatedly         | Switch options multiple times | Values update correctly without lag           | Exploratory |
| 41 | Leave database unselected          | Keep default value            | System handles empty selection safely         | Edge        |
| 42 | Select database for multiple fuels | Update several rows           | Each fuel retains its selected database       | Functional  |
| 43 | Verify emission factor auto-fill | Select database             | Emission factor auto-populates                      | Functional |
| 44 | Verify emission factor format    | Observe value               | Decimal precision displayed correctly               | UI         |
| 45 | Verify read-only behavior        | Try editing emission factor | Field should be non-editable (if system controlled) | Validation |
| 46 | Verify unit mapping              | Select database             | Correct unit displayed (kg/Litre etc.)              | Functional |
| 47 | Save updated configuration | Modify database → Click Save Settings | Settings saved successfully         | Positive    |
| 48 | Save without changes       | Click Save Settings                   | No error; system handles gracefully | Edge        |
| 49 | Refresh after save         | Save → Refresh page                   | Saved values persist                | Regression  |
| 50 | Navigate away after save   | Save → Open another module            | Changes retained                    | Integration |



