# Test Case: Validate Sign Up Using an Email Address

**ID:** TC_FB_REG_002  
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

1. Enter a valid First name
2. Enter a valid Surname  
2. Select a valid date of birth that makes the user 50 years old
3. Select a gender  
4. Enter a valid email address
5. Enter a secure password (Enter a combination of at least six numbers, letters and punctuation marks(such as ! and &))  
6. Click on the **Sign Up** button

---

**Expected Result:**  
- The system accepts the email address  
- A confirmation email is sent to the provided email
- User proceeds to the next step or sees a confirmation message

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**
- This test also confirms that users aged 50 can register successfully
- The email address must follow a valid format (e.g., username@example.com)
- The email address must not already be registered
