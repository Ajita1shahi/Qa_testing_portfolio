\# LunaCycle Regression Testing Report



\## 1. Project Information



\- Project Name: LunaCycle

\- Testing Type: Regression Testing

\- Application: LunaCycle Period Tracking System

\- Test Environment: Local development environment

\- Tester: Ajita Shahi

\- Execution Date: 2026-10-27



\## 2. Objective



The objective of regression testing is to verify that the existing LunaCycle features continue to work correctly and that changes or fixes have not introduced new defects.



\## 3. Scope of Testing



The following existing features will be retested:



\- User login

\- Period record creation

\- Period record editing and deletion

\- Period date validation

\- Calendar and cycle predictions

\- Symptom journal

\- Insights and charts



\## 4. Test Results



| Test ID | Feature | Expected Result | Actual Result | Status |

|---|---|---|---|---|

| REG\_001 | Login with valid credentials | User logs in successfully |log in succesfully |Pass|

| REG\_002 | Login with invalid credentials | Login is rejected with an error message | Log in rejected by saying "Invalid username or password."| Pass |

| REG\_003 | Add a period record | Record is saved and displayed |Record is saved and showed "Your period record was saved!" message |  Pass |

| REG\_004 | Edit a period record | Updated information is displayed | Updated information is displayed and showed notification "Your period record was updated!" |Pass |

| REG\_005 | Delete a period record | Selected record is removed | Selecte record is delete and showed "Your period record was deleted." |Pass  |

| REG\_006 | Validate an invalid date range | Application rejects an end date before the start date |Applicatio is rejected and said "The end date cannot be before the start date" |Pass  |

| REG\_007 | View calendar | Recorded period dates appear correctly |  Recorded period dates appear correctly|Pass  |

| REG\_008 | View cycle predictions | Predictions are displayed when sufficient history exists |  Predictions are displayed when sufficient history exists| Pass|

| REG\_009 | Save a symptom entry | Symptom entry is saved and displayed |System save with "Your daily journal entry was saved!" message  | Pass|

| REG\_010 | View insights | Insights and charts load correctly |Insights and charts load correct | Pass|



\## 5. Execution Summary



\- Total Test Cases: 10

\- Passed: 10

\- Failed: 0

\- Blocked: 0




\## 6. Defects and Observations



No new defects have been confirmed during this regression test cyclet.



\## 7. Conclusion



All the test were succesfully passed.



