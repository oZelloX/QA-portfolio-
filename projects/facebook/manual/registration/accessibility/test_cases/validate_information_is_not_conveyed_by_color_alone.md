# Test Case: Verify Information Is Not Conveyed by Color Alone

**ID:** TC_FB_ACC_011  
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

1. Inspect all visible form fields, status indicators, and error messages  
2. Attempt to submit the form with at least one required field left empty or invalid  
3. Observe how the form communicates the error  
4. Verify that the error is not conveyed using color only (e.g., red border or text alone)  
5. Check for additional indicators: icon, text explanation, or ARIA attributes

---

**Expected Result:**  
- All status or error messages are communicated using **color + text and/or icon**  
- No critical information is presented **only** through color

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Users with color vision deficiency may not perceive red, green, or other color cues  
- Using color alone to convey meaning violates WCAG 2.1 (Success Criterion 1.4.1 – Use of Color)
