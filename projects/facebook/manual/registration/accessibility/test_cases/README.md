# Accessibility Testing – Facebook Registration

This section contains accessibility test documentation for the Facebook registration page, aligned with WCAG 2.1 (AA level) standards.

## ✅ Included Files

- `accessibility_checklist.md` – High-level checklist for accessibility coverage
- `TC_FB_ACC_001` to `TC_FB_ACC_018` – Individual test cases covering keyboard navigation, screen reader behavior, visual structure, zoom/responsiveness, and ARIA usage

## 🔍 Scope

Focused on:
- Keyboard-only usage
- Screen reader support
- Visual clarity (focus, labels, contrast)
- Error message accessibility
- Responsiveness and zoom compatibility
- Compliance with WCAG 2.1 AA requirements

## 📅 Author & Date

- **Author:** Aleksandrs Goldobenkovs  
- **Started:** 2025-06-15  
- **Completed:** 2025-06-22

---

Ready for review or integration into larger QA documentation.



# ♿ What Was Tested – Accessibility

This section documents accessibility testing of the Facebook registration page. The goal was to assess compliance with WCAG 2.1 (AA level), ensuring that the form is usable by people relying on assistive technologies or alternative input methods.

## 🔍 Coverage Strategy

The following accessibility principles and techniques were applied:

- **Keyboard-Only Navigation**  
  Validated that all interactive elements can be accessed, focused, and used via keyboard alone (Tab, Shift+Tab, Arrow keys, Enter, Space).

- **Screen Reader Compatibility**  
  Verified correct labeling, focus announcement, and error message narration across form inputs.

- **Visual Design & Contrast**  
  Checked text/background contrast ratios, focus visibility, and layout clarity under zoom and small-screen conditions.

- **ARIA & Semantic Roles**  
  Evaluated the presence and correctness of ARIA roles (`form`, `button`, `textbox`, etc.) and landmarks (`main`, `header`, `nav`).

## 🧠 Notable Design Decisions

- All checks were mapped to WCAG 2.1 success criteria, with the AA compliance level as the baseline.  
- Wherever a bug or inconsistency was found (e.g. broken tab order, invisible focus), a separate test case was created and documented.
- Redundant low-impact checks (e.g. placeholder presence in multiple fields) were grouped into a single test to reduce noise.

## 🚧 Future Work

This suite focuses on **desktop browser accessibility** using tools like:

- Manual keyboard testing
- Screen readers (NVDA, VoiceOver)
- Zoom and resolution simulation
- Visual inspection of focus and labels

Future extensions may include:

- **Mobile Accessibility Testing**  
  Using TalkBack (Android) and VoiceOver (iOS) to validate mobile behavior

- **Automated Audits**  
  Integration of tools like axe DevTools or Lighthouse to speed up regression and standard compliance checks

- **Assistive Device Scenarios**  
  Testing voice input, switch control, or external keyboard navigation across platforms

These steps aim to ensure that Facebook’s registration page is accessible and inclusive for all users.





# Accessibility Testing – Facebook Registration

## Scope
Accessibility testing of the Facebook registration form, focused on compliance with WCAG 2.1 (AA level).

## Coverage Strategy
- Keyboard-only navigation and logical focus flow
- Screen reader compatibility for fields, labels, and error messages
- Color contrast, non-color indicators, and zoom responsiveness
- ARIA roles and semantic landmarks

## Design Notes
- Each test case targets a specific accessibility concern based on WCAG criteria
- Checklist was grouped to avoid duplication and simplify structure
- Tests are executable without specialized devices (where possible)
- 
