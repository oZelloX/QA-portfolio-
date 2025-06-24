# Test Case: Verify Page Functionality at 200% Zoom

**ID:** TC_FB_ACC_015  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** Medium  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Page is fully loaded  
- Browser zoom level is set to 200%

---

**Test Steps:**

1. Set browser zoom level to 200% (use browser settings or Ctrl/Cmd + Plus key)  
2. Scroll through the entire registration form  
3. Attempt to complete the form using keyboard or mouse  
4. Observe whether all fields, labels, and buttons are accessible and readable  
5. Check for horizontal scrolling, overlapping elements, or broken layout

---

**Expected Result:**  
- Page content remains readable and usable  
- No overlapping UI, broken layout, or inaccessible elements  
- Horizontal scrolling is minimized or absent  
- Registration form can be completed normally

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- At 200% zoom, all content must be visible without breaking the layout or obscuring elements  
- This test aligns with WCAG 2.1 (Success Criterion 1.4.4 – Resize Text)
