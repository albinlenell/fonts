# LenéllR&D Fonts

Self-hosted webfont CDN for the **AbreuDidot** typeface family, served via GitHub Pages.

> **Specimen & docs:** [albinlenell.github.io/fonts](https://albinlenell.github.io/fonts/)

---

## Quick start

```html
<!-- Load a single optical size -->
<link rel="stylesheet"
      href="https://albinlenell.github.io/fonts/css/abreudidot-24.css">

<!-- Or load all sizes at once -->
<link rel="stylesheet"
      href="https://albinlenell.github.io/fonts/css/abreudidot-all.css">
```

```css
h1 {
  font-family: 'AbreuDidot 64', serif;
  font-weight: 300;
}

body {
  font-family: 'AbreuDidot 11', serif;
  font-weight: 300;
}
```

---

## Optical sizes

Each optical size is a separate `font-family`, optimized for its intended point size.

| Family | CSS file | Intended use |
|--------|----------|-------------|
| `AbreuDidot 06` | `abreudidot-06.css` | Caption, fine print |
| `AbreuDidot 11` | `abreudidot-11.css` | Body text |
| `AbreuDidot 16` | `abreudidot-16.css` | Subheadings |
| `AbreuDidot 24` | `abreudidot-24.css` | Headings |
| `AbreuDidot 42` | `abreudidot-42.css` | Display |
| `AbreuDidot 64` | `abreudidot-64.css` | Large display |
| `AbreuDidot 96` | `abreudidot-96.css` | Banner, poster |

## Weights & styles

Each optical size includes:

| Weight | Value | Styles |
|--------|-------|--------|
| Light | `300` | normal, italic |
| Medium | `500` | normal, italic |
| Bold | `700` | normal, italic |

**42 font files total** (7 sizes × 3 weights × 2 styles).

---

## Repository structure

```
/
├── css/
│   ├── abreudidot-06.css
│   ├── abreudidot-11.css
│   ├── abreudidot-16.css
│   ├── abreudidot-24.css
│   ├── abreudidot-42.css
│   ├── abreudidot-64.css
│   ├── abreudidot-96.css
│   └── abreudidot-all.css
├── woff2/
│   ├── AbreuDidot-06Light.woff2
│   ├── AbreuDidot-06LightItalic.woff2
│   ├── AbreuDidot-06Medium.woff2
│   ├── ...
│   └── AbreuDidot-96BoldItalic.woff2
├── index.html          (specimen page)
└── README.md
```

## Adding font files

Place your `.woff2` files in the `woff2/` directory. To convert from OTF/TTF:

```bash
# Install woff2 tools
brew install woff2    # macOS
apt install woff2     # Ubuntu/Debian

# Convert
woff2_compress AbreuDidot-11Light.otf
```

## Enabling GitHub Pages

1. Go to **Settings → Pages**
2. Set source to **Deploy from a branch**
3. Select **main** branch, **/ (root)** folder
4. Save

Your fonts will be available at `https://albinlenell.github.io/fonts/`

---

*LenéllR&D Fonts*
