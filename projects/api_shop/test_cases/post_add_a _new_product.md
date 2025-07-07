# Test Case: Add a new product

**ID:** TC_API_004  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products`  
- The user has Postman installed and a working internet connection

---

**Test Steps:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. In the **Body** tab, select **raw**, format **JSON**, and input the following:
```json
{
  "title": "Wireless Mouse",
  "price": 29.99,
  "description": "Compact ergonomic design",
  "image": "http://example.com/mouse.jpg",
  "category": "electronics"
}
```
5. Click **Send**

---

**Expected Result:**  
- Status code: **201 Created**  
- Response contains newly created product with assigned ID:
```json
{
  "id": 0,
  "title": "string",
  "price": 0.1,
  "description": "string",
  "category": "string",
  "image": "http://example.com"
}
```

---

**Actual Result:**  
- Status code: **200 OK**  
- Response body:
```json
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
- Although the resource was successfully created, the API returned `200 OK` instead of the expected `201 Created`.  
- This may violate REST conventions and could be considered for a bug report.
