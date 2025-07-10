# Test Case: Verify Product is Deleted

**ID:** TC_API_008  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-10  
**Priority:** High  
**Type:** Functional / Negative / Follow-up  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products/{id}`  
- The user has Postman installed and a working internet connection  
- Product with ID = 7 was previously deleted using the DELETE request

---

**Test Steps:**

1. Open Postman  
2. Set method to **GET**  
3. Enter URL: `https://fakestoreapi.com/products/7`  
4. Click **Send**

---

**Expected Result:**  
- Status code: **404 Not Found**  
- Or response body is `null`

---

**Actual Result:**  
- Status code: **200 OK**  
- Response body:
```json
{
  "id": 7,
  "title": "White Gold Plated Princess",
  "price": 9.99,
  "description": "Classic Created Wedding Engagement Solitaire Diamond Promise Ring for Her. Gifts to spoil your love more for Engagement, Wedding, Anniversary, Valentine's Day...",
  "category": "jewelery",
  "image": "https://fakestoreapi.com/img/71YAIFU48IL._AC_UL640_QL65_ML3_.jpg",
  "rating": {
    "rate": 3,
    "count": 400
  }
}
```
---

**Notes:**
- This test verifies whether the product was actually deleted after a DELETE request.
- fakestoreapi returns a static product object with status 200 OK, meaning the product still exists.
- This confirms that the DELETE operation is non-functional in fakestoreapi.
- The test is retained to document full coverage and highlight API limitations.
