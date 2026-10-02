# Stride

A small sneaker store front end built with plain HTML, JavaScript and Tailwind CSS (via CDN). No build step and no backend.

## Features
- Home, Shop, Product, Wishlist, Cart and Checkout pages (hash routing, e.g. `#/shop`, `#/product/3`)
- Shop filters by category and sorting by price
- Product pages with description, rating, details table and **Buy Now**
- Cart with quantity controls and a free-shipping progress bar
- Wishlist, cart and newsletter state saved in `localStorage`
- Responsive layout with a mobile menu

> Demo only: checkout takes no payment, and the ratings and specs are placeholder text.

## Run locally
Open `index.html` in a browser.

## Deploy with GitHub Pages
1. Push this folder to a GitHub repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then `main` and `/ (root)`.
4. Your site appears at `https://<username>.github.io/<repo>/` after a minute or two.

## Structure
```
index.html   page shell, Tailwind config, header and footer
app.js       products, cart, wishlist, routing and views
images/      put your own product photos here (optional)
```

## Edit products
Products are the `P` array at the top of `app.js`; descriptions, ratings and specs are in `INFO`.
To use your own photo, save it in `images/` and change the product's `file:` value to, for example, `"images/cloudrunner.jpg"`. If an image fails to load, a drawn sneaker is shown instead.
