facebook_registration/
├── manual/
│   ├── functionality/
│   │   ├── checklist/
│   │   ├── test_cases/
│   │   └── README.md
│   ├── accessibility/
│   │   ├── checklist/
│   │   ├── test_cases/
│   │   └── README.md
│   ├── usability/
│   │   ├── checklist/
│   │   ├── test_cases/
│   │   └── README.md
│   ├── localization/
│   │   ├── checklist/
│   │   ├── test_cases/
│   │   └── README.md
│   ├── compatibility/
│   │   ├── checklist/
│   │   ├── test_cases/
│   │   └── README.md
│   └── README.md  ← обзор всех ручных направлений

├── automation/
│   ├── functionality/
│   │   ├── test_suites/
│   │   ├── scripts/
│   │   └── README.md
│   ├── api/
│   │   ├── collections/
│   │   ├── scripts/
│   │   └── README.md
│   └── README.md  ← обзор автоматизации

├── performance/
│   ├── load_tests/
│   ├── stress_tests/
│   └── README.md

├── security/
│   ├── checklist/
│   ├── reports/
│   └── README.md

└── README.md  ← главное описание проекта  












# Facebook Registration – Accessibility Testing Checklist

## ♿ Keyboard Navigation
- [ ] Validate that all form fields are reachable via the Tab key
- [ ] Validate correct tab order through all interactive elements
- [ ] Validate that focus is visibly indicated on all focusable elements
- [ ] Validate that Shift+Tab allows reverse navigation

## 🔊 Screen Reader Compatibility
- [ ] Validate that each form field has an associated and properly read label
- [ ] Validate that error messages are announced after invalid input
- [ ] Validate that buttons and links have descriptive accessible names
- [ ] Validate that screen reader can detect required fields

## 🎨 Visual Clarity & Contrast
- [ ] Validate sufficient color contrast between text and background
- [ ] Validate that input fields and buttons are distinguishable without relying solely on color
- [ ] Validate that focus indicators are visible to users with low vision

## 🧩 Other Accessibility Features
- [ ] Validate zoom functionality up to 200% without layout breakage
- [ ] Validate support for high contrast mode (system setting)
- [ ] Validate that form fields do not rely on placeholder-only labeling  
 











# Facebook Registration – Accessibility Test Cases

## Test Case: Validate Keyboard Navigation for All Form Fields
**ID:** TC_FB_ACC_001  
**Module:** Facebook – Registration Accessibility  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-06-19  
**Priority:** High  
**Type:** Accessibility / Functional  

### Preconditions:
- User is on the Facebook registration page
- No assistive software is interfering with tab behavior

### Test Steps:
1. Use `Tab` key to navigate through all form fields from top to bottom.
2. Verify logical and sequential tab order.
3. Verify `Shift + Tab` moves focus in reverse order.

### Expected Result:
- Each interactive field receives focus in a logical order.
- No fields are skipped.
- Focus is visible (highlighted/outlined).

---

## Test Case: Validate Screen Reader Labeling for Input Fields
**ID:** TC_FB_ACC_002  
**Module:** Facebook – Registration Accessibility  
**Priority:** High  
**Type:** Accessibility  

### Preconditions:
- User is on the registration page
- A screen reader (e.g., NVDA, VoiceOver) is enabled

### Test Steps:
1. Move to each input field using screen reader navigation keys.
2. Listen to the labels read aloud.

### Expected Result:
- Each input field has a clear, correctly associated label.
- The screen reader reads the field purpose and required status if applicable.

---

## Test Case: Validate Visible Focus Indicator
**ID:** TC_FB_ACC_003  
**Module:** Facebook – Registration Accessibility  
**Priority:** Medium  
**Type:** Accessibility / UI  

### Preconditions:
- User is on the registration page

### Test Steps:
1. Use `Tab` key to move through all interactive elements
2. Observe the screen during navigation

### Expected Result:
- Focus indicator (e.g., blue border, outline) is clearly visible on each element

---

## Test Case: Validate Error Message Announcement with Screen Reader
**ID:** TC_FB_ACC_004  
**Module:** Facebook – Registration Accessibility  
**Priority:** High  
**Type:** Accessibility  

### Preconditions:
- Screen reader is active
- User triggers a validation error (e.g., empty required field)

### Test Steps:
1. Attempt to submit the form with one or more required fields empty
2. Observe how the screen reader responds when error messages appear

### Expected Result:
- Screen reader announces error message clearly
- Focus moves to the first error field or error summary

---

## Test Case: Validate Color Contrast for Text and Input Fields
**ID:** TC_FB_ACC_005  
**Module:** Facebook – Registration Accessibility  
**Priority:** Medium  
**Type:** Accessibility / UI  

### Preconditions:
- User is on the registration page

### Test Steps:
1. Use browser tools (e.g., Chrome DevTools) or contrast analyzer
2. Check color contrast ratio of all text and input field borders

### Expected Result:
- Contrast ratio meets WCAG 2.1 AA standard (at least 4.5:1 for normal text)

---

## Test Case: Validate Registration via Only Keyboard (No Mouse)
**ID:** TC_FB_ACC_006  
**Module:** Facebook – Registration Accessibility  
**Priority:** High  
**Type:** Accessibility / Usability  

### Preconditions:
- Mouse is not used

### Test Steps:
1. Complete the entire registration flow using keyboard only (`Tab`, `Enter`, `Space`)
2. Attempt to submit the form

### Expected Result:
- All fields are reachable and usable
- Form is submitted successfully
