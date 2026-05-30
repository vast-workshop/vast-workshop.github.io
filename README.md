# VAST Workshop

This is a maintainable static workshop site built with Eleventy.

## Local preview

```bash
npm install
npm run dev
```

Open:

```text
http://127.0.0.1:4174/
```

## Build

```bash
npm run build
```

The generated site is written to `_site/`.

## Where to edit

- Homepage content: `src/index.md`
- Site title, subtitle, venue, email: `src/_data/site.json`
- Navigation: `src/_data/navigation.json`
- Call for Papers and topic lists: `src/call-for-papers.md`
- Important dates: `src/_data/dates.json`
- Styles: `src/assets/styles.css`

## GitHub Pages path

If this is deployed as a user or organization site, such as
`https://yourname.github.io/`, keep `baseUrl` in `src/_data/site.json` as `""`.

If this is deployed as a project site, such as
`https://yourname.github.io/vast-workshop/`, set:

```json
"baseUrl": "/vast-workshop"
```
