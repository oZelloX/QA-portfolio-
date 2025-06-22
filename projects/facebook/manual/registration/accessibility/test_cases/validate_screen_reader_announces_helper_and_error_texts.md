# Test Case: Verify Descriptive Texts Are Announced via aria-describedby

**ID:** TC_FB_ACC_006  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded  
- Screen reader is active (e.g., NVDA, VoiceOver, JAWS)

---

**Test Steps:**

1. Navigate to input fields that include helper or instruction text (e.g., password field, email field)  
2. Observe what the screen reader announces upon entering the field  
3. Trigger a validation error (e.g., submit the form with required field empty or invalid password)  
4. Observe whether the screen reader announces the associated error message  
5. Verify that both helper text and error message are programmatically connected via `aria-describedby`

---

**Expected Result:**  
- Screen reader announces all relevant helper texts when the user focuses on the field  
- Error messages are announced immediately after triggering validation  
- All texts are properly associated with the input fields via `aria-describedby` or `aria-live`

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Missing or unlinked descriptions result in critical loss of information for screen reader users  
- This is a violation of WCAG 2.1 (Success Criterion 1.3.1 – Info and Relationships)
