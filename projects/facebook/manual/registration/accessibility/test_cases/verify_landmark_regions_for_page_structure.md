# Test Case: Verify Use of Landmark Regions for Page Structure

**ID:** TC_FB_ACC_018  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** Medium  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Page is fully loaded  
- Developer Tools or screen reader is available

---

**Test Steps:**

1. Open browser Developer Tools or accessibility inspector  
2. Check the page structure for semantic landmarks: `<main>`, `<nav>`, `<header>`, `<footer>`, etc.  
3. Verify that main content is wrapped in a `<main>` tag  
4. Confirm that navigation (if any) is inside a `<nav>` tag  
5. Use a screen reader to test if landmark regions are announced correctly (e.g., "main region", "navigation region")

---

**Expected Result:**  
- Semantic landmarks (`main`, `nav`, `header`, etc.) are used where appropriate  
- Screen readers correctly identify and announce page regions  
- Landmark tags reflect the actual structure and purpose of the content

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Proper landmark regions improve navigation for screen reader users  
- Missing or misused landmarks violate WCAG 2.1 (Success Criterion 1.3.1 – Info and Relationships)
