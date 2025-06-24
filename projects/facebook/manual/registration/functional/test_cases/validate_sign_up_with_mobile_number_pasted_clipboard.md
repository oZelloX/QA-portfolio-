# Test Case: Validate Sign Up With Mobile Number Pasted from Clipboard

**ID:** TC_FB_REG_031  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-17  
**Priority:** Medium    
**Type:** Functional  
**Preconditions:**  
- User is on the Facebook registration page  ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Registration form is fully loaded

---

**Test Steps:**

1. Enter a valid First name
2. Enter a valid Surname
3. Select a valid date of birth
4. Select a gender  
5. Paste the phone number into the mobile number field using Ctrl+V or right-click paste
6. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
7. Click on the **Sign Up** button

---

**Expected Result:**  
- The system correctly processes the pasted number as input
-	No formatting or validation issues occur if the number is valid

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**    
- The field should support paste operations without breaking validation rules
