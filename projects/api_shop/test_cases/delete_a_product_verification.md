# Test Case: Update a Product

**ID:** TC_API_008  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-10  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products/{id}`  
- The user has Postman installed and a working internet connection  
- Product with ID = 7 doesn't exists
  
---

**Test Steps:**

1. Open Postman  
2. Set method to **GET**  
3. Enter URL: `https://fakestoreapi.com/products/7` 
4. Click **Send**

---

**Expected Result:**  
- Status code: **404 Not Found**  

---

**Actual Result:**  
- Status code: **200 OK**  
- Response body:
  
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
- The request deletes product with ID = 7.
- fakestoreapi returns a static response even for DELETE requests.

