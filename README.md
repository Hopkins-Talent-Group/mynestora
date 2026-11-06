# MyNestora — Storefront & Theme

A fast, lightweight e-commerce storefront for **MyNestora** with direct Shop Pay checkout integration.

---

## 🚀 Live Static Storefront (Root)

The root of this branch contains the standalone static storefront ready for deployment (GitHub Pages, Vercel, Netlify, or local preview):

- **[`index.html`](index.html)** — Homepage featuring the hero banner, brand styling, announcement bar, and product showcase.
- **[`product.html`](product.html)** — Product detail page for the **MyNestora Turbo Vac** featuring interactive photo gallery, live pricing, badges, and trust assurances.
- **[`images/`](images/)** — Brand assets and product photography organized by category.

### Direct Shop Pay Checkout Link
All purchase buttons ("Shop all", "Buy it now", Shop Pay button, and product cards) redirect to the active dropshipping checkout:

```text
https://shop.app/checkout/81753374950/cn/hWNIpKekBssPGtDWZ5ultSZY/en-us/shoppay_login?_mcs=3.AMPS&_r=AQAB1WSgM9j2ZiyklrdxyqKO5ZmtbsS3E8dnDT2mMOktz3gWNxSc&redirect_source=direct_checkout_product&tracking_unique=0253b564-04a6-4506-94a1-ac8e2598de0b&tracking_visit=c5e2a50e-7009-41a7-8d08-a6bee22505a6
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
