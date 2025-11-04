# Professor Homepage (Static)

An elegant, minimal academic homepage for a Computer Science professor. Includes:

- English-only design, academic style
- Sections: About, Selected Publications, Projects, Students, Contact
- Dedicated students directory and a redirect list for student homepages
- Responsive, accessible layout with dark academic theme

## Structure

- `index.html` — main professor homepage
- `students.html` — full student roster (PhD/M.S., current and alumni)
- `students-redirects.html` — maintains slug→URL mapping for student personal pages and performs client-side redirects
- `teaching.html` — teaching page with current and past courses
- `talks.html` — invited talks and presentations
- `cv.html` — CV page embedding a local `assets/pdf/cv.pdf`
- `assets/css/styles.css` — sitewide styles
- `assets/img/` — SVG images (favicon, professor illustration, avatars)
- `assets/pdf/` — put your `cv.pdf` here

## Customize

- Replace text content directly in the HTML files.
- Update student links in `students-redirects.html` (the `mapping` object).
- Replace SVGs in `assets/img/` with your own images (keep file names or update HTML references accordingly).

## Preview locally (Windows, cmd)

You can open `index.html` directly in a browser, or run a tiny server for cleaner relative links.

Optional: using Python (already on many systems):

```cmd
python -m http.server 8000
```

Then open: http://localhost:8000/index.html

## Notes

- All links to external student pages are placeholders; update them to real URLs.
- The site uses no frameworks and works on any static host (GitHub Pages, university servers, etc.).
 - Light theme is enabled by default; customize colors in `:root` CSS variables.
