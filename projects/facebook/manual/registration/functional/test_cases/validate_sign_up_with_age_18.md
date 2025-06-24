# Test Case: Validate Sign Up With Age 18

**ID:** TC_FB_REG_042  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-18  
**Priority:** Medium  
**Type:** Functional  
**Preconditions:**  
- User is on the Facebook registration page  ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Registration form is fully loaded

---

**Test Steps:**

1. Enter a valid First name
2. Enter a valid Surname
3. Select a date of birth that makes the user exactly 18 years old
4. Select a gender
5. Enter a valid email or mobile number 
6. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))
7. Click on the **Sign Up** button

---

**Expected Result:**   
- The system allows registration
- A standard adult account is created

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**
- This test validates the lower boundary of adult account eligibility (18+ years)
- Adult accounts have access to the full set of Facebook features without teen-specific restrictions
