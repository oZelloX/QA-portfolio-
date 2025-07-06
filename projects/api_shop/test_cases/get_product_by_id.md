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
*(To be filled after test execution)*

---

**Notes:**  
- No authorization required  
- Endpoint should return valid product details for a known ID
 
