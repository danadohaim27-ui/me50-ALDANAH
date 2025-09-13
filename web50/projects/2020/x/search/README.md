# CS50W Project 0 — Search (Student Frontend)

This folder contains a simple static frontend that submits queries to Google, Google Images, and Google Advanced Search using **GET parameters**.

## Files
- `index.html` — main page with **Google Search** and **I'm Feeling Lucky**.
- `images.html` — **Google Image Search** using `tbm=isch`.
- `advanced.html` — **Advanced Search** using parameters: `as_q`, `as_epq`, `as_oq`, `as_eq`.
- `styles.css` — basic Google-like styles.

## How it works
- All forms use `action="https://www.google.com/search"` with `method="GET"`.
- Main search uses the `q` parameter.
- **I'm Feeling Lucky** sets `btnI=I'm Feeling Lucky` (sent automatically by naming the submit input `btnI`), which tells Google to skip the results page.
- Image search uses a hidden `tbm=isch` parameter.
- Advanced search maps to Google's documented parameters:
  - **All these words** → `as_q`
  - **Exact word or phrase** → `as_epq`
  - **Any of these words** → `as_oq`
  - **None of these words** → `as_eq`

## Running locally
Open any of the HTML files directly in your browser by double-clicking them, or use a simple HTTP server:

```bash
# Python 3
python -m http.server 8000
# then visit http://localhost:8000/index.html
```

## Submission tips
- Place these files at: `web50/projects/2020/x/search/` in your GitHub repo.
- Your final paths should look like:
  - `.../search/index.html`
  - `.../search/images.html`
  - `.../search/advanced.html`
  - `.../search/styles.css`
- Record a <=5-minute screencast demonstrating each spec item, with timestamps in the description.
