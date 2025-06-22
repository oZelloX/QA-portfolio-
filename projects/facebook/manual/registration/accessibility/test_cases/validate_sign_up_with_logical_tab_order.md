# Test Case: Verify Logical Tab Order Across Form Fields

**ID:** TC_FB_ACC_002  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-21  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded  
- Mouse and trackpad are not used during the test  

---

**Test Steps:**

1. Press the `Tab` key repeatedly to navigate through each interactive element  
2. Observe the order of focus movement across fields:  
   - First Name  
   - Surname
   - Date of birth (day, month, year)
   - Gender selection
   - Mobile/email  
   - New password  
   - Sign Up button  
   - Already have an account? link

---

**Expected Result:**  
- Focus moves in a logical, top-to-bottom, left-to-right order  
- No unexpected jumps or loops in the tab sequence  
- No interactive element is skipped

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- If focus returns to the beginning or skips gender selection, this is a critical accessibility bug
