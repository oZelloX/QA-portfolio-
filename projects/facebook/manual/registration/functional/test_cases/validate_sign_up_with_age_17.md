# Test Case: Validate Sign Up With Age 17 (Teen Account)

**ID:** TC_FB_REG_041  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-18  
**Priority:** Medium  
**Type:** Functional  
**Preconditions:**  
- User is on the Facebook registration page  
- Registration form is fully loaded

---

**Test Steps:**

1. Enter a valid First name
2. Enter a valid Surname
3. Select a date of birth that makes the user exactly 17 years old
4. Select a gender
5. Enter a valid email or mobile number 
6. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))
7. Click on the **Sign Up** button

---

**Expected Result:**   
- The system allows registration
- The account is created with appropriate settings for teen users (13–17)

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**
- This test validates the upper boundary of the teen account range (13–17)
- Age-related parental settings apply after registration, not during sign-up
