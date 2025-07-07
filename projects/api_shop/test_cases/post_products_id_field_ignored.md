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

- Status code: 201 Created
- Response body includes the same id value as sent (i.e., "id": 123)
- All other fields match the request

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

- The API ignores the id value sent in the request and generates its own
- This contradicts the official documentation, which suggests the id can be provided manually
- Bug report will be created separately regarding the inconsistency
