# Font licenses

The five SVGs in `assets/` are fully self-contained: each one embeds its fonts
as base64 **WOFF2** inside a `<style>` block. Nothing is fetched from Google
Fonts, a CDN, or any other network location at render time.

Two typefaces are embedded.

## Inter (display / UI)

- Copyright (c) 2016 The Inter Project Authors — https://github.com/rsms/inter
- License: SIL Open Font License, Version 1.1
- Used for: UI text, names, labels, and the oversized display headings
  (`Inter` and `Inter Display`, weights 400/500/600/700 and 800/900)
- Full license text: [`licenses/Inter-OFL.txt`](./licenses/Inter-OFL.txt)

## JetBrains Mono (monospace / technical)

- Copyright 2020 The JetBrains Mono Project Authors — https://github.com/JetBrains/JetBrainsMono
- License: SIL Open Font License, Version 1.1
- Used for: handles, URLs, eyebrows, captions and all technical labels
  (weights 400/700)
- Full license text: [`licenses/JetBrainsMono-OFL.txt`](./licenses/JetBrainsMono-OFL.txt)

## Subsetting

Each face was subset with `fontTools` to the printable ASCII range plus a small
set of symbols used in the layouts, then converted to WOFF2. Subsetting is an
explicitly permitted modification under the OFL, and the fonts are **not**
sold, and are not redistributed as standalone font files — they are embedded
inside the SVG documents only.

Resulting embedded sizes:

| Face | Embedded WOFF2 |
| --- | --- |
| Inter Regular / Medium / SemiBold / Bold | ~20 KB each |
| Inter Display ExtraBold / Black | ~19 KB each |
| JetBrains Mono Regular / Bold | ~20 KB each |

## Licensing note for redistributors

Both licenses permit embedding and redistribution inside documents such as
these SVGs, provided the copyright notice and license are retained. If you fork
this profile, keep this file and the `licenses/` directory with it.

No fonts are bundled in this repository as installable `.ttf`/`.otf` files.
