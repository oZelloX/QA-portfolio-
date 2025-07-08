# Test Case: Update a Product

**ID:** TC_API_006  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-07  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products/{id}`  
- The user has Postman installed and a working internet connection  
- Product with ID = 5 exists
  
---

**Test Steps:**

1. Open Postman  
2. Set method to **PUT**  
3. Enter URL: `https://fakestoreapi.com/products/5`
4. In **Body** tab, select **raw** and format **JSON**  
5. Paste the following request body:
```json
{
  "title": "string",
  "price": 0.1,
  "description": "string",
  "category": "string",
  "image": "http://example.com"
}
```
5. Click **Send**

---

**Expected Result:**  
- Status code: **200 OK**  
- Response is a JSON object containing the following fields:
 
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
    "id": 5,
    "title": "USB Flash drive",
    "price": 50.55,
    "description": "The best USB Flash Drive",
    "image": "http://example.com",
    "category": "Computer"
}
```
---

**Notes:**  
- Actual response includes undocumented field `rating` with nested `rate` (float) and `count` (integer)
 

