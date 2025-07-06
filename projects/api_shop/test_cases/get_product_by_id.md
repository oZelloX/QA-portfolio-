# Test Case: GET /products/{id}

**ID:** TC_API_002  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products/1`  
- The product with ID 1 exists  
- The user has Postman installed and a working internet connection

---

**Test Steps:**

1. Open Postman  
2. Set method to **GET**  
3. Enter URL: `https://fakestoreapi.com/products/1`  
4. Click **Send**

---

**Expected Result:**  
- Status code is **200 OK**  
- Response is a JSON object  
- Object contains the following fields:
  - `id` (integer)
  - `name` (string)
  - `price` (float)
  - `stock` (integer)

---

**Actual Result:**  
```
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
- No authorization required  
- Endpoint should return valid product details for a known ID
 
