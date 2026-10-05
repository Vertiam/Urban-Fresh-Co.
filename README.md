# Urban Fresh Co. 🌱

**Fresh & local microgreens delivery.** A demo storefront built from the Urban Fresh Co. business model canvas. It runs as a single static HTML file, so it deploys straight to GitHub Pages with no build step and no backend.

> **Demo only.** Orders, subscriptions and the UPI payment screen are simulated. No real payments are taken and nothing leaves the browser.

## Features

- **Shop:** 13 microgreen varieties, a branded grow kit and gift certificates, with prices in ₹. Each product has a generated illustration, or your own photo (see below).
- **Subscriptions:** choose one-time or weekly delivery (10% off). Pause, resume or cancel from the account panel.
- **Cart and checkout:** home delivery by e-trike or pick-up at a local hub or co-op.
- **Demo UPI payment:** pay with a UPI ID or a sample QR code, then enter any 4 to 6 digit PIN. Use `0000` to see a failed payment.
- **Restaurant standing orders:** chefs save a weekly tray order and pick a delivery route.
- **Farm-to-table traceability:** enter a batch code (for example `UF-2610-4821`) to see the seed lot, farm rack and harvest details.
- **Eco-impact score:** every order adds to a personal score based on food-km avoided and plastic clamshells saved.
- **Saved in the browser:** the cart, orders, subscriptions and standing orders are stored in `localStorage`. The account panel has a "Clear saved data" button.

## Business canvas mapping

| Canvas block | In the app |
|---|---|
| Value propositions | Organic microgreens, home delivery, batch traceability |
| Channels | Website, weekly subscriptions, restaurant routes, local delivery hubs |
| Customer relationships | Chef standing orders, account panel, eco-impact score |
| Customer segments | Households and restaurant chefs |
| Revenue streams | Subscriptions, restaurant bulk orders, gift certificates, grow kits |


To run it locally, open `index.html` in a browser.

## Customise

All settings are in the `<script>` at the bottom of `index.html`:

- `PRODUCTS`: names, prices (`p:`), descriptions, colours and tags.
- `HUBS`: delivery and pick-up locations.
- `DISC`: the subscription discount (`0.10` is 10%).

**Real product photos:** create an `images/` folder and add files named after each product id, such as `images/pea.jpg` or `images/mus.jpg`. A photo replaces the illustration, and products without one keep it.

## Tech

Plain HTML, CSS and JavaScript in one file. Fonts (Bricolage Grotesque and Figtree) load from Google Fonts. There are no other dependencies.

## Limitations

- Data lives in one browser only. Clearing site data removes it.
- Payments, delivery tracking and traceability records are demo data.
- For real orders you would need a backend and a payment gateway.

---

*Urban Fresh Co.: a sustainable growth model.*
