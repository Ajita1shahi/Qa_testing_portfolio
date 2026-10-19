# LunaCycle : QA Test Plan

## 1. Project Information

- Project Name: LunaCycle
- Document ID: LC-TP-001
- Version: 1.0
- Testing Type: Manual Software Testing
- Application Type: Django Web Application
- Environment: Local Development Environment
- Test Status: Planned

## 2. Objective

The objective is to verify that LunaCycle's implemented features work as expected, invalid inputs are handled correctly, stored data remains consistent, and users can access only the information they are authorized to view.

## 3. Features in Scope

1. User registration and login
2. Period record creation
3. Period record editing and deletion
4. Calendar and cycle predictions
5. Daily symptom journal
6. Insights and charts
7. Input validation and error handling
8. Data integrity and access control

## 4. Testing Types

- Functional Testing: Verify the behavior of implemented features.
- Negative Testing: Check how the application handles invalid or missing inputs.
- Boundary Testing: Test date boundaries and unusual but valid inputs.
- Regression Testing: Verify that existing features continue working after changes.
- Data Integrity Testing: Compare displayed information with saved database records.
- Security Testing: Check authentication, protected pages, and access to user-specific data.

## 5. Test Environment

- Application: LunaCycle
- Framework: Django
- Browser: To be recorded during test execution
- Operating System: Windows
- Database: Existing project database configuration
- Test Data: Fictional accounts and sample records

## 6. Entry Criteria

- The application starts successfully.
- The relevant page can be accessed.
- Suitable fictional test data is available.
- The tester can record the expected and actual results.

## 7. Exit Criteria

- All planned test cases have been executed or assigned an appropriate status.
- Failed tests have been documented.
- Reproducible defects have been recorded with steps and evidence where appropriate.
- Test results have been summarized.
- No test is marked as passed without verification.

## 8. Test Status Definitions

- Not Run: Testing has not started.
- Pass: Actual behavior matches the expected result.
- Fail: Actual behavior differs from the expected result.
- Blocked: Testing cannot continue because of an obstacle.
- Not Testable: The feature is unavailable or cannot currently be tested.

## 9. Risks and Considerations

- Cycle predictions may be estimates and should not be treated as medical advice.
- Prediction accuracy depends on the available historical records and the implemented calculation logic.
- Deletion and editing tests must use fictional test data.
- Private health information, passwords, and real personal records must not be published in the portfolio.
- Existing application code must not be modified solely to make a test pass.

## 10. Deliverables

- Test plan
- Manual test cases
- Test execution report
- Bug reports
- Relevant test screenshots
- Final testing summary

## 11. Conclusion

This plan establishes the approach for manually testing LunaCycle's implemented features. Testing will be performed against the existing application, and results will be documented based on observed behavior and verified requirements.