# Test Case: Validate Sign Up With Password Without Letters

**ID:** TC_FB_REG_036  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-18  
**Priority:** Medium  
**Type:** Negative Functional  
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
6. Enter a password that contains only digits and special characters (e.g. “1234!@”) 
7. Click on the **Sign Up** button

---

**Expected Result:**   
- The system prevents registration
- A validation message is displayed indicating that the password must include letters

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**
- Letters (a–z, A–Z) are required to ensure password complexity and security
