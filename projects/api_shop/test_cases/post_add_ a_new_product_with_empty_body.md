# Test Case: Add a New Product with empty body

**ID:** TC_API_009  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-013  
**Priority:** High  
**Type:** Functional  
**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products`  
- The user has Postman installed and a working internet connection

---

**Test Steps:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. In the **Body** tab, select **raw**, format **JSON**, and leave body empty
5. Click **Send**

---

**Expected Result:**  
- Status code: **400 Bad Request**  
- Response body contains an error message indicating missing or invalid input


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
- The API accepts an empty body and creates a product, assigning a new ID.
- This behavior violates standard REST validation expectations.
- API should reject requests with missing required fields.
- A bug report will be created to highlight this issue.  
