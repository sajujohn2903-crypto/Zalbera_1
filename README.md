# Zalbera — website

Landing page and product pages for Zalbera, a house of eau de parfum (8 fragrances).

## Pages
- `index.html` — landing page: hero, "A scent that tells a story" with the gold line-drawn bottle and notes, the collection with filters, and footer.
- `product.html` — one page for every fragrance, chosen by the link's hash, e.g. `product.html#alfaro`.
  Ids: `alfaro`, `prestige-king`, `oud-rosara`, `tesoro-leather`, `hudsaro`, `rubelle`, `zenvora`, `rose-mystique`.

Each product page has an image gallery (zoom on desktop, swipe on phones), size and quantity, Add to cart and Buy now, a slide-out cart, the top / heart / base notes, a story section, reviews and "You may also like".

## Run it
It's a static site with no build step. Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000. It can be hosted as-is on GitHub Pages, Netlify or similar.

## Before launch
- **Prices are placeholders** (AED 250 for 50 ml, AED 395 for 100 ml). Edit `SIZES` near the top of the script in `product.html`.
- **Checkout is not connected to payments.** The cart is kept in the visitor's browser (localStorage); connect it to the store (e.g. Shopify) to take orders.
- **Reviews** start empty and are saved only in the visitor's browser until a review service is connected.
- **Email sign-up** forms are not connected to a mailing list yet.
- The **WELCOME10** promo bar text is placeholder copy.

## Assets
- `img/` — landing page images; `img/p/` — product gallery images.
- `assets/` — Zalbera logo mark and wordmark (SVG). The logo is also inlined in both pages.
- Fonts: Italiana and Archivo from Google Fonts.
