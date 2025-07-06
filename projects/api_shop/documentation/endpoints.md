# API Shop — Endpoints Documentation

This document describes the available API endpoints for the API Shop project.

---

## 🔷 Products

### GET /products

Returns a list of all products.

**Example response:**

```json
[
  {
    "id": 0,
    "title": "string",
    "price": 0.1,
    "description": "string",
    "category": "string",
    "image": "http://example.com"
  }
]
```

---

### GET /products/{id}

Returns details of a single product by ID.

**Example response:**

```json
{
  "id": 0,
  "title": "string",
  "price": 0.1,
  "description": "string",
  "category": "string",
  "image": "http://example.com"
}
```

---

## 🔷 Cart

### POST /cart

Adds a product to the user's cart.

**Request body:**

```json
{
  "product_id": 1,
  "quantity": 2
}
```

**Example response:**

```json
{
  "item_id": 1,
  "product_id": 1,
  "quantity": 2
}
```

---

### GET /cart

Returns the current contents of the user's cart.

**Example response:**

```json
[
  {
    "item_id": 1,
    "product_id": 1,
    "quantity": 2
  }
]
```

---

### DELETE /cart/{item_id}

Removes a product from the cart by item ID.

---

## 🔷 Orders

### POST /orders

Places a new order using items in the cart.

**Request body:**

```json
{
  "items": [
    { "product_id": 1, "quantity": 2 },
    { "product_id": 2, "quantity": 1 }
  ]
}
```

**Example response:**

```json
{
  "order_id": 1001,
  "items": [
    { "product_id": 1, "quantity": 2 },
    { "product_id": 2, "quantity": 1 }
  ],
  "total": 109.97
}
```

---

### GET /orders/{order_id}

Returns the details of a specific order.

**Example response:**

```json
{
  "order_id": 1001,
  "items": [
    { "product_id": 1, "quantity": 2 }
  ],
  "total": 59.98
}
```

---

## 🔷 Authentication

### POST /login

Authenticates a user and returns an access token.

**Request body:**

```json
{
  "email": "user@example.com",
  "password": "123456"
}
```

**Example response:**

```json
{
  "token": "abc123xyz456"
}
```

---

### GET /profile

Returns user profile information. Requires token in Authorization header.

**Example response:**

```json
{
  "user_id": 10,
  "name": "John Doe",
  "email": "user@example.com"
}
```
