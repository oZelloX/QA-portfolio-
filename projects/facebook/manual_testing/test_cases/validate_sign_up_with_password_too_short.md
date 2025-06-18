# Test Case: Validate Sign Up With Password of Insufficient Length

**ID:** TC_FB_REG_035  
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
3. Select a valid date of birth
4. Select a gender
5. Enter a valid email or mobile number 
6. Enter a password with fewer than 6 characters (e.g. “Abc1!”) 
7. Click on the **Sign Up** button

---

**Expected Result:**   
- The system prevents registration
- A validation message is displayed indicating that the password is too short

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**
- Other password criteria are intentionally met to isolate length validation
- Passwords must meet minimum length requirements (typically 6+ characters) for security reasons.
