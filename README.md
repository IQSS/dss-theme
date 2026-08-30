# dss-theme

A Quarto extension carrying the look of IQSS Data Science Services (Questrial
headings, Montserrat text, the IQSS blue and orange, the DSS wordmark, the
standard navbar links and footer with the IQSS logo, a Light / Dark / System
switch, and callouts, images, figures, and code output that hold in both
modes), so that the
workshops site, the beginner's guides, and any future DSS page share one look
from one place. For the DSS
team and for anyone building a DSS-branded Quarto site.

## Use

```sh
quarto add IQSS/dss-theme
```

Then `project: type: dss-theme` in `_quarto.yml` for a website with the DSS
navbar and footer, or `format: dss-theme-html` to take only the HTML format.
Update with `quarto update IQSS/dss-theme`.

For a Quarto book, `project: type: dss-theme-book` instead: the same navbar,
footer, and favicon under `book:` (an extension contributes one project type,
so books have their own; `quarto add` installs both). The book title stays
off the navbar, on the cover page and in the tab.

## Develop

`quarto preview` at the repository root renders the two-page demo
(`index.qmd`, `sample.qmd`) with the extension in `_extensions/dss-theme/`.
Edit `dss.scss`, look, bump `version` in `_extension.yml`.
