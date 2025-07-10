 # Test Case: Add a New Product – ID Provided in Request (Based on Documentation)

**ID:** TC_API_005  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Priority:** Medium  
**Type:** Functional / Documentation Validation  

**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products`  
- The user has Postman installed and a working internet connection  
- Documentation indicates `id` can be included in request body  

---

**Test Steps:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. In **Body** tab, select **raw** and format **JSON**  
5. Paste the following request body:  
```json
{
  "id": 123,
  "title": "Test Product",
  "price": 9.99,
  "description": "Test description",
  "category": "test-category",
  "image": "http://example.com/test.jpg"
}
```
6. Click **Send** 

---

**Expected Result:**  

- Status code: 201 OK
{
  "id": 123,
  "title": "Test Product",
  "price": 9.99,
  "description": "Test description",
  "category": "test-category",
  "image": "http://example.com/test.jpg"
}

---  

**Actual Result:**  

- Status code: 200 OK
- Response body:
```json  
{
  "id": 22,  
  "title": "Test Product",
  "price": 9.99,
  "description": "Test description",
  "category": "test-category",
  "image": "http://example.com/test.jpg"
}
```

---
 
**Notes:**  
- The API ignores the `id` value provided in the request body and assigns its own, which is standard behavior for RESTful APIs.  
- However, this contradicts the API documentation, which implies that the `id` field can be manually specified.  
- The API also returns status code `200 OK` instead of the expected `201 Created`, which is a deviation from REST conventions.  
- Expected result based on documentation was not met; however, the actual behavior is correct by design.  
- A bug report will be created to address the misleading documentation and non-standard response code.

