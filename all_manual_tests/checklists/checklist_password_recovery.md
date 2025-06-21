# Password Recovery Checklist

This checklist verifies the password recovery process.

## Preconditions
- User is on the "Forgot Password" page

## Checklist

- [ ] "Forgot Password" link is visible on Login page
- [ ] User can open password recovery form
- [ ] Input accepts valid email format
- [ ] Input shows validation error for invalid email
- [ ] Submit button is disabled for empty or invalid input
- [ ] User receives confirmation message after submission
- [ ] Email is sent to the user (check message or simulate)
- [ ] Reset link in email redirects to the reset form
- [ ] Reset link expires after set time
- [ ] New password form validates inputs (length, complexity)
- [ ] User can successfully log in with the new password
- [ ] Old password no longer works after reset
