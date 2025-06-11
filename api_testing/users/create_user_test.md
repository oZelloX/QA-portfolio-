# Create User – API Test

**Method**: POST  
**Endpoint**: `https://reqres.in/api/users`  
**Description**: Verifies that a user can be created successfully with valid input data.  

## Request Payload
```json
{
  "name": "morpheus",
  "job": "leader"
}
```

## Expected Result  
- Status code: **201 Created**  
- Response body contains:  
  - name: "morpheus"  
  - job: "leader"  
  - id: string (auto-generated)  
  - createdAt: string (timestamp)

 
## Actual Result  
- Status code: **201 Created**  
- ID and createdAt fields were generated and returned as expected.  
## Notes
This confirms the create user endpoint responds correctly with dynamically generated data.
