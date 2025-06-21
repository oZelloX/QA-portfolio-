# Test Case: Validate Sign Up Using a Cyrillic Letters for Name and Surname

**ID:** TC_FB_REG_003  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-16  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- User is on the Facebook registration page  
- Registration form is fully loaded

---

**Test Steps:**

1. Enter a valid first name and surname using Cyrillic characters (e.g., Алексей Иванов)  
2. Select a valid date of birth
3. Select a gender  
4. Enter a valid mobile phone number or email address
5. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
6. Click on the **Sign Up** button

---

**Expected Result:**  
- The system accepts Cyrillic input for name and surname
- A confirmation message is sent to the provided email or mobile number 
- User proceeds to the next step or sees a confirmation message

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**    
- Verify that no character encoding issues occur when using non-Latin characters  
- Ensure the input does not trigger any validation errors specific to character sets

