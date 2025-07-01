## 🧷 Data Model Overview

The API includes the following entities:

- **Products** — items available for purchase (e.g. mouse, keyboard)
- **Cart Items** — user-selected products in a virtual shopping cart
- **Orders** — submitted purchases with total amounts

### 🛒 Cart Model: Item-Based

This system uses an **item-based cart model**. Each product added to the cart creates a separate entry (`item_id`), even if it's the same product.

This allows:

- Tracking each cart item individually
- Supporting product variations (like color, packaging) without separate `product_id`s
- Removing specific cart entries by `item_id`

In some systems, different product variants have separate `product_id`s. In our case, variations are handled via request data, so `item_id` is necessary.

---

## Endpoints

[дальше идут `GET /products`, `POST /cart` и т.д., как раньше]
