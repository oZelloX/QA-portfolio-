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

1. Use `Tab` key to move to the First Name field and enter a valid name  
2. Use `Tab` to navigate to the Surname field and enter a valid surname  
3. Use `Tab` to move to the date of birth fields  
4. Use `Arrow` keys and `Enter` or `Space` to select Day, Month, and Year  
5. Use `Tab` to navigate to the gender selection  
6. Use `Arrow` keys and `Space` to choose a gender option  
7. Use `Tab` to navigate to Mobile/Email and Password fields and enter valid values  
8. Use `Tab` to move to the **Sign Up** button  
9. Press `Enter` to attempt registration

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
