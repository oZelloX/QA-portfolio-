# Test Case: Verify Layout at 320px Screen Width

**ID:** TC_FB_ACC_016  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** Medium  
**Type:** Accessibility  
**Preconditions:**  
- User is viewing the Facebook registration page  
- Browser window is resized to 320px width  
- Page is fully loaded

---

**Test Steps:**

1. Resize the browser window to 320px width  
   _(use responsive mode in DevTools or an actual mobile device)_  
2. Scroll through the registration form  
3. Attempt to enter values in each field  
4. Check whether buttons, labels, and inputs remain visible and functional  
5. Observe for layout issues: overlapping, cut-off elements, or unusable inputs

---

**Expected Result:**  
- All elements remain visible and properly aligned  
- No horizontal scrolling required  
- Labels and fields are readable and not clipped  
- Page remains usable on small screens

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- 320px width simulates smaller smartphones and must be supported without layout issues  
- This test helps verify compliance with WCAG 2.1 (Success Criterion 1.4.10 – Reflow)
