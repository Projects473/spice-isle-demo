# Spice Isle Adventures Tours & Water Sports: demo site

A single-page demo with eight design samples for the client to compare. Everything is in `index.html`; there is no build step.

## Publish on GitHub Pages

1. Create a new public repository (for example `spice-isle-demo`).
2. Upload `index.html` and this `README.md` to the repository root.
3. Open **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, then save.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Linking to one sample

The bar at the bottom of the page switches samples. To open a specific one, add its name to the address:

| Sample | Link ending |
| --- | --- |
| 1 · Silversea | `#style-silversea` |
| 2 · Regent | `#style-regent` |
| 3 · Grandium | `#style-grandium` |
| 4 · Kanila | `#style-kanila` |
| 5 · Original | `#style-signature` |
| 6 · CozyStay | `#style-cozystay` |
| 7 · LetsGo 1 | `#style-letsgo` |
| 8 · LetsGo 2 | `#style-letsgo2` |

## Enquiry form

Near the top of the script at the bottom of `index.html`:

```js
var SITE={
  enquiryEmail:'',   // the address enquiries should be sent to
  formEndpoint:''    // optional form service URL (Formspree or similar)
};
```

- With `enquiryEmail` set, "Open in email app" opens a pre-addressed email.
- With `formEndpoint` set, enquiries are sent straight from the page.
- With both blank, the form still builds the enquiry for the visitor to email or copy.

## Before going live

- Replace the placeholder photos and hero videos with the client's own media.
- Add the client's phone number and email in the footer.
- Confirm prices, durations and crew names with the client.

## Media credits

- Placeholder photos: Unsplash (Unsplash License).
- Sculpture park photos: Boris Kasimov and SunCat, CC BY 2.0, via Wikimedia Commons. Keep this credit while the photos are in use.
- Hero videos: Mixkit (Mixkit License).

Demo concept by Savvy Tech.
