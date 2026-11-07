# inkecode.com

The website of INK & CODE LTDA, a software studio from Curitiba, Brazil. It is plain static HTML and one stylesheet, served by GitHub Pages at <https://inkecode.com>. There is no JavaScript and no build step.

## Structure

```
index.html                 English landing (primary language)
privacy/index.html         Privacy Policy (English translation)
terms/index.html           Terms of Use (English translation)
pt/index.html              Portuguese landing
pt/privacidade/index.html  Política de Privacidade (prevailing version)
pt/termos/index.html       Termos de Uso (prevailing version)
404.html                   Bilingual not-found page
assets/css/site.css        The only stylesheet
assets/fonts/              Self-hosted fonts and their licenses
assets/img/                Favicon, touch icon, app icon
CNAME, .nojekyll, robots.txt, sitemap.xml
```

Every page sets a Content-Security-Policy that allows only same-origin resources and no scripts, so all styling lives in `assets/css/site.css` (no inline styles).

## Preview locally

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000/>. Paths are root-absolute, so serve from the repository root.

## Licenses

- Fonts (Space Grotesk, JetBrains Mono, Instrument Serif) are under the SIL Open Font License 1.1; see the `LICENSE-*.txt` files in `assets/fonts/`.
- All other content (text, images, code of this site) © 2026 INK & CODE LTDA. All rights reserved.
