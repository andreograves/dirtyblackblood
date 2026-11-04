# dirtyblackblood

Rebuild of [dirtyblackblood.com](https://dirtyblackblood.com) as a static [Astro](https://astro.build) site.

> Status: scaffold with placeholder content. The real copy, images and
> styling from the current site still need to be brought over.

## Develop

```sh
npm install
npm run dev      # http://localhost:4321
npm run build    # outputs static site to dist/
npm run preview  # serve the built site locally
```

## Structure

- `src/site.config.ts`: site name, tagline, nav links, socials, contact email
- `src/layouts/Base.astro`: page shell (head/meta, header, footer)
- `src/components/`: header and footer
- `src/pages/`: one file per route (`index`, `about`, `contact`, `404`)
- `src/styles/global.css`: design tokens (colors, fonts) and base styles
- `public/`: static assets served as-is (favicon, images)

To add a page, create `src/pages/<name>.astro` using the `Base` layout and add it to `nav` in `src/site.config.ts`.
