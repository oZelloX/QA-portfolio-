# Test Case: Verify Checkbox and Radio Groups Are Announced Correctly

**ID:** TC_FB_ACC_008  
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

1. Use the screen reader to navigate to the gender selection radio buttons  
2. Observe how the group and individual options are announced  
3. Confirm that the screen reader identifies the group label (e.g., “Gender”) and each option (e.g., “Male”, “Female”, “Custom”)  
4. Use arrow keys to move between options and listen to how state (selected/not selected) is read  
5. If "Custom" is selected, confirm that the additional input field becomes available and announced

---

**Expected Result:**  
- Screen reader announces the group name (e.g., “Gender”) when entering the radio group  
- Each option is announced with its label and current state  
- Navigation between options is possible with arrow keys  
- Any dynamic field (like custom gender input) is also read when visible

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Radio and checkbox groups must have a programmatically defined group name (e.g., via `<fieldset>` and `<legend>`)  
- Failure to identify group context violates WCAG 2.1 (Success Criterion 1.3.1 – Info and Relationships)
