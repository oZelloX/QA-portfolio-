# Test Case: Get a Single Product - Invalid {ID}

**ID:** TC_API_003  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-06  
**Priority:** Medium  
**Type:** Negative / Functional  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products/{id}`  
- The user has Postman installed and a working internet connection

---

**Test Steps:**

1. Open Postman  
2. Set method to **GET**  
3. Enter URL: `https://fakestoreapi.com/products/{id}` (replace `{id}` with an invalid ID that doesn't exist, e.g., `9999`)    
4. Click **Send**

---

**Expected Result:**  
- Status code: **404 Not Found** or other error status  
- Response should contain a clear error message (e.g., `"Product not found"`)

---

**Actual Result:**  
- Status code: **200 OK**  
- Response body:  
```json
null
```

**Notes:**  
- The API returns status code 200 OK and body `null` when a non-existent product ID is requested.  
- This behavior may be misleading and does not follow standard REST practices.  
- A proper error status (e.g., 404 Not Found) and message should be returned instead.  
- A bug report will be created separately.
