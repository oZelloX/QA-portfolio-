# Bug Report: GET /products – Invalid ID returns 200 OK

**ID:** BUG_API_001  
**Module:** API Shop – Products  
**Reported by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Severity:** Medium  
**Priority:** Medium  

**Environment:**  
- Endpoint: `https://fakestoreapi.com/products/9999`  
- Method: GET  
- Tool: Postman  
- Internet: Stable

---

**Preconditions:** 
- The API is accessible at https://fakestoreapi.com/products
- The user has Postman installed and a working internet connection
- Product ID `9999` does not exist in the database

---

**Steps to Reproduce:**

1. Open Postman  
2. Set method to **GET**  
3. Enter URL: `https://fakestoreapi.com/products/9999`  
4. Click **Send**

---

**Expected Result:**  
- Status code: **404 Not Found**  
- Response body:  
```json
{
  "error": "Product not found"
}
```

---

**Actual Result:**  
- Status code: **200 OK**  
- Response body:  
```json
null
```

---

**Notes:**  
- API returns success (200 OK) for a non-existent product, which may confuse the client or tester.  
- Proper REST behavior would be to return an error status (e.g., 404) with a clear message.
