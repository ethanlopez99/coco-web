# coco-web

Static marketing + deep-link fallback pages for Coco.

## Universal links setup

1. Host the AASA file at `/.well-known/apple-app-site-association`.
2. Replace `TEAMID` inside the AASA file with your Apple Team ID.
3. Ensure the AASA file is served with `Content-Type: application/json` and no redirects.

## Fallback landing page

- Use `app.html` as the universal link entry point.
- Example share URL: `https://the-coco-app.com/app.html?path=/recipe/123`.
- Update the App Store link in `app.html` once you have the app ID.

Note: Open Graph tags in `app.html` are generic; per-content previews require server-side rendering.
