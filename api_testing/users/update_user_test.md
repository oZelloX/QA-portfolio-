# Update User – API Test

**Method**: PUT  
**Endpoint**: `https://reqres.in/api/users/2`  
**Description**: Verifies that user data can be successfully updated via PUT request.

## Request Payload
```json
{
  "name": "morpheus",
  "job": "zion resident"
}
```

## Expected Result
- Status code: **200 OK**
- Response body contains:
  - `name`: "morpheus"
  - `job`: "zion resident"
  - `updatedAt`: current timestamp

## Actual Result
- Status code: **200 OK**
- Response body:
```json
{
  "name": "morpheus",
  "job": "zion resident",
  "updatedAt": "2025-06-12T17:56:22.087Z"
}
```

## Notes
This confirms the user update endpoint processes data correctly and returns a valid timestamp.
