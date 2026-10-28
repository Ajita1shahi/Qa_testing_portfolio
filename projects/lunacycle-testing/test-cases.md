# LunaCycle — Manual Test Cases

## 1. Test Information

- Project: LunaCycle
- Test Plan ID: LC-TP-001
- Testing Type: Manual Functional Testing
- Initial Status: Not Run

## 2. Authentication Testing

### TC_AUTH_001 — Login with Valid Credentials
- Preconditions: A test account exists.
- Steps:
  1. Open LunaCycle.
  2. Enter valid login credentials.
  3. Click Login.
- Expected Result: The user should log in and reach the appropriate page.
- Actual Result: logged in succesfully.
- Status: Pass

### TC_AUTH_002 — Login with Invalid Credentials
- Preconditions: The login page is accessible.
- Steps:
  1. Enter an incorrect username or password.
  2. Click Login.
- Expected Result: Access should be denied with an appropriate error message.
- Actual Result: Access should be denied and an appropriate error message "Invalid username and password" occured.
- Status: Pass

## 3. Period Record Testing

### TC_PERIOD_001 — Add a Valid Period Record
- Preconditions: The user is logged in.
- Steps:
  1. Open the period tracking page.
  2. Enter a valid start date and any other required fields.
  3. Save the record.
- Expected Result: The record should be saved and displayed correctly.
- Actual Result:The period record was saved successfully .
- Status: Pass

### TC_PERIOD_002 — Validate End Date Before Start Date
- Preconditions: The user is logged in and can add or edit a period record.
- Steps:
  1. Enter an end date earlier than the start date.
  2. Submit the form.
- Expected Result: The application should reject the invalid date range or display an appropriate validation message.
- Actual Result:- Actual Result: The application rejected the invalid date range and displayed the message "The end date cannot be before the start date."
- Status: Pass

### TC_PERIOD_003 — Edit an Existing Period Record
- Preconditions: At least one test period record exists.
- Steps:
  1. Open an existing record.
  2. Change one of its editable fields.
  3. Save the changes.
- Expected Result: The updated information should be saved and displayed correctly.
- Actual Result: The new record was updated.
- Status: Pass

### TC_PERIOD_004 — Delete a Period Record
- Preconditions: A disposable test record exists.
- Steps:
  1. Select the test record.
  2. Use the available delete action.
  3. Confirm deletion if prompted.
- Expected Result: The selected record should be removed, and unrelated records should remain unchanged.
- Actual Result: The period record was deleted.
- Status: Pass


## 4. Calendar and Prediction Testing

### TC_CAL_001 — View Period Records on Calendar
- Preconditions: At least one period record exists.
- Steps:
  1. Open the calendar.
  2. Navigate to the month containing the test record.
- Expected Result: The calendar should display the relevant saved dates correctly.
- Actual Result: It successfully navigate the period date in calendar.
- Status: Pass

### TC_CAL_002 — Check Predictions with Available History
- Preconditions: The test account has sufficient period history for the application's prediction logic.
- Steps:
  1. Open the calendar or prediction page.
  2. Review the predicted dates.
- Expected Result: Predictions should follow the application's implemented calculation logic and available history.
- Actual Result: It follow the pplication's implemented calculation logic and available history.
- Status: Pass

## 5. Symptom Journal Testing

### TC_SYM_001 — Save a Symptom Entry
- Preconditions: The user is logged in and the journal feature is available.
- Steps:
  1. Open the symptom journal.
  2. Enter sample symptoms and any required information.
  3. Save the entry.
- Expected Result: The entry should be saved and displayed correctly.
- Actual Result: The entry is saved and displayed correctly.
- Status: Pass

### TC_SYM_002 — Submit Journal Entry with Optional Fields Empty

- Preconditions: The user is logged in and the symptom journal form is available.
- Steps:
  1. Open the symptom journal.
  2. Enter a date.
  3. Leave the other fields empty.
  4. Submit the form.
- Expected Result: The application should handle empty optional fields according to its requirements and save the entry if only the date is required.
- Actual Result: The journal entry was saved successfully with only the date filled in.
- Status: Pass, pending confirmation that the other fields are optional.

## 6. Insights and Charts Testing

### TC_INS_001 — View Insights
- Preconditions: The account contains suitable sample data.
- Steps:
  1. Open the insights page.
  2. Review the displayed summaries and charts.
- Expected Result: The page should load, and the displayed values should match the underlying data and implemented calculation logic.
- Actual Result:The page loaded, and the displayed values match the underlying data and implemented calculation logic.
- Status: Pass

## 7. Execution Summary

- Total Test Cases: 11
- Passed: 11
- Failed: 0
- Blocked: 0


