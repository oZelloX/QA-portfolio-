# Bug Report: Keyboard Navigation Skips Interactive Elements on Registration Page

**ID:** BR_FB_ACC_001  
**Module:** Facebook – Registration  
**Reported by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-22  
**Severity:** High  
**Priority:** High  
**Type:** Accessibility / Keyboard Navigation  
**Status:** Open  

---

## 📍 Environment

- **URL:** [`https://www.facebook.com/r.php?entry_point=login`](https://www.facebook.com/r.php?entry_point=login)  
- **Browser:** Chrome (latest stable)  
- **OS:** macOS / Windows  
- **Zoom Level:** 100%  
- **Screen Reader:** *Not required to reproduce*

---

## ✅ Preconditions

- User is on the Facebook registration page  
- Page is fully loaded  
- Keyboard-only navigation is used (Tab/Shift+Tab)

---

## 🔁 Steps to Reproduce

1. Press `Tab` to start navigating from the **First Name** input field  
2. Continue pressing `Tab` through the form  
3. Observe which elements receive keyboard focus  

---

## ❌ Actual Result

- Keyboard focus **skips multiple interactive elements**, specifically:
  - **Gender selection** (radio buttons or dropdown)
  - **Sign Up** button  
  - **"Already have an account?"** link  
- After skipping these, focus jumps to the **browser’s address bar**, bypassing the remaining form controls  
- These elements are visible on the page but **not accessible via keyboard**

---

## ✅ Expected Result

- Every visible, interactive form element must be **reachable using Tab**  
- Focus should proceed logically through:
  - First Name → Surname → DOB → Gender → Email/Phone → Password → Sign Up → Existing Account Link  
- Focus must not skip or bypass active UI components

---

## 📌 Notes

- This is a **critical accessibility issue** affecting users who rely on keyboard navigation  
- It violates WCAG 2.1:  
  - **Success Criterion 2.1.1 – Keyboard**  
  - **Success Criterion 2.4.3 – Focus Order**

---

## 📎 Attachments

*Optional: Add screenshots or video if needed*
