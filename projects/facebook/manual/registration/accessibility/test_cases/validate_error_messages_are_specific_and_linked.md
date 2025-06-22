# Test Case: Verify Error Messages Are Specific and Linked to Corresponding Fields

**ID:** TC_FB_ACC_014  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded

---

**Test Steps:**

1. Use Tab to navigate through the form  
2. Leave one or more required fields empty (e.g., Surname, Email)  
3. Press the **Sign Up** button to trigger validation  
4. Observe the error messages displayed  
5. Check if the message:
   - Clearly describes what’s wrong
   - Is positioned next to the corresponding field
   - Is programmatically linked to the field (e.g., `aria-describedby`)

---

**Expected Result:**  
- Each error message is specific (e.g., "Please enter your surname" vs. generic "Field is required")  
- Each message is **visually and programmatically** associated with its input field

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Vague or misplaced error messages confuse all users — not just those using assistive tech  
- This is a violation of WCAG 2.1 (Success Criterion 3.3.1 – Error Identification and 3.3.2 – Labels or Instructions)
