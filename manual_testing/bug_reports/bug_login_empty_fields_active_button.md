**ID**: BUG-002  
**Module**: Login  
**Reported by**: oZelloX  
**Date**: 2025-06-09  
**Environment**: Safari 18.5, macOS 15.5

## Description

The login button is active even when the required fields are empty.

## Steps to Reproduce

1. Go to the login page  
2. Leave the email field empty  
3. Leave the password field empty  
4. Observe the state of the "Login" button

## Expected Result

The "Login" button should be disabled until both fields are filled in.

## Actual Result

The "Login" button is active and clickable even when both fields are empty.

## Severity

Medium

## Priority

High

## Attachments

_None_
