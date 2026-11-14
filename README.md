# Elle Driving School website

https://www.elledrivingschoolsleaford.co.uk

This repository is the whole site. GitHub Pages builds it with Jekyll on every
push to `main`, so there is no separate source repository and no build step
to run. Editing a file on github.com and committing is enough.

## Common edits

| To change | Edit |
| --- | --- |
| Add a recommendation | `_data/reviews.yml` (copy a block to the top) |
| Phone, email, Facebook, areas covered, test centre | `_config.yml` |
| Prices | `prices.html` |
| Home page text and FAQs | `index.html` |
| Header, footer | `_includes/header.html`, `_includes/footer.html` |
| Page frame, meta tags | `_layouts/default.html` |
| Styling | `assets/css/site.css` |

Each page starts with a block between `---` lines. `title` and `description`
are what Google shows in search results; `heading` is the large heading on the
page.

## Previewing locally (optional)

    docker run --rm -p 4000:4000 -v "$PWD":/srv/jekyll jekyll/jekyll:3.8 jekyll serve

Then open http://localhost:4000.
