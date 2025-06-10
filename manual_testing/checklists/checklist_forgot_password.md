# Forgot Password Functionality Checklist

This checklist covers test scenarios related to the "Forgot Password" process.

## Preconditions
- User is on the Login page
- "Forgot Password" link is visible
- Test email accounts are available

## Checklist

- [ ] "Forgot Password" link is visible on the Login page
- [ ] Clicking "Forgot Password" navigates to recovery page
- [ ] Email input field is present on the recovery page
- [ ] Email field validates input format
- [ ] Submit button is disabled when input is empty
- [ ] Submit button becomes active after valid email entry
- [ ] Error appears on invalid or unregistered email
- [ ] Confirmation message is shown after valid email submission
- [ ] Password reset email is sent (check inbox)
- [ ] Recovery link in the email redirects to reset page
- [ ] Reset page accepts and confirms new password
- [ ] User can log in with the new password after reset
