# Test Case: Validate Sign Up With Gender Custom - He

**ID:** TC_FB_REG_013  
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
2. Select a valid date of birth
3. Select “Custom” as gender and ensure pronoun dropdown is displayed, then choose “They”
4. Enter a valid mobile phone number or email address 
5. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
6. Click on the **Sign Up** button

---

**Expected Result:**   
- The system accepts the provided gender as “Custom” with pronoun “They”
- A confirmation message is sent to the provided email or mobile number 
- User proceeds to the next step or sees a confirmation message

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Gender selection should persist after form submission
- When “Custom” is selected, a pronoun dropdown must appear
- The selected gender and pronoun should be stored in the user profile after registration


