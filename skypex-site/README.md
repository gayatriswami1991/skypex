# Skypex Supplies homepage (static HTML)

Open `index.html` in a browser. No build step, no dependencies. Keep the `assets/` folder next to it.

## Structure
- `index.html`: one file with all CSS (in `<style>`) and JS (before `</body>`). JSON-LD (LocalBusiness, WebSite, FAQPage) is in `<head>`.
- `assets/img/`: photos, logos and banners (jpg/png). `assets/video/`: product videos (mp4, H.264, muted, loop).
- Fonts: Lato and Roboto from Google Fonts (the only external request).

## Sections (ids)
`#top` hero carousel (3 slides) | `#who` who we supply | `#cakemix` Skybake cake mixes | `#range` baking supplies by category (cream, fillings, bread, packaging) | `#chocolate` | `#order` WhatsApp order builder | `#why` about | `#trust` partners and recognition | `#learn` guides | `#reviews` Google reviews | `#instagram` | `#faq` | footer.

## To do before going live
1. Replace every `[CONFIRM]` / `[ADD]` placeholder in the text (search the file): minimum order, delivery, payment, baking-desk person, Top 100 year/issuer, partner letters.
2. Google reviews (`#reviews`): paste 3 real reviews with name and date, or embed a Google reviews widget. Rating is a placeholder.
3. Missing product photos: cards and tiles for these hide themselves until the file exists in `assets/img/`: cakemix25, sugarpaste, coconut, prestige, savor, delifruit, frutti-cans, komplet, victoria, moulds.
4. Replace `logo-pristine.png` with the official Pristine logo (current one is cropped from a pack photo). Add a sharp Frutti logo if wanted.
5. Update `og:image` and `canonical` to the real absolute URLs. Check `LocalBusiness` JSON-LD values.
6. WhatsApp number is `254722386394` (search and replace to change). Phone, email and address are in the footer and JSON-LD.
7. Optional: compress videos further or host them on a CDN. Add width/height to images and `loading="lazy"` for below-the-fold images.

## Notes for WordPress/Elementor
Sections map to Elementor containers. Brand/page links point to existing pages on skypex.co.ke. Videos use `data-src` and are loaded when scrolled into view (IntersectionObserver).

## Spare files
Not used on the page right now, kept for reuse: `assets/video/glaze.mp4`, `sprinkles.mp4`, `yeast.mp4`, `clearglaze.mp4`, `showcase.mp4` and matching `*-poster.jpg`, plus `skypower-logo.png`.
