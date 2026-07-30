# Color Palette from Image

Extract a dominant color palette from any image, right in your browser. No server, no tracking, no third-party scripts.

**Live demo:** https://0xelitesystem.github.io/color-palette-from-image/

## Use

Open `index.html` in any modern browser, or visit the GitHub Pages link in the repo description.

Drag an image onto the drop zone, or click to pick a file. The tool samples the pixels on a canvas and clusters them with median cut quantization, then shows:

- A preview of your image
- A palette of dominant colors (choose 4, 6, 8, or 12)
- Each swatch with its HEX value, RGB value, and a copy button
- A "Copy all HEX" button for the whole palette

Change the color count and the palette re-extracts from the same image.

## Why this exists

Most palette extractors upload your image to a server or load a heavy library from a CDN. This is a single HTML file that does the clustering locally with median cut, so it works offline and keeps your image on your machine. Good for pulling brand colors out of a logo, building a theme from a photo, or grabbing accent colors from a screenshot.

## Privacy

Everything runs in your browser. The image is read into a canvas with FileReader and never leaves your machine. You can verify by viewing the page source or by opening DevTools and watching the network tab, no requests are made.

## Run locally

```bash
git clone https://github.com/0xelitesystem/color-palette-from-image
cd color-palette-from-image
# Open index.html in your browser, or:
python -m http.server 8000
```

## Build

There is no build. It's a single HTML file.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT.

## Related

- [color-contrast-checker](https://github.com/0xelitesystem/color-contrast-checker)
- [color-format-converter](https://github.com/0xelitesystem/color-format-converter)
- [gradient-generator](https://github.com/0xelitesystem/gradient-generator)
