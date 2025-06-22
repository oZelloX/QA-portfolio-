# Test Case: Verify Focus Visibility on All Focusable Elements

**ID:** TC_FB_ACC_003  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded  
- Mouse and trackpad are not used during the test  

---

**Test Steps:**

1. Press the `Tab` key repeatedly to move through all focusable elements on the registration page  
2. Observe the focus indicator (outline, border, glow, etc.)  
3. Use `Shift + Tab` to reverse navigate and repeat observation  
4. Confirm that every interactive element shows visible focus

---

**Expected Result:**  
- All focusable elements clearly indicate when they are focused  
- Focus indicator is always visible and distinguishable from the rest of the UI  
- Focus is not lost or hidden at any point

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Lack of visible focus is a violation of WCAG 2.1 (Success Criterion 2.4.7 – Focus Visible)  
- Common elements to verify: input fields, dropdowns, radio buttons, Sign Up button, links
