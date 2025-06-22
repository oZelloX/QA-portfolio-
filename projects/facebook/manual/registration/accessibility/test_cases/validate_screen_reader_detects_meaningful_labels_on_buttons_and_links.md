# Test Case: Verify Buttons and Links Have Meaningful Text

**ID:** TC_FB_ACC_007  
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

1. Use the screen reader to navigate through all buttons and links on the registration page  
2. Observe how each button and link is announced  
3. Confirm that each one includes a meaningful and descriptive label (e.g., "Sign Up", not "Click here")  
4. Pay attention to any icons or visual-only elements acting as buttons or links — verify they have accessible names

---

**Expected Result:**  
- All buttons and links are announced with clear, meaningful text  
- No element is announced as “button”, “link”, or “click here” without context  
- Icon-only buttons (if any) have proper `aria-label` or `aria-labelledby`

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Meaningless or generic labels confuse screen reader users and reduce navigability  
- This is a violation of WCAG 2.1 (Success Criterion 2.4.4 – Link Purpose (In Context))
