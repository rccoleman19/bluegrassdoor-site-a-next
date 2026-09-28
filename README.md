# Bluegrass Commercial Door & More website

Static website for Bluegrass Commercial Door & More, 930 Gordon Avenue, Bowling Green, KY 42101 · 270-780-3235.

The homepage opens on the door builder: the visitor builds one or more doors, and only then asks for a quote on exactly those doors.

- `index.html`: the page (door builder first, then projects, reviews, services, about, service area, contact)
- `styles.css`: mobile-first styles (brand navy #0033A0, Barlow / Barlow Condensed)
- `app.js`: menu, call bar, the door builder (steps → finished doors → quote request → email hand-off), shared build links (`#build=`), help chat, photo lightbox
- `builder-rules.js`: hardware compatibility rules (one list; edit it to change what the builder allows, adds, renames or notes)
- `door-spec.js`: door catalog, the spec wording used on the page and in the email, and the link format (base64url JSON)
- `door-preview.js` / `door-preview.css`: door drawings (live beside the steps on desktop, and on each finished door)
- `door-visualize.js` / `door-visualize.css`: optional "See it on your building" step (the photo never leaves the visitor's device)
- `request.html` / `request.js` / `request.css`: a quote request as the office sees it, drawn entirely from its own link (`request.html#b=...` or `?b=...`); nothing is stored on the website
- `images/`: company photos and logo

Quote requests are delivered by the visitor's own email app (a pre-filled email to sonya@bluegrassdoor.com).

Run it locally with `python3 -m http.server` in this folder, then open http://localhost:8000.
