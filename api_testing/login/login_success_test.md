# Successful Login – API Test

**Method**: POST  
**Endpoint**: `https://reqres.in/api/login`  
**Description**: Verifies that a user can log in with valid credentials.

## Request Payload
```json
{
  "email": "eve.holt@reqres.in",
  "password": "cityslicka"
}
```

## Expected Result
- Status code: **200 OK**
- Response body contains a token:
```json
{
  "token": "QpwL5tke4Pnpja7X4"
}
```

## Actual Result
- Status code: **200 OK**
- Token received successfully.
```json
{
  "token": "QpwL5tke4Pnpja7X4"
}
```

## Notes
This confirms the login endpoint works correctly with valid credentials.

