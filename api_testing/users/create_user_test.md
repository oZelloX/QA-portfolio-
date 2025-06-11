On 2025-06-11, I tested the POST /users endpoint at https://reqres.in/api/users to verify that a user can be created successfully when valid input is provided. The method used was POST and the request body was:

{
  "name": "morpheus",
  "job": "leader"
}

The expected result was a 201 Created status code and a response body containing the same name and job along with a generated id and createdAt timestamp. The actual response returned status 201 Created, and the following body:

{
  "name": "morpheus",
  "job": "leader",
  "id": "938",
  "createdAt": "2025-06-11T09:15:00.000Z"
}

The ID and timestamp were generated dynamically as expected. This confirms that the endpoint behaves correctly when provided with valid data.

