# Logue legal texts

The source of the legal documents published on [logue.is](https://logue.is):

- [`privacy.md`](privacy.md): Privacy Policy, shown at
  [logue.is/privacy](https://logue.is/privacy)
- [`terms.md`](terms.md): Terms of Service, shown at
  [logue.is/terms](https://logue.is/terms)

The Logue app includes this repository as a git submodule and renders the
Markdown on those pages. A change here goes live once the submodule is updated
in the app and the app is deployed.

## Format

Each document starts with a front matter block:

```md
---
title: Privacy Policy
updated: 2026-10-12
---
```

- `title` is the page heading.
- `updated` (`YYYY-MM-DD`) is shown as "Last updated". Change it with every
  change to the text.

The body is written with one line per paragraph and per list item, without
hard wrapping: a line break inside a paragraph is shown as a line break on the
site.

It can use headings (`##`, `###`), paragraphs, bulleted and numbered lists,
**bold**, _italic_, `code`, and links. Links must be absolute
(`https://logue.is/terms`, `mailto:...`).

Tables, block-level images, HTML and horizontal rules are not supported and
fail the app's build.
