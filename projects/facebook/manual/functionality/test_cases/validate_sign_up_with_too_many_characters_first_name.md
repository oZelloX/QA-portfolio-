# Test Case: Validate Sign Up With Too Many Characters in First Name

**ID:** TC_FB_REG_026  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-17  
**Priority:** Medium  
**Type:** Negative Boundary  
**Preconditions:**  
- User is on the Facebook registration page  
- Registration form is fully loaded

---

**Test Steps:**

1. Enter a First name with more than 50 characters
2. Enter a valid Surname
3. Select a valid date of birth
4. Select a gender  
5. Enter a valid mobile phone number or email address
6. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
7. Click on the **Sign Up** button

---

**Expected Result:**  
- The system prevents registration
- Validation message explains character limit

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**    
- Maximum First name length should typically be up to 50 characters
