# Test Case: Validate Sign Up Using Only Keyboard

**ID:** TC_FB_ACC_004  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded  
- Mouse and trackpad are not used during the test  

---

**Test Steps:**

1. Press the `Tab` key to move to the First Name field and enter a valid name  
2. Continue using `Tab` to navigate and fill in all required fields  
3. Use `Arrow` keys and `Space` to select gender option  
4. Navigate to the **Sign Up** button  
5. Press `Enter` to attempt registration

---

**Expected Result:**  
- User is able to complete and submit the registration form using only the keyboard  
- All required fields are filled, and form submits successfully  
- No mouse or trackpad interaction is necessary

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**    
- Focus must reach all required fields and the submit button
- Inability to complete the registration process without using a pointing device is a violation of WCAG 2.1 (Success Criterion 2.1.1 – Keyboard)
