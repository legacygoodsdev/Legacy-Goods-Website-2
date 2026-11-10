# Legacy Goods | Pakistani Clothing

This repository contains the **Legacy Goods** responsive online clothing storefront prototype. It is a Pakistani-inspired fashion label preview, intended for development and review before a commercial launch.

## Current features

- Responsive desktop and Android/mobile layout
- Women's unstitched lawn, women's ready to wear, men's kurtas, kidswear, and dupattas
- Eight **fictional** sample products with PKR prices, sizes, and conceptual SVG illustrations
- Product categories, product search, sorting, detailed product dialog
- Size-specific cart entries, quantity updates, and browser-local cart persistence
- Demonstration checkout and browser-local demonstration order summaries
- Self-contained `index.html` with CSS, JavaScript, and illustrative SVG markup

## Important

**This is a demonstration, not a functioning ecommerce shop.**

- Product names, materials, sizes, stock, discounts and prices are illustrative placeholders.
- No live payments or genuine purchases take place.
- Demo orders and shopping bag are stored in this browser's localStorage only, not sent to an admin dashboard.
- The checkout form does not transmit or save customer contact or address details.
- There is no customer sign-up, production inventory, admin dashboard, or Supabase connection yet.
- Replace sample product illustrations with properly licensed images of actual stock before launch.

## Development

Open `index.html` locally in your browser, or run:

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080.

## Deploy frontend to Netlify

1. Open https://app.netlify.com/
2. Choose **Add new project → Import an existing project**.
3. Connect GitHub, then select `legacygoodsdev/Legacy-Goods-Website-2`.
4. Branch: `main`, build command: **none**, publish directory: `.`.
5. Deploy. Changes pushed to `main` can trigger subsequent frontend deployments.

For commercial ecommerce, use hosting that permits commercial websites. GitHub is the source-code repository, not the production shopping backend.

## Production roadmap

1. Approve real brand identity, garments, fabric descriptions, photos, size charts, prices and stock.
2. Add a secure backend such as Supabase for authenticated customers, products and orders.
3. Use Row Level Security for customer data, enforce roles server-side, and protect admin/super-admin areas.
4. Create server-validated checkout, shipping fee and stock calculations, and COD or a verified payment provider.
5. Add return/exchange, privacy, shipping, contact and store policies.
6. Perform accessibility, mobile browser, order lifecycle and security tests before launch.

Do not add Supabase `service_role` keys or other secrets to frontend code.
