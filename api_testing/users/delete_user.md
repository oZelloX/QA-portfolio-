# Delete User – API Test

**Method**: DELETE  
**Endpoint**: `https://reqres.in/api/users/2`  
**Description**: Verifies that the API handles user deletion requests correctly.  
Note: The user is not actually deleted on the server, as this is a mock API.

## Request
No request payload required.

## Expected Result  
- Status code: **204 No Content**  
- Response body: *(empty)*

## Actual Result  
- Status code: **204 No Content**  
- Response body: *(empty)*

## Notes  
This confirms that the delete endpoint correctly returns 204 status for a valid user ID, even though no action is performed.
