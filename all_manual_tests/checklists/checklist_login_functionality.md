# Login Functionality Checklist

This checklist covers the basic test scenarios for verifying the Login functionality of the application.

## Preconditions
- User is on the Login page
- Application is accessible
- Test credentials are available

## Checklist

- [ ] Login page loads successfully
- [ ] Email/Username field is present
- [ ] Password field is present
- [ ] Login button is present
- [ ] Login button is disabled when fields are empty
- [ ] User can type into Email/Username field
- [ ] User can type into Password field
- [ ] Password is masked by default
- [ ] Option to show/hide password is available and works
- [ ] Error message is shown for invalid email format
- [ ] Error message is shown for wrong credentials
- [ ] User is redirected after successful login
- [ ] Session is created after login
- [ ] Forgot password link is present and navigates correctly
- [ ] Login form is cleared after unsuccessful attempt
