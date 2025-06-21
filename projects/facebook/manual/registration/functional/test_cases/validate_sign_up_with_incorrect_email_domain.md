# Test Case: Validate Sign Up With Incorrect Email Domain

**ID:** TC_FB_REG_033  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-17  
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
5. Enter an email with an incorrect or non-existent domain (e.g. user@invalid_domain.xyz)
6. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
7. Click on the **Sign Up** button

---

**Expected Result:**  
- The system prevents registration
- 	A validation message is displayed indicating that the email domain is incorrect or unsupported

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**    
- System should validate domain format and existence where applicable
