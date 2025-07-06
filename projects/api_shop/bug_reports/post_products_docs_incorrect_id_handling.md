# Bug Report: POST /products – Accepts Custom ID in Request Body

**ID:** BUG_API_003  
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
- Postman is installed and has internet access  
- Valid JSON body is prepared with a custom `id` field  

---

**Steps to Reproduce:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. In the **Body** tab, select **raw** and choose **JSON** format  
5. Paste the following request:  
```json
{
  "id": 99,
  "title": "Wireless Mouse",
  "price": 29.99,
  "description": "Compact ergonomic design",
  "category": "electronics",
  "image": "http://example.com/mouse.jpg"
}
```  
6. Click **Send**

---

**Expected Result:**  
- The API should ignore the custom `id` field from the request  
- It should generate a new ID automatically  
- Status code: `201 Created`

---

**Actual Result:**  
- Status code: `200 OK`  
- Response body:  
```json
{
  "id": 99,
  "title": "Wireless Mouse",
  "price": 29.99,
  "description": "Compact ergonomic design",
  "category": "electronics",
  "image": "http://example.com/mouse.jpg"
}
```

---

**Notes:**  
- The API accepts and returns the client-defined `id`, which can lead to ID conflicts and violates typical RESTful practices.  
- According to the [official documentation](https://fakestoreapi.com/docs), the `id` should not be supplied by the client.  
- This behavior may indicate a lack of input validation or missing constraints on the server.
