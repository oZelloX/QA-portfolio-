# Test Case: Get a Single Product

**ID:** TC_API_002  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Priority:** High  
**Type:** Functional  
**Preconditions:**
- Product with ID = 10 exists
- The API is accessible at `https://fakestoreapi.com/products/10`  
- The user has Postman installed and a working internet connection  

  
---

**Test Steps:**

1. Open Postman  
2. Set method to **GET**  
3. Enter URL: `https://fakestoreapi.com/products/10`
4. Click **Send**

---

**Expected Result:**  
- Status code: **200 OK**  
- Response is a JSON object.  
- The following is an example of the expected structure, based on API documentation:
 
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
- The expected result reflects the documented structure of a product object.  
- The actual response includes an additional field `rating`, with nested `rate` (float) and `count` (integer), which is not described in the official documentation. 
