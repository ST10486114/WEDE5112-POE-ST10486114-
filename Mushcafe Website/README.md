# MushCafe Website

Simple static site for MushCafe Grilled Chicken (school assignment). Contains contact and enquiries pages, basic styling, and example client-side validation.

## Files
- `contactUs.html` — contact page (form + map + contact info)
- `Enquiries.html` — enquiries form page
- `style.css` — site styles (if present)
- `robots.txt` — robots instructions (place at site root)
- `sitemap.xml` — sitemap (place at site root)

## Run locally
- Option A — open file:
  - Double-click `contactUs.html` or `Enquiries.html` in File Explorer.
- Option B — serve via HTTP (recommended):
  - Open PowerShell in the project folder:
    cd "C:\Users\RC_Student_Lab\Documents\Mushcafe Website"
    python -m http.server 8000
  - Open http://localhost:8000/contactUs.html
  - Or use VS Code Live Server → "Go Live".

## Make the forms work
- Use a form service (Formspree, formsubmit.co) or your backend.
- Example (Formspree — replace `{your_form_id}`):

```html
<form method="POST" action="https://formspree.io/f/{your_form_id}">
  <input type="hidden" name="_subject" value="New contact from MushCafe website">
  <!-- keep name,email,subject,message fields -->
  <button type="submit">Send Message</button>
</form>
```

## Changelog

- 2025-11-05 — Project created: added initial pages (contactUs.html, Enquiries.html) and basic styles.
- 2025-11-05 — Implemented client-side form examples and basic validation on contact/enquiries pages.
- 2025-11-17 — Added SEO suggestions and structured data for contactUs.html; created robots.txt and sitemap.xml examples.
- 2025-11-17 — Added README.md with run/deploy instructions and form integration notes.
- 2025-11-19 — Updated README with changelog and deployment notes; flagged and removed accidental sitemap XML appended to contactUs.html (ensure file is cleaned in the project).
- Next steps: replace placeholder URLs/images with real domain, connect forms to a form service or backend, verify site in Google Search Console, and upload robots.txt + sitemap.xml to