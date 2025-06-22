# Test Case: Verify Focus Moves to Error Message After Submission Failure

**ID:** TC_FB_ACC_013  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded  
- At least one required field is left blank  
- Screen reader is optional but recommended

---

**Test Steps:**

1. Navigate through the form using only the keyboard (Tab)  
2. Leave at least one required field (e.g., Surname or Email) empty  
3. Press the **Sign Up** button  
4. Observe whether the focus moves automatically to the corresponding error message or error summary section  
5. Optionally, observe screen reader behavior

---

**Expected Result:**  
- Focus is shifted to the error message or error summary  
- The user is immediately made aware of the problem location without manually searching for it

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- If the focus remains on the **Sign Up** button, user may not notice the issue  
- This violates WCAG 2.1 (Success Criterion 3.3.1 – Error Identification) and 2.4.3 – Focus Order
