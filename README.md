# JUNO: Little Worlds website

The product, support and privacy pages for **JUNO: Little Worlds**, a calm pet and puzzle game for children on iPhone and iPad, in English and Swedish. Published with GitHub Pages at https://tintronix-lab.github.io/Juno-LittleWorlds/.

- `index.html`: product page
- `support.html`: help for parents and how to get in touch
- `privacy.html`: privacy for parents

English is at the root; Swedish is in `sv/`.

## Editing

The HTML files are generated: do not edit them by hand.

- Text lives in `i18n/en.json` and `i18n/sv.json`, with the same keys.
- Layout lives in the templates in `build.mjs`; styles in `styles.css`.
- `node build.mjs --check` verifies the Swedish against the English (same keys, links and placeholders) and that the turtle is called GrandPa Tintin in English and Morfar Tintin in Swedish.
- `node build.mjs` writes all pages. Commit the result: GitHub Pages serves the `main` branch as it is.

The screenshots in `assets/` come from the game's production build at iPhone size. The site has no cookies, analytics, fonts or scripts from anywhere else, like the game itself.
