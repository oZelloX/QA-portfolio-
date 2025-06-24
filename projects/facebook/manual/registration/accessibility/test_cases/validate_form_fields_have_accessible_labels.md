# Test Case: Verify All Form Fields Have Associated Labels

**ID:** TC_FB_ACC_005  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Page is fully loaded  
- Screen reader is active (e.g., NVDA, VoiceOver, JAWS)

---

**Test Steps:**

1. Navigate through each form field using screen reader navigation keys (e.g., Tab, Arrow keys)  
2. Listen to how the screen reader announces each input field  
3. Confirm that each field is announced with a meaningful label (e.g., "First Name", "Mobile Number", etc.)  
4. Verify that there is no ambiguity or missing field name

---

**Expected Result:**  
- Each input field is announced with a clear and descriptive label  
- Labels are either associated via `<label for="id">`, `aria-label`, or `aria-labelledby`  
- No field is announced as “edit”, “blank”, or similar without context

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Missing or unclear labels make the form unusable for screen reader users  
- This is a violation of WCAG 2.1 (Success Criterion 1.3.1 – Info and Relationships)
