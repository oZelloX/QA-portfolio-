# Bug Report: POST / API accepts empty request body when creating a new product

**ID:** BUG_API_004  
**Module:** API Shop – Products  
**Reported by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-13  
**Severity:** High  
**Priority:** High  

**Environment:**  
- Endpoint: `https://fakestoreapi.com/products`  
- Method: POST  
- Tool: Postman  
- Internet: Stable
- Body: empty JSON body ({} or completely empty)

---

**Preconditions:** 
- The API is accessible at `https://fakestoreapi.com/products`
- The user has Postman installed and a working internet connection

---

**Steps to Reproduce:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. Click **Send**

---

**Expected Result:**  
- Status code: **400 Bad Request**  
- Response should contain an error message indicating missing or invalid input (e.g., "title" is required)

---

**Actual Result:**  
- Status code: **200 OK**  
- Response body:  
```json
{
  "id": 21
}

```

---

**Notes:**  
- The API incorrectly accepts an empty body and proceeds to create a product with only an auto-generated ID.
- This violates standard RESTful API validation practices.
- Required fields (title, price, etc.) must be validated before creation.
