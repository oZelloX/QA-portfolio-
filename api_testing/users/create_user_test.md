On 2025-06-11, I tested the POST /users endpoint at https://reqres.in/api/users. The goal was to check whether a user can be created successfully when valid data is sent. I used the following request:

POST https://reqres.in/api/users  
Content-Type: application/json  

The request body looked like this:

{
  "name": "morpheus",
  "job": "leader"
}

The expected result was a 201 Created status and a response body containing the same name and job, along with a generated id and createdAt timestamp. The actual response was:

{
  "name": "morpheus",
  "job": "leader",
  "id": "938",
  "createdAt": "2025-06-11T09:15:00.000Z"
}

I sent this request using Postman. The status was 201, and the fields matched the expected format. This confirms that the endpoint behaves correctly when provided with valid input. Here's the short test case that I followed:

Test Case: Create user with valid data  
Step 1: Send POST request to /users with name and job  
Expected result: Status 201, and response contains name, job, id, and createdAt  
Status: Passed

Since this is a mock API, no data is saved, and each request returns a new id and timestamp. Everything worked as expected.

