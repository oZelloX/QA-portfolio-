# Delete User – API Test

**Method**: DELETE  
**Endpoint**: `https://reqres.in/api/users/2`  
**Description**: Verifies that a user can be deleted successfully.

## Request
No payload required.

## Expected Result
- Status code: **204 No Content**
- Response body is empty

## Actual Result
- Status code: **204 No Content**
- Response body: *(empty)*

## Notes
This confirms that the delete user endpoint responds correctly with no content when the operation is successful.
