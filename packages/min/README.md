# `astro-min`

> Extremely Fast and Smart Minification of 🟠 HTML 🟡 JS 🔵 CSS 🟣 SVG  
> Meticulously optimized for Speed 🥇 and Effectiveness 🏅

[![Built with Astro](https://astro.badg.es/v2/built-with-astro/tiny.svg)](https://astro.build)
[![NPM Package Version](https://img.shields.io/npm/v/astro-min?style=flat-square)](https://www.npmjs.com/package/astro-min)
[![Package Install Size](https://packagephobia.com/badge?p=astro-min&style=flat-square)](https://packagephobia.com/result?p=astro-min)
[![License: MIT][license-src]][license-href]
[![Style: TS-Standard][codestyle-src]][codestyle-href]
[![GitHub Repo Stars][gh-repo-stars-img]][gh-repo-url]

## Feature Highlights ✨

- 👟 fastest processing ~1000 files/s
- 🪶 lighter build output ~25% smaller
- 📦 small packaged size ~30KB

## Feature Roadmap 🌱

- [x] HTML, CSS, JS, SVG
- [x] Files and inline Code
- [x] Static Site Minification

- [ ] Support SSR / Hybrid Rendering
- [ ] Remove Comments from external CSS/JS

## Getting started 🎯

Use your package manager of your choice

```sh
# NPM
npm run astro add astro-min

# Bun
bun astro add astro-min

# PNPM
pnpm astro add astro-min

# Yarn
yarn astro add astro-min
```

### Manual Installation 🧑‍💻

1. Install package `astro-min`

2. Import and add to integrations list

```js
//astro.config.mjs
import { defineConfig } from 'astro/config'
import minify from 'astro-min'

export default defineConfig({
  integrations: [minify()]
})
```

## Options 🔧

```js
//astro.config.mjs
import { defineConfig } from 'astro/config'
import minify from 'astro-min'

export default defineConfig({
  integrations: [
    minify({
      do_not_minify_doctype: false,
      ensure_spec_compliant_unquoted_attribute_values: false,
      keep_closing_tags: false,
      keep_comments: false,
      keep_html_and_head_opening_tags: false,
      keep_input_type_text_attr: false,
      keep_spaces_between_attributes: false,
      keep_ssi_comments: false,
      minify_css: false,
      minify_js: false,
      preserve_brace_template_syntax: false,
      preserve_chevron_percent_template_syntax: false,
      remove_bangs: false,
      remove_processing_instructions: false,
    })
  ]
})
```

## Development

[![Open in StackBlitz][open-in-sb]](https://stackblitz.com/github/advanced-astro/astro-min)
[![Open with CodeSandbox][open-in-csb]](https://codesandbox.io/p/sandbox/github/advanced-astro/astro-min)
[![Open in GitHub Codespaces][open-in-ghc]](https://codespaces.new/advanced-astro/astro-min?devcontainer_path=.devcontainer/minimal/devcontainer.json)
[![Open in Gitpod][open-in-gp]](https://gitpod.io/#https://github.com/advanced-astro/astro-min)

## Learn more 🔖

- <https://warpspeed-world.github.io/css-minification-benchmark/>
- <https://github.com/neon-bindings/neon>

## Colophon

- <https://tsup.egoist.dev>
- <https://github.com/frontendista/astro-html-minify>
- <https://github.com/wilsonzlin/minify-html>

[codestyle-src]: https://flat.badgen.net/badge/code%20style/ts-standard/blue?icon=typescript
[codestyle-href]: https://github.com/standard/ts-standard

[gh-repo-stars-img]: https://img.shields.io/github/stars/advanced-astro/astro-min
[gh-repo-url]: https://github.com/advanced-astro/astro-min

[license-src]: https://flat.badgen.net/github/license/amio/badgen
[license-href]: https://opensource.org/license/isc-license-txt/

[open-in-csb]: https://assets.codesandbox.io/github/button-edit-lime.svg
[open-in-ghc]: https://github.com/codespaces/badge.svg
[open-in-gp]: https://gitpod.io/button/open-in-gitpod.svg
[open-in-sb]: https://developer.stackblitz.com/img/open_in_stackblitz.svg

## Changelog
