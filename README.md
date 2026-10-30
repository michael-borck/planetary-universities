# Planetary Universities

Live: https://planetary-universities.eduserver.au

Public landing page for the Planetary Universities research project at Curtin
University. The site is a single teaser page using the instrument direction the
research team chose in October 2026.

The other design concepts are preserved in the `design-concepts` git tag. They
are not part of the live site.

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

DNS points that hostname to `michael-borck.github.io` with a CNAME record.
HTTPS is enforced in the repository's Pages settings.

`.nojekyll` is present so files and folders beginning with an underscore are
served as-is.

## Structure

```
index.html          the landing page
styles.css
assets/             favicon and social preview image
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

## Licence

Code: MIT, see `LICENSE`. Text and figures: CC BY 4.0, see
`CONTENT-LICENSE.md`.
