# MyNestora — Storefront & Theme

A fast, lightweight e-commerce storefront for **MyNestora** with direct Shop Pay checkout integration.

---

## 🚀 Live Static Storefront (Root)

The root of this branch contains the standalone static storefront ready for deployment (GitHub Pages, Vercel, Netlify, or local preview):

- **[`index.html`](index.html)** — Homepage featuring the hero banner, brand styling, announcement bar, and product showcase.
- **[`product.html`](product.html)** — Product detail page for the **MyNestora Turbo Vac** featuring interactive photo gallery, live pricing, badges, and trust assurances.
- **[`images/`](images/)** — Brand assets and product photography organized by category.

### Direct Shopee Affiliate Buy Link
All purchase buttons ("Shop on Shopee", "Buy on Shopee", "Check Out on Shopee") redirect to the active Shopee affiliate product link:

```text
https://s.shopee.ph/4Ve9GTb4bO
```

---

## 📦 Shopify Theme Archive (`archive/`)

The original Shopify Liquid theme is archived with the direct checkout URL setting pre-configured.

- **[`archive/shopify-theme/`](archive/shopify-theme/)** — Full uncompressed Shopify theme source files (`assets/`, `blocks/`, `config/`, `layout/`, `locales/`, `sections/`, `snippets/`, `templates/`).
- **[`archive/shopify-theme.zip`](archive/shopify-theme.zip)** — Ready-to-upload ZIP package for Shopify Admin.

### Uploading to Shopify Admin
1. Go to **Shopify Admin** → **Online Store** → **Themes**.
2. Click **Add theme** → **Upload zip file**.
3. Select `archive/shopify-theme.zip`.

### Developing with Shopify CLI
```bash
cd archive/shopify-theme
shopify theme dev --store tytg51-g3.myshopify.com
```

---

## 💻 Local Preview
To preview locally in your browser without any server setup:
```powershell
Start-Process "index.html"
```
