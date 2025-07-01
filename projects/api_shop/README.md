## 🧷 Cart Model: Item-Based

This project uses an **item-based cart model**, meaning each item added to the cart is stored as a separate entry with a unique `item_id`.

This allows us to:
- Track multiple entries of the same product separately
- Handle product variations (e.g. color, packaging) within the same `product_id`
- Remove specific cart items using their `item_id`

> Note: In some systems, different product variations (like color) may have their own `product_id`. In our case, variations can be represented as part of the request body, so `item_id` is required to distinguish them.

