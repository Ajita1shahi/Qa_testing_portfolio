
# Login Testing of SauceDemo

## 1. Project Overview

**Application:** SauceDemo  
**Website:** https://www.saucedemo.com/  
**Module:** Login  
**Testing Type:** Manual Functional Testing  
**Objective:** To verify that the login functionality behaves correctly with valid and invalid credentials.

## 2. Test Environment

- Browser: Google Chrome
- Testing Type: Manual Testing
- Environment: Public demo application
- Test Status: Not Executed

## 3. Test Cases

| Test Case ID | Test Scenario | Test Steps | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC_LOGIN_001 | Login with valid credentials | 1. Open the website. 2. Enter username and password. 3. Click Login. | standard_user / secret_sauce | User should log in successfully and see the products page. | The page run succesfully | pass |
| TC_LOGIN_002 | Login with an invalid username | 1. Open the website. 2. Enter an invalid username. 3. Enter the valid password. 4. Click Login. | abc_user / secret_sauce | An appropriate error message should appear and login should be denied. | Appropriate messaged 'Username and password do not match any user in this service'displayed. | pass |
| TC_LOGIN_003 | Login with an invalid password | 1. Open the website. 2. Enter the valid username. 3. Enter an incorrect password. 4. Click Login. | standard_user / ajita123 | An appropriate error message should appear and login should be denied. | Appropriate messaged 'Username and password do not match any user in this service'displayed.| pass |
| TC_LOGIN_004 | Login with both fields empty | 1. Open the website. 2. Leave both fields empty. 3. Click Login. | Username: blank; Password: blank | The application should prevent login and display a validation message. | Appropriate message'Epic sadface: Username is required' | pass |
| TC_LOGIN_005 | Login with an empty username | 1. Open the website. 2. Leave username empty. 3. Enter a password. 4. Click Login. | Username: blank; Password: secret_sauce | The application should prevent login and display an appropriate validation message. |Appropriate message'Epic sadface: Username is required'  | pass |
| TC_LOGIN_006 | Login with an empty password | 1. Open the website. 2. Enter a valid username. 3. Leave password empty. 4. Click Login. | Username: standard_user; Password: blank | The application should prevent login and display an appropriate validation message. | Appropriate message'Epic sadface: Username is required' | pass |
| TC_LOGIN_007 | Verify password masking | 1. Open the website. 2. Enter a password in the password field. | Password: secret_sauce | The password should be masked rather than displayed as readable text. | Password is masked|Pass|
| TC_LOGIN_008 | Login with a locked-out account | 1. Open the website. 2. Enter the locked-out user's credentials. 3. Click Login. | locked_out_user / secret_sauce | Login should be denied and an appropriate error message should be displayed. | Appropriate message 'Epic sadface: Sorry, this user has been locked out.'| Pass|

## 4. Test Execution Summary

Total Test Cases: 8  
Passed: 8 
Failed: 0  
Blocked: 0  


## 5. Conclusion
These test cases cover valid login, invalid credentials, missing input, password masking, and account lockout behavior. They will be executed manually to evaluate the login module of the SauceDemo application.
