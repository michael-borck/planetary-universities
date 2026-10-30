# Planetary Universities

Live: https://planetary-universities.eduserver.au

Public landing page for the Planetary Universities research project at Curtin
University. The site is a single teaser page with three layout concepts for the
research leads to review.

## Status

Design concepts are under review. The root page is concept A. Two alternatives
live in `concepts/`:

- Concept A, editorial: `/`
- Concept B, instrument: `/concepts/b.html`
- Concept C, brief: `/concepts/c.html`
- Comparison page: `/concepts/`

Review link: https://planetary-universities.eduserver.au/concepts/

Concepts are marked `noindex` and blocked in `robots.txt`. They will be removed
once a direction is chosen.

## Local preview

No build step. Serve the folder with any static server:

```sh
python3 -m http.server 8080
```

Then open http://localhost:8080.

## Publishing

GitHub Pages serves the repository root from `main`. The custom domain is set
in `CNAME`:

```
planetary-universities.eduserver.au
```

DNS should point that hostname to `michael-borck.github.io` with a CNAME
record. Enable HTTPS in the repository's Pages settings.

`.nojekyll` is present so files and folders beginning with an underscore are
served as-is.

## Structure

```
index.html          concept A, the current default
styles.css
concepts/           comparison page and concepts B and C
assets/             favicon
CNAME               custom domain for GitHub Pages
```

## Reference material

The grant application, award letter, draft conference deck and related source
documents are not part of this repository. They are kept outside it, at
`../planetary-universities-reference/`. Do not add them.

## Content notes

- The pilot figures are preliminary: two universities, two SDGs, one coder,
  not yet reconciled. Keep the caveat wherever they appear.
- The seven-of-nine planetary boundaries figure comes from the Planetary
  Health Check 2025 (PIK).
- The corpus is described as 37 Australian public universities in the grant
  application and about 40 in the conference deck. This site uses 37 until the
  leads confirm the final number.
- The conference talk is dated October 2026. Change "presenting at" to
  "presented at" after the event.

## Licence

Code: MIT, see `LICENSE`. Text and figures: CC BY 4.0, see
`CONTENT-LICENSE.md`.
