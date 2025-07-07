# Test Case: Get a single product Invalid {ID}

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
3. Enter URL: `https://fakestoreapi.com/products/{id}` (replace `{id}` with a invalid ID (doesn't exist)  
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

- API returns 200 OK with null for a non-existent product ID  
- This may be misleading and is a potential issue — should return a proper error status and message  
- Bug report will be created separately  
