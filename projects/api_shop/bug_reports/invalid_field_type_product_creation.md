# Bug Report: POST / API accepts empty request body when creating a new product

**ID:** BUG_API_005  
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
- Request body:
```json
{
  "title": "Wireless Mouse",
  "price": Very low price,
  "description": "Compact ergonomic design",
  "category": "20",
  "image": "http://example.com/mouse.jpg"
}

---

**Preconditions:** 
- The API is accessible at `https://fakestoreapi.com/products`
- The user has Postman installed and a working internet connection

---

**Steps to Reproduce:**

1. Open Postman  
2. Set method to **POST**  
3. Enter URL: `https://fakestoreapi.com/products`  
4.In the Body tab, select raw, format JSON
5. Paste the invalid request (non-numeric value in price)
6. Click **Send**

---

**Expected Result:**  
- Status code: **400 Bad Request**  
- Response should be in JSON format, with a clear error message (e.g., "price" must be a number)

---

**Actual Result:**  
- Status code: **200 OK**  
- Response is returned as an HTML error page:   

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




---

**Notes:**  
- API does not validate input types correctly or handle errors in a structured, client-friendly JSON format.
- HTML response is not suitable for API consumers and violates RESTful API best practices.
- Input validation for required types is critical for API reliability and client integration.
