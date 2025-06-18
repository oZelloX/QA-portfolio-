# Test Case: Validate Sign Up With Age Between 13 and 17 (Teen Account)

**ID:** TC_FB_REG_007  
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

1. Enter a valid first name and surname  
2. Select a date of birth that makes the user exactly 13 years old (boundary value)
3. Select a gender  
4. Enter a valid mobile phone number or email address 
5. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
6. Click on the **Sign Up** button

---

**Expected Result:**   
- The system accepts the provided age between 13 and 17  
- A confirmation message is sent to the provided email or mobile number
- User proceeds to the next step or sees a confirmation message

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- 
- This test also covers lower boundary for valid age (13 years)
- Facebook’s policy requires users to be at least 13 years old
- Age-related parental settings apply after registration, not during sign-up
