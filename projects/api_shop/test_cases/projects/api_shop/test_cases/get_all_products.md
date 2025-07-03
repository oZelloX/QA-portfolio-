# Test Case: GET /products

- **ID:** TC_API_001  
- **Module:** Products  
- **Designed by:** Aleksandrs Goldobenkovs  
- **Date:** 2025-07-03  
- **Priority:** High  
- **Type:** Positive  
- **Preconditions:** API is available and reachable

---

## ✅ Test Steps:

1. Open Postman
2. Send a **GET** request to `/products` endpoint

---

## 🟢 Expected Result:

- Status code is **200 OK**
- Response body is a JSON array of product objects
- Each product includes:
  - `id` (integer)
  - `name` (string)
  - `price` (float)
  - `stock` (integer)

---

## 🔴 Actual Result:

_TBD (after Postman request)_

---

## 📝 Notes:

- Endpoint should return at least 1 product for verification
