# Test Case: Verify Placeholder Text Is Not Used as the Only Label

**ID:** TC_FB_ACC_010  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Page is fully loaded  
- Visual inspection and/or screen reader is available

---

**Test Steps:**

1. Visually inspect all input fields on the registration form  
2. Check if any field uses only placeholder text (e.g., light grey text inside the input) to indicate its purpose  
3. Verify whether a visible label is present outside the input field  
4. Use a screen reader to navigate through the fields  
5. Observe if field names are still announced after typing into the field (i.e., label persists)

---

**Expected Result:**  
- All input fields have visible labels outside of the input box  
- Placeholder text is never used as the only method of identifying the field  
- Screen reader users can still understand each field after typing starts

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Placeholder text disappears when users type, and it is often low-contrast  
- Relying on it as the only label violates WCAG 2.1 (Success Criterion 3.3.2 – Labels or Instructions)
