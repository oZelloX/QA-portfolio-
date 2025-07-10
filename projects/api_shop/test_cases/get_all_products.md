# Test Case: Get All Products

**ID:** TC_API_001  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-03  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products`  
- The user has Postman installed and a working internet connection

---

**Test Steps:**

1. Open Postman  
2. Set method to **GET**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. Click **Send**

---

**Expected Result:**  
- Status code: **200 OK**  
- Response is a JSON array of product objects  
- Each object follows the documented structure. For example:

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
- Response includes multiple valid product objects with expected structure:

```json

{
  "id": 1,
  "title": "Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops",
  "price": 109.95,
  "description": "Your perfect pack for everyday use and walks in the forest. Stash your laptop (up to 15 inches) in the padded sleeve, your everyday",
  "category": "men's clothing",
  "image": "https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg",
  "rating": {
   "rate": 3.9,
   "count": 120
 }
}
  

```

---

**Notes:**  
- The response contains an array of product objects.
- The expected result provides a sample structure for one product as a reference.
- Each object is expected to follow the documented format.
- Rating field with nested fields rate (float) and count (integer), which is not documented in the official API specification.
- This test confirms that the structure is mostly consistent, but undocumented fields exist.
