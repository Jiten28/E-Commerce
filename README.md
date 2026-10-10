# SportStore — Premium Sport Edition

A complete redesign of the original HTML/CSS/JavaScript e-commerce project. No packages, internet connection, build step or external fonts are needed.

<img width="1440" height="840" alt="image" src="https://github.com/user-attachments/assets/e0f2c41a-bad9-4720-942b-1e10fdbc19cb" />

## Live Link

URL : [SportStore — Premium Sport Edition](https://sport-store-pied.vercel.app/)

## Run locally

Use a local web server so all pages share the same browser storage:

```sh
cd E-Commerce
python3 -m http.server 8000
```

On Windows, use `py -m http.server 8000` if `python3` is unavailable. Open `http://localhost:8000` in your browser. You can also use VS Code Live Server. Opening individual files directly may prevent consistent storage across pages in some browsers.

## Pages

- `index.html`: homepage, curated products and category collections
- `products.html`: catalogue, search, category/size/price filters, sorting and saved-products view
- `product_details.html?id=1`: dynamic details for all 12 products; gallery on the first product
- `cart.html`: variant-aware bag, quantities, removal, automatic totals and demo checkout
- `account.html`: optional local demo profile, not authentication
- `about.html`: honest project overview
- `contact.html`: validated local demo contact form, not email delivery

## Features

- Consistent SportStore name and a new vector logo
- Responsive layouts, two-column mobile product cards, mobile navigation and filter drawers
- Keyboard-accessible dialogs, visible focus states, form labels, reduced-motion support and semantic HTML
- Search, combined filters, sorting and clearable filter chips; shareable catalogue URLs
- Persistent wishlist and cart; cart items are distinguished by product and size
- Product size selection, gallery switching, quantity limits (1–20 per product/size)
- Consistent INR pricing; sample delivery is ₹99 below ₹5,000 and ₹0 at or above ₹5,000; illustrative tax is included
- Demo checkout validation with a confirmation; no payment taken and no real order placed
- Browser-local profile with no password collection
- Privacy controls to clear SportStore local data
- Optimised local images and SVG icons; no third-party runtime requests

## Project structure

- `style.css`: design tokens and responsive styles
- `app.js`: sample product data and shared interactions
- `brand/`: SVG logo, light logo, compact mark, and palette notes
- `images/`: optimised photography from the original project

## Important production limitations

This is a working frontend demonstration, not a live store. Product prices, sizes and stock are sample data. Product materials, care instructions and manufacturer fit measurements have not been verified. No fabricated reviews, partner logos, discounts or payment badges are included.

A real launch needs server-side product/inventory data, secure authentication, server-side pricing and validation, a payment provider, order management, delivery/returns rules, contact-message delivery, and approved legal policies. Never use local storage as authentication. Do not collect real payment information in this demo.

Only the bag, saved product IDs and optional profile name/email are stored in local storage. Checkout and contact-form entries are not saved or sent. A production system must handle personal data securely.

## Assets and licensing

The redesign uses source photography supplied in the original project. Asset ownership and brand/trademark rights have not been verified; obtain appropriate rights before publishing commercially. Product branding was corrected where visibly identifiable, but catalogue names are otherwise descriptive. The new logo is a code-native SVG design; perform a trademark check before commercial use.

## Deployment

Upload the folder contents to a static host such as GitHub Pages or another static hosting service. Keep the directory structure intact. HTTPS is recommended. No runtime dependencies or secrets are needed for the demo.
