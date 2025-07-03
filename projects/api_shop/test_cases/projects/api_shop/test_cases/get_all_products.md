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
- Each product must include:
  - `id` (integer)  
  - `title` (string)  
  - `price` (float)  
  - `description` (string)  
  - `category` (string)  
  - `image` (string - URL)  
  - `rating` (object) containing:
    - `rate` (float)  
    - `count` (integer)


---

## 🔴 Actual Result:

- Status code is **200 OK**

```   
    {
        "id": 1,
        "title": "Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops",
        "price": 109.95,
        "description": "Your perfect pack for everyday use and walks in the forest. Stash your laptop (up to 15 inches) in the padded sleeve, your everyday",
        "category": "men's clothing",
        "image": "https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg",
        "rating": {
            "rate": 3.9,
            "count": 120
        }
    }
```
---

## 📝 Notes:

- Endpoint should return at least 1 product for verification
