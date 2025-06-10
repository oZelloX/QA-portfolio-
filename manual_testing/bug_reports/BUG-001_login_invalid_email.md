**ID**: BUG-001  
**Module**: Login  
**Reported by**: oZelloX  
**Date**: 2025-06-09  
**Environment**: Safari 17, macOS 15.5

## Description

Submitting an invalid email does not trigger an error message.

## Steps to Reproduce

1. Go to the login page  
2. Enter an invalid email (e.g., `user@com`)  
3. Enter a valid password  
4. Click **Login**

## Expected Result

An error message appears: `Invalid email format`.

## Actual Result

The form is cleared without any error message shown.

## Severity

Medium

## Priority

High

## Attachments

_None_
