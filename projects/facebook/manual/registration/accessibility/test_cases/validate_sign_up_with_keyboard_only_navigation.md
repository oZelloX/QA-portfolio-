# Test Case: Verify All Interactive Elements Are Reachable via Keyboard

**ID:** TC_FB_ACC_001  
**Module:** Facebook – Registration  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-21  
**Priority:** High  
**Type:** Accessibility  
**Preconditions:**  
- User is on the Facebook registration page  
- Page is fully loaded  
- Mouse and trackpad are not used during the test  

---

**Test Steps:**

1. Press the `Tab` key repeatedly to navigate through the page  
2. Observe focus movement on all interactive elements (input fields, radio buttons, dropdowns, buttons, links)  
3. Use `Shift + Tab` to reverse navigate  
4. Attempt to activate buttons using the `Enter` or `Space` key  

---

**Expected Result:**  
- All interactive elements are reachable and focusable using the keyboard  
- Focus is visible and not lost  
- Buttons are activated correctly via `Enter` or `Space`

---

**Actual Result:**  
_To be filled after test execution_

---

**Notes:**  
- Check that no element requires a mouse to interact  
- Include dropdown and gender selection in the check
