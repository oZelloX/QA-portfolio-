# Get Users – API Test

**Method**: GET  
**Endpoint**: `https://reqres.in/api/users?page=2`  
**Description**: Verifies that the API returns a paginated list of users with the correct structure.  
**Expected Result**:  
- Status code: **200 OK**  
- Response body contains page information and a list of 6 user objects with fields: id, email, first_name, last_name, avatar  
**Actual Result**:  
- Status code: **200 OK**  
- The response included 6 users with correct fields and pagination metadata  
**Notes**: This confirms that the user listing endpoint returns valid paginated user data with the expected structure.

