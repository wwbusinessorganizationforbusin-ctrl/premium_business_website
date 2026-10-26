# Little Luxe Toys — Premium Kids’ Toy Boutique

A responsive, luxury-inspired kids’ toy boutique website with a product catalogue made from the images supplied in `11.11.zip`, search, category filters, product details, an order list, and WhatsApp ordering.

## What's included
- `index.html`, `styles.css`, `app.js` — website source.
- `products.json` — editable catalogue records.
- `assets/products/` — 347 unique product images extracted and resized from the uploaded archive.
- WhatsApp number configured as +27 78 741 2314.

## Important catalogue note
The uploaded images did not include reliable product names, descriptions, categories, or prices that could be safely inferred. Products are therefore labelled Little Luxe Toy 001, Little Luxe Toy 002, etc. and their category is `Premium Kids' Toys`; prices are blank. These are placeholders, not verified toy names. Update `products.json` with accurate product details before publishing. Each record has `name`, `description`, `price`, `category`, `options`, `image`, and `original_file` fields. Keep the `image` path intact unless you also rename the corresponding file.

Example product record:
```json
{
  "id": 1,
  "name": "Accurate toy name",
  "description": "A verified product description.",
  "price": "R 199.00",
  "category": "Premium Kids' Toys",
  "image": "assets/products/product-001.jpg",
  "options": "Black, White",
  "original_file": "original-file-name.png"
}
```

## Run locally
Browsers may block `fetch()` from `products.json` when opening `index.html` directly as a `file://` URL. Run a local web server from this folder instead:

### Python
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`.

### VS Code
Open this folder and use the Live Server extension.

## Publish online
1. Edit the product catalogue and review the business content.
2. Upload the folder contents to a static host such as Netlify, Cloudflare Pages, or a web host that supports static files.
3. Connect your own domain in the hosting dashboard and follow its DNS/HTTPS setup steps.
4. Test product images, mobile layout, and the WhatsApp links after publishing.

## WhatsApp ordering
Orders open WhatsApp with a pre-filled message. The customer must press Send in WhatsApp. No online payment is taken by this website. Delivery, stock, and final prices must be confirmed with the business.

## Before going live
- Replace placeholder toy names with the accurate product names, descriptions, categories, prices, age guidance and variations in `products.json`.
- Confirm business hours, delivery/returns policy, terms and privacy notice. The legal notes on this starter page are brief placeholders, not legal advice.
- Add only social media profiles and contact details you control.
- A contact form, product admin dashboard, online payment, inventory sync, customer accounts, and secure backend are not included in this static starter; these need additional development or services.
- Google Fonts is loaded from an external service; system fonts are used as fallback.

## Accessibility and test notes
The site includes responsive layouts, labelled search/filter controls, keyboard Escape handling for overlays, image alt text, and status messages. Test on current Chrome and mobile devices before launch. A full browser-based visual QA run was not available in this build environment.

## Brand direction
The website is positioned as a premium kids’ toy boutique: polished, playful, gift-worthy, and warm. Product names and prices remain placeholders until confirmed against the actual items.
