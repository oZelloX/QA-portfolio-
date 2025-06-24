# Test Case: Verify Layout at 320px Screen Width

**ID:** TC_FB_ACC_016  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** Medium  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Page is fully loaded  
- Browser is in responsive mode set to 320px screen width (e.g., using Chrome DevTools)

---

**Test Steps:**

1. Open browser DevTools (F12 or right-click → Inspect)  
2. Enable responsive design mode  
3. Set screen width to **320px**  
4. Reload the Facebook registration page  
5. Scroll through the form and attempt to fill out each field  
6. Verify that all inputs, buttons, and labels are visible and functional  
7. Look for layout issues like overlapping, clipping, or horizontal scrolling

---

**Expected Result:**  
- All UI elements are properly aligned  
- No content is cut off  
- Horizontal scrolling is not required  
- Registration form remains fully usable

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- This simulates usage on smaller smartphones  
- Any layout failure may violate WCAG 2.1 (Success Criterion 1.4.10 – Reflow)
