# Accessibility Checklist – Facebook Registration

**Module**: Registration Page  
**Designed by**: Aleksandrs Goldobenkovs  
**Date**: 2025-06-21  
**Priority**: High  
**Scope**: Accessibility Testing (WCAG 2.1, AA level)

---

### 🧠 Keyboard Navigation
- [ ] All interactive elements (inputs, buttons, dropdowns) are reachable via Tab key
- [ ] Tab order follows a logical and expected sequence
- [ ] Focus is clearly visible and not lost during navigation
- [ ] User can complete registration using only the keyboard (no mouse)

### 🔈 Screen Reader Compatibility
- [ ] All form fields have associated `<label>` or `aria-label`
- [ ] Descriptive `aria-describedby` is used for helper/error texts
- [ ] Buttons and links have meaningful text (no "click here")
- [ ] Checkbox and radio groups are announced correctly

### 👁 Visual & Contrast
- [ ] Text and UI elements meet minimum contrast ratio (4.5:1 for normal text)
- [ ] Placeholder text is not used as the only label
- [ ] No color is used as the sole means of conveying information

### ⚠️ Error Handling
- [ ] Error messages are announced by screen readers
- [ ] Focus moves to the error or summary upon submission failure
- [ ] Error messages are specific and clearly associated with the field

### 📱 Responsive & Zoom
- [ ] Page remains functional and readable at 200% zoom
- [ ] Layout does not break on small screen widths (e.g., 320px)

### 🛠 ARIA & Landmarks
- [ ] Proper ARIA roles are used (`form`, `button`, `textbox`, etc.)
- [ ] Landmarks (`<main>`, `<nav>`, `<header>`, etc.) are correctly implemented

---

**Notes**:  
This checklist is meant for desktop web browser testing. Mobile-specific accessibility (VoiceOver, TalkBack) should be tested separately.



# Accessibility Checklist – Facebook Registration

**Module**: Registration Page  
**Designed by**: Aleksandrs Goldobenkovs  
**Date**: 2025-06-15  
**Priority**: High  
**Scope**: Accessibility Testing (WCAG 2.1, AA level)

---

- [ ] All interactive elements are keyboard-accessible with visible, logical focus  
- [ ] All fields and controls have accessible labels and descriptions  
- [ ] Errors are visible, specific, associated, and announced  
- [ ] No field uses placeholder as the only label  
- [ ] Contrast meets WCAG standards; color is not the only indicator  
- [ ] Page is readable at 200% zoom and usable at 320px width  
- [ ] Proper ARIA roles and landmarks are implemented
