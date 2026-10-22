# Oasis Automations blog

Plain static HTML. No build step, no markdown.

## Add a new post
1. Pick a short slug, e.g. `my-new-post`.
2. Copy `blog/_template.html` to `blog/my-new-post/index.html`.
3. In the new file, delete the first comment line, then replace every `{{...}}` placeholder:
   `{{TITLE}}`, `{{SUMMARY}}` (one sentence), `{{DATE ...}}` (e.g. `Nov 4, 2026`), `{{N}}` (minutes to read), `{{TAG}}`.
   Also delete the `<meta name="robots" content="noindex">` line.
4. Write the post inside `<article>` using `<p>`, `<h2>`, `<ul><li>`, `<ol><li>`, `<blockquote>`, `<a>`. A boxed aside is `<div class="note">…</div>`.
5. In `blog/index.html`, copy one `<a class="post-card">…</a>` block, paste it at the top of the list (newest first), and update the link, date, tag, title, and summary.
6. Commit and push to `main`. GitHub Pages updates in about a minute.

## Files
- `assets/blog.css` – shared styles (slate, teal, silver).
- `assets/mark.svg` – palm-in-ring mark for dark backgrounds; `assets/badge.svg` – same mark on a slate disc (favicon, light backgrounds).
- `assets/lockup.jpg`, `assets/og.jpg` – wide logo for the blog hero and link previews.

## House rules
Plain first-person voice, no hype, no income claims. Never post client plans, client names, or job details.
