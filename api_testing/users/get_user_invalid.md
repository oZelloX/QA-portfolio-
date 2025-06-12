# Get User by ID – Invalid Case

**Method**: GET  
**Endpoint**: `https://reqres.in/api/users/23`  
**Description**: Verifies that the API returns a 404 status when the user ID does not exist.

## Request
No request payload required.

## Expected Result  
- Status code: **404 Not Found**  
- Response body is empty: `{}`

## Actual Result  
- Status code: **404 Not Found**  
- Response body:
```json
{}
```

## Notes

This confirms the API handles non-existent user IDs gracefully with proper 404 response.
