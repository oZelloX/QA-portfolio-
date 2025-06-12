# Get User by ID – API Test with Postman Script

**Method**: GET  
**Endpoint**: `https://reqres.in/api/users/2`  
**Description**: Verifies that a specific user can be retrieved successfully and that the response contains all expected fields.

## Request
No payload required.

## Expected Result
- Status code: **200 OK**
- Response body contains a `data` object with the following fields:
  - `id`
  - `email`
  - `first_name`
  - `last_name`
  - `avatar`

## Test Script (Postman)
```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response contains user data", function () {
    var jsonData = pm.response.json();
    pm.expect(jsonData.data).to.have.property("id");
    pm.expect(jsonData.data).to.have.property("email");
    pm.expect(jsonData.data).to.have.property("first_name");
    pm.expect(jsonData.data).to.have.property("last_name");
    pm.expect(jsonData.data).to.have.property("avatar");
});
```

## Notes

This test verifies that the API returns a valid response for a specific user and includes all expected fields. The assertions are automated and run in the Postman test tab after sending the request.
