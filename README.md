# Spice Isle Adventures Tours & Water Sports: website demo

A website demo for Spice Isle Adventures (Grand Anse, Grenada). It combines apple.com's layout with the Island Routes Caribbean tours site, in turquoise. The whole site is in one file, `index.html`, with no build step: 19 pages, switched with links like `#/sunset-cruise`.

## Publish on GitHub Pages

1. Open your repository on GitHub (or create a new public one, for example `spice-isle-adventures`).
2. Delete the old files from the earlier version (the separate `.html` pages, the `assets` and `_build` folders, and the old `index.html`).
3. Upload `index.html` and this `README.md` to the repository root.
4. Open **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, then save.
5. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Linking to a page

Add the page name after `#/` at the end of the address:

| Page | Link ending |
| --- | --- |
| Home | `#/` |
| All experiences | `#/experiences` (filters: `#/experiences?cat=snorkel`, `sunset`, `beaches`, `celebrations`, `couples`, `groups`) |
| Underwater Sculpture Park Snorkel | `#/sculpture-park-snorkel` |
| Grenada Sunset Cruise | `#/sunset-cruise` |
| Private Island Tour | `#/private-island-tour` |
| Private Dinner Aboard | `#/private-dinner-aboard` |
| Wonders of Grenada | `#/wonders-of-grenada` |
| Parties & Celebrations | `#/parties-and-celebrations` |
| Private & Bespoke Charters | `#/private-charters` |
| Group Experiences | `#/group-experiences` |
| Trip Inspo and articles | `#/trip-inspo`, `#/sculpture-park-guide`, `#/grenada-sunset-guide`, `#/beaches-by-boat` |
| About Us & Reviews | `#/about` |
| FAQ | `#/faq` |
| Contact Us | `#/contact` |
| Your Enquiry | `#/enquiry` |

The "Demo pages" bar at the bottom of the screen is for showing the client around. Remove it before launch by deleting the `<nav class="demo-pages" ...>...</nav>` line near the end of `index.html`.

## Forms

Forms send nothing until connected. In `index.html`, search for `var SITE=` and fill in:

```js
var SITE={
  enquiryEmail:'',   // the address enquiries should be sent to
  formEndpoint:''    // optional form service URL (Formspree or similar)
};
```

- With `enquiryEmail` set, the "Open in email app" button opens a pre-addressed email.
- With `formEndpoint` set, the enquiry, contact and bespoke forms send straight from the page.
- With both blank, the forms still build the message for the visitor to email or copy.

## Before going live

- Add the client's phone, WhatsApp, email and social media links (search for "to be added").
- Add prices (every experience currently shows "Request a quote").
- Confirm timings, what's included, minimum age, terms and the FAQ answers with the client.
- Replace the placeholder photos and hero video with the client's own.

## Media credits

- Placeholder photos: Unsplash (Unsplash License).
- Sculpture park photos: Boris Kasimov and SunCat, CC BY 2.0, via Wikimedia Commons. Keep this credit while they are used.
- Hero video: Mixkit (Mixkit License).
- Fonts: Playfair Display and Outfit (Google Fonts, Open Font License); system fonts elsewhere.

Website demo by Savvy Tech.
