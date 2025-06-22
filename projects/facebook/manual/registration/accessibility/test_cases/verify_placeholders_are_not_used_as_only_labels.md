# Test Case: Verify That Placeholder Text Is Not Used as the Only Label

**ID:** TC_FB_ACC_017  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page (`https://www.facebook.com/r.php?entry_point=login`)  
- Page is fully loaded

---

**Test Steps:**

1. Inspect each input field in the registration form  
2. Check whether there is a visible label (e.g., "First name") outside of the input field  
3. If no visible label is found, check if placeholder text is being used instead  
4. Verify whether the placeholder disappears on focus or typing  
5. Confirm that screen readers correctly announce each field’s purpose

---

**Expected Result:**  
- Each input field must have a visible label (not just placeholder text)  
- Placeholders, if used, are supplemental and not the only form of labeling  
- Screen readers announce the field meaningfully

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Placeholder text is **not a substitute** for a proper label  
- Relying solely on placeholders violates WCAG 2.1 (Success Criterion 3.3.2 – Labels or Instructions)
