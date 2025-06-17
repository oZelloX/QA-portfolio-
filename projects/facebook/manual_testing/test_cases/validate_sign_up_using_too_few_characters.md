# Test Case: Validate Sign Up Using Too Few Characters

**ID:** TC_FB_REG_024  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-17  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- User is on the Facebook registration page  
- Registration form is fully loaded

---

**Test Steps:**

1. Enter1 character in the First name field
2. Select a valid date of birth
3. Select a gender  
4. Enter a valid mobile phone number or email address
5. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
6. Click on the **Sign Up** button

---

**Expected Result:**  
- The system accepts very short but valid names and surnames
- A confirmation message is sent to the provided email or mobile number 
- User proceeds to the next step or sees a confirmation message

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**    
- Minimum accepted character count for name fields should be validated  
- No validation error should appear for short but valid entries

