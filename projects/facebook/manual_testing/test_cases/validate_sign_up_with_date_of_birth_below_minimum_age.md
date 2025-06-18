# Test Case: Validate Sign Up With Date of Birth Below Minimum Age

**ID:** TC_FB_REG_039  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-18  
**Priority:** Medium  
**Type:** Negative Boundary  
**Preconditions:**  
- User is on the Facebook registration page  
- Registration form is fully loaded

---

**Test Steps:**

1. Enter a valid First name
2. Enter a valid Surname
3. Select a date of birth that makes the user under 13 years old
4. Select a gender
5. Enter a valid email or mobile number 
6. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))
7. Click on the **Sign Up** button

---

**Expected Result:**   
- The system prevents registration
-  A validation message is displayed indicating that the user does not meet the minimum age requirement

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**
- - Facebook requires users to be at least 13 years old to register
