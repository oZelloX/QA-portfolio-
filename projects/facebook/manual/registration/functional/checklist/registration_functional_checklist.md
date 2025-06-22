# Functionality Checklist – Facebook Registration

**Module**: Registration Page  
**Designed by**: Aleksandrs Goldobenkovs  
**Date**: 2025-06-15  
**Priority**: High  
**Scope**: Functional Testing

##  Positive Test Scenarios
- [] Validate sign up using a phone number  
- [] Validate sign up using an email address  
- [] Validate input of Cyrillic first and last names  
- [] Validate input of very short names or surnames  
- [] Validate different phone number formats (with and without country code)  
- [] Validate teen account sign up (age 13–17, including boundary 17)  
- [] Validate adult account sign up (age 18–120, including boundary 18)  
- [] Validate selection of different gender options  

##  Negative Test Scenarios
- [] Validate sign up with empty required fields  
- [] Validate name fields with invalid characters  
- [] Validate name fields with invalid length (too few / too many character
- [] Validate phone number field with invalid formats (length, spacing, pasted input)  
- [] Validate Email with invalid format  
- [] Validate Email with incorrect domain  
- [] Validate sign up with already registered email  
- [] Validate password field against security rules (length, letters, numbers, special characters)  
- [x] Validate age-related registration rules (minors, adults, boundary values)  

##  Navigation & UI
- [] Validate “Already have an account?” link functionality  
- [] Validate “Create New Account” link functionality from Login page  
