# Alex Maxham — portfolio mockup

A single-page portfolio mockup for a tech journalist writing for Android Headlines,
built in the Material 3 Expressive design language.

Open `index.html` in a browser. There is no build step and no dependencies beyond
Google Fonts (Roboto Flex and Material Symbols Rounded).

## What's in it

- **Hero** with expressive display type, a morphing portrait placeholder, and topic chips.
- **Featured story** card and a **filterable grid** of recent bylines (Reviews, News, Buying guides, Explainers, Deals).
- **Beats**, **About**, and a **Social** section with copy-to-clipboard handles.
- **Light / System / Dark** theme switcher in the top app bar. The choice is remembered in `localStorage`; "System" follows `prefers-color-scheme`.
- Extended FAB, snackbar, segmented button group, chips, tonal surfaces, and springy shape-morph motion per Material 3 Expressive.

## Theming

All colors are Material 3 color roles defined as CSS custom properties on `:root`
(light), with the dark scheme repeated under `@media (prefers-color-scheme: dark)` and
`:root[data-theme="dark"]`. The palette is a custom teal seed with a warm coral tertiary
and deliberately does not use the Android Headlines brand kit. Swap the role values at
the top of the `<style>` block to re-skin the whole page.

## Placeholders to replace

- Article titles, dates, read times, and the three "by the numbers" stats.
- Social handles, the email address, and the "Based in" fact.
- The portrait (currently initials on a morphing blob) and article art (gradient tiles).
- Every link marked `data-placeholder` shows a snackbar instead of navigating. Point these at live Android Headlines URLs.
