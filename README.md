# Nora Whitcombe Real Estate: realtor website template

A one-page website for a residential realtor. It's plain HTML, CSS and JavaScript in a single `index.html` with no build step, so it runs on GitHub Pages as-is.

## Highlights
- **Day-to-dusk hero.** The hero photo is a draggable before/after slider showing the same house at 2 pm and at dusk with the lights on. On load it sweeps once from day to dusk. It works with a mouse, a finger or the arrow keys.
- **Listing photo before/after** in the selling section: a dull phone snapshot next to the finished listing photo.
- **Listings** with filters and a pop-up for each home (photo gallery, details, "Book a showing" that fills in the contact form).
- **Interactive neighbourhood map** with median prices and days on market. Map dots open listings, and each area can filter the listings grid.
- **Mortgage calculator** using Canadian rules (semi-annual compounding, CMHC insurance under 20% down, the $1.5M rule).
- Reviews, about section, a three-way contact form (valuation, showing, question) and a sticky Call / Valuation bar on phones.
- SEO basics: meta description, Open Graph tags and `RealEstateAgent` structured data (JSON-LD). Respects reduced-motion settings.

## Customizing for a client
- **Name and details:** search `index.html` for `Nora`, `Whitcombe`, `Port Ashby`, `555` and `whitcombehomes.ca`, and update the JSON-LD block in `<head>`.
- **Colours:** change the CSS variables at the top of `<style>` (`--lamp` is the accent, `--night` the dark colour).
- **Listings and neighbourhoods:** edit the `listings` and `hoods` arrays at the top of the script. `img` is an Unsplash photo ID; swap in the client's own image URLs in the `U()` helper if needed.
- **Hero photo:** replace the two Unsplash URLs in the hero SVGs. The window-glow rectangles in the dusk layer are positioned for this photo (in a 1200×800 frame), so move them to match a new photo's windows.
- **Contact form:** it shows a thank-you message only. To receive emails, point it at a service such as Formspree and remove the `preventDefault` demo handler.

Photos come from [Unsplash](https://unsplash.com) (free to use) and load from their CDN.
