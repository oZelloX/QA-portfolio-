# Login Unsuccessful – API Test

**Method**: POST  
**Endpoint**: `https://reqres.in/api/login`  
**Description**: Verifies that the login endpoint returns an appropriate error when password is missing.

## Request Payload
```json
{
  "email": "peter@klaven"
}
```

## Expected Result  
- Status code: **400 Bad Request**  
- Response body contains:
```json
{
  "error": "Missing password"
}
```

##Actual Result  
- Status code: **400 Bad Request**  
- Response body:
```json 
{
  "error": "Missing password"
}
```

##Notes
The API correctly returns an error message in JSON format when the password field is missing.

