# Test Case: Verify Text and UI Elements Meet Minimum Contrast Requirements

**ID:** TC_FB_ACC_009  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded  
- Contrast checking tool is available (e.g., axe DevTools, WCAG Contrast Checker)

---

**Test Steps:**

1. Open a contrast-checking tool (such as axe DevTools or WCAG Contrast Checker)  
2. Inspect all visible text elements on the registration page (e.g., field labels, placeholders, buttons, links)  
3. Measure color contrast between text and background for each element  
4. Verify that contrast ratio meets WCAG 2.1 AA minimum:  
   - 4.5:1 for normal text  
   - 3:1 for large text (≥18pt regular or ≥14pt bold)  
5. Pay special attention to disabled fields, placeholder text, and subtle elements like links or tooltips

---

**Expected Result:**  
- All text elements meet or exceed the minimum contrast ratio requirements  
- No content is hard to read due to low contrast

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Insufficient contrast can render text unreadable for users with low vision  
- This is a violation of WCAG 2.1 (Success Criterion 1.4.3 – Contrast (Minimum))
