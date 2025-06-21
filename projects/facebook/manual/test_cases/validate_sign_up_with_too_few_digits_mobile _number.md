# Test Case: Validate Sign Up With Too Few Digits in Mobile Number

**ID:** TC_FB_REG_028  
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

1. Enter a valid First name
2. Enter a valid Surname
3. Select a valid date of birth
4. Select a gender  
5. Enter a phone number with fewer than the required digits (e.g. 12345)
6. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
7. Click on the **Sign Up** button

---

**Expected Result:**  
- The system prevents registration
- A validation message is displayed indicating that the phone number is too short

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**    
- Standard mobile numbers usually require 10–15 digits depending on country
