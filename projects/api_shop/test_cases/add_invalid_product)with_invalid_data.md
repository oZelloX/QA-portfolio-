# Test Case: Create Product – Invalid Field Types

**ID:** TC_API_010  
**Module:** API Shop – Products  
**Designed by:** Aleksandrs Goldobenkovs  
**Date:** 2025-07-13  
**Priority:** High  
**Type:** Negative / Functional  

**Preconditions:**  
- The API is accessible at `https://fakestoreapi.com/products`  
- The user has Postman installed and a working internet connection  

---

**Test Steps:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4. In the **Body** tab, select **raw**, format **JSON**, and paste:
```json
{
  "title": "Wireless Mouse",
  "price": Very low price,
  "description": "Compact ergonomic design",
  "category": "20",
  "image": "http://example.com/mouse.jpg"
}
```
5. Click **Send**

---

**Expected Result:**  
- Status code: **400 Bad Request**  
- Response body should contain an error message indicating that the `price` field has an invalid type (string instead of number)

---

**Actual Result:**  
- Status code: **400 Bad Request**  
- Response body:
```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>Error</title>
</head>
<body>
<pre>Bad Request</pre>
</body>
</html>
```

---

**Notes:**  
- The API fails with a generic HTML error page instead of a structured JSON response.
- The error handling lacks clarity and does not specify which field caused the problem.
- Proper validation and structured error response should be implemented to aid developers and testers.
