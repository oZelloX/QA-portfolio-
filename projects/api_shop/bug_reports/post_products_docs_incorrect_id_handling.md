# Bug Report: POST /products – Documentation Incorrectly States That ID Should Be Supplied by Client

**ID:** BUG_API_004  
**Module:** API Shop – Products  
**Reported by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Severity:** Low  
**Priority:** Low  

**Environment:**  
- Endpoint: https://fakestoreapi.com/products  
- Method: POST  
- Tool: Postman  
- Internet: Stable  

---

**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products`  
- The user has Postman installed and a working internet connection  
- Request body is prepared according to official documentation, including `id` field

---

**Steps to Reproduce:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. In the **Body** tab, select **raw** and choose **JSON** format  
5. Paste the following request body (as shown in the official documentation):  
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
- The API should ignore the `id` field supplied in the request body  
- A new ID should be generated automatically  
- Status code: `201 Created`  
- Returned product object should contain a server-generated ID, not the client-provided one

---

**Actual Result:**  
- Status code: `200 OK`  
- Response body:
```json
{
  "id": 21,
  "title": "Test Product",
  "price": 9.99,
  "description": "Test description",
  "category": "test-category",
  "image": "http://example.com/test.jpg"
}
```

---

**Notes:**  
- The API behaves correctly by generating its own ID and ignoring the client-supplied one  
- However, the [official documentation](https://fakestoreapi.com/docs) shows that the client should provide the `id` field, which is misleading  
- This inconsistency may confuse users and should be corrected in the documentation
- A separate bug (see `BUG_API_002`) already covers the incorrect status code (`200 OK` instead of `201 Created`)
