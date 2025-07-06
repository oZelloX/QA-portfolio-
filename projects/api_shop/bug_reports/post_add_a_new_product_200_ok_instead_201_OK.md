# Bug Report: POST /products – Returns 200 OK Instead of 201 Created

**ID:** BUG_API_002  
**Module:** API Shop – Products  
**Reported by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Severity:** Low  
**Priority:** Medium  

**Environment:**  
- Endpoint: https://fakestoreapi.com/products    
- Method: POST  
- Tool: Postman  
- Internet: Stable

---

**Preconditions:** 
- The API is accessible at https://fakestoreapi.com/products
- The user has Postman installed and a working internet connection
- Valid request body is prepared

---

**Steps to Reproduce:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. In **Body** tab, select **raw** and set format to **JSON**  
5. Paste the following request:  
```json
{
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
- Status code: 201 Created  
- Response body includes the created product with the same field order as in the request, plus assigned id  


---

**Actual Result:**  
- Status code: **200 OK**  
- Response body:
``` 
{
  "id": 21,
  "title": "Wireless Mouse",
  "price": 29.99,
  "description": "Compact ergonomic design",
  "image": "http://example.com/mouse.jpg",
  "category": "electronics"
}
```

---

**Notes:**  
- API returns 200 OK instead of the expected 201 Created, which breaks standard RESTful behavior.    
- Field order in the response is not preserved (e.g., description and image positions swapped), which may affect systems that rely on consistent field ordering, though this is technically allowed in JSON.
