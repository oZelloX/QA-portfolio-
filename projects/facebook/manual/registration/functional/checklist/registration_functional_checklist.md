# Functionality Checklist – Facebook Registration

**Module**: Registration Page  
**Designed by**: Aleksandrs Goldobenkovs  
**Date**: 2025-06-15  
**Priority**: High  
**Scope**: Functional Testing

## ✅ Positive Test Scenarios
- [x] Validate sign up using a phone number  
- [x] Validate sign up using an email address  
- [x] Validate input of Cyrillic first and last names  
- [x] Validate input of very short names or surnames  
- [x] Validate different phone number formats (with and without country code)  
- [x] Validate teen account sign up (age 13–17, including boundary 17)  
- [x] Validate adult account sign up (age 18–120, including boundary 18)  
- [x] Validate selection of different gender options  

## ❌ Negative Test Scenarios
- [x] Validate sign up with empty required fields  
- [x] Validate name fields with invalid characters  
- [x] Validate name fields with invalid length (too few / too many character
- [x] Validate phone number field with invalid formats (length, spacing, pasted input)  
- [x] Validate Email with invalid format  
- [x] Validate Email with incorrect domain  
- [x] Validate sign up with already registered email  
- [x] Validate password field against security rules (length, letters, numbers, special characters)  
- [x] Validate age-related registration rules (minors, adults, boundary values)  

## 🔁 Navigation & UI
- [x] Validate “Already have an account?” link functionality  
- [x] Validate “Create New Account” link functionality from Login page  
