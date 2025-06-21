# Partial Update User – API Test

**Method**: PATCH  
**Endpoint**: `https://reqres.in/api/users/2`  
**Description**: Verifies that a user's data can be partially updated using the PATCH method.

## Request Payload
```json
{
  "job": "senior developer"
}
```

## Expected Result
- Status code: **200 OK**
- Response body contains:
  - `job`: "senior developer"
  - `updatedAt`: current timestamp

## Actual Result
- Status code: **200 OK**
- Response body:
```json
{
  "job": "senior developer",
  "updatedAt": "2025-06-12T18:04:52.993Z"
}
```

## Notes
This confirms the PATCH method updates specific user fields without altering others.
