# Test Case: Verify Error Messages Are Announced by Screen Readers

**ID:** TC_FB_ACC_012  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  ([`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login))
- Page is fully loaded  
- Screen reader is enabled and running

---

**Test Steps:**

1. Enable screen reader (e.g., NVDA on Windows or VoiceOver on Mac)  
2. Navigate through the registration form using Tab or arrow keys  
3. Leave at least one required field empty  
4. Press the **Sign Up** button to trigger validation  
5. Observe whether the screen reader announces the error message for the empty field

---

**Expected Result:**  
- The screen reader should automatically announce the relevant error message  
- The error text should be associated with the input field using `aria-describedby`, `aria-live`, or similar techniques

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- If the screen reader doesn’t announce the error, it’s a serious accessibility failure  
- This violates WCAG 2.1 (Success Criterion 3.3.1 – Error Identification)
