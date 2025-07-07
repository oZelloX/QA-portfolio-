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
- Product with ID = 10 exists
  
---

**Test Steps:**

1. Open Postman  
2. Set method to **PUT**  
3. Enter URL: `https://fakestoreapi.com/products/{id}` (replace `{id}` with a valid ID)
4. In **Body** tab, select **raw** and format **JSON**  
5. Paste the following request body:
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
    "id": 10,
    "title": "SanDisk SSD PLUS 1TB Internal SSD - SATA III 6 Gb/s",
    "price": 109,
    "description": "Easy upgrade for faster boot up, shutdown, application load and response (As compared to 5400 RPM SATA 2.5” hard drive; Based on published specifications and internal benchmarking tests using PCMark vantage scores) Boosts burst write performance, making it ideal for typical PC workloads The perfect balance of performance and reliability Read/write speeds of up to 535MB/s/450MB/s (Based on internal testing; Performance may vary depending upon drive capacity, host device, OS and application.)",
    "category": "electronics",
    "image": "https://fakestoreapi.com/img/61U7T1koQqL._AC_SX679_.jpg",
    "rating": {
        "rate": 2.9,
        "count": 470
    }
}
```
---

**Notes:**  
- Actual response includes undocumented field `rating` with nested `rate` (float) and `count` (integer)
 

