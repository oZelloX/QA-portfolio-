# Test Case: Verify Proper Use of ARIA Roles on Form Elements

**ID:** TC_FB_ACC_017  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** Medium  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Page is fully loaded  
- Developer tools or screen reader is available

---

**Test Steps:**

1. Open browser Developer Tools or use an accessibility extension  
2. Inspect all input elements (e.g., text fields, radio buttons, dropdowns, buttons)  
3. Check for appropriate ARIA roles (`textbox`, `button`, `radiogroup`, etc.)  
4. Verify that these roles match the actual function of the element  
5. If applicable, check for additional ARIA attributes (e.g., `aria-required`, `aria-invalid`)

---

**Expected Result:**  
- All interactive form elements have correct ARIA roles  
- Roles accurately describe the purpose and behavior of the elements  
- No redundant or incorrect ARIA attributes are present

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Incorrect or missing ARIA roles may confuse assistive technologies  
- Misuse of roles violates WCAG 2.1 (Success Criterion 4.1.2 – Name, Role, Value)
