# Bug Report: Keyboard Navigation Skips Interactive Elements on Registration Page

**ID:** BR_FB_ACC_001  
**Module:** Facebook – Registration  
**Reported by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-24  
**Severity:** High  
**Priority:** High  
**Type:** Accessibility – Keyboard Navigation  
**Status:** Open  

---

## Environment

- **URL:** [https://www.facebook.com/r.php?entry_point=login](https://www.facebook.com/r.php?entry_point=login)  
- **Browser:** Safari 18.5 (20621.2.5.11.8)  
- **OS:** macOS Sequoia 15.5  

---

## Preconditions

- User is on the registration page  
- Page is fully loaded  
- Navigation is performed using keyboard only (`Tab` / `Shift+Tab`)

---

## Steps to Reproduce

1. Press `Tab` to focus the **First Name** field  
2. Continue pressing `Tab` to navigate through the form  
3. Observe focus behavior on all form elements  

---

## Actual Result

- Keyboard focus **skips**:
  - **Gender selection** (radio buttons / dropdown)  
  - **Sign Up** button  
  - **"Already have an account?"** link  
- Focus jumps to the **browser address bar**, skipping critical elements  
- These elements are visible but **not reachable** via keyboard  

---

## Expected Result

- Keyboard focus should sequentially move through **all interactive elements**:
  - First Name → Surname → DOB → Gender → Email/Phone → Password → Sign Up → Existing Account Link  
- **No focus skips** should occur  

---

## Notes

- Critical accessibility failure  
- Violates:
  - WCAG 2.1 – **2.1.1 Keyboard**  
  - WCAG 2.1 – **2.4.3 Focus Order**  

---

##  Attachments

- [Watch Bug Reproduction Video (Loom)](https://www.loom.com/share/2c3a1d86ae974d439b70152f97d7ca45?sid=6b28c488-0de0-466b-9c64-ff46195d9a76)

