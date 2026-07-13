# Plan — Flowchart Planner

A single-file, no-build, no-dependency flowchart sketchpad that runs entirely in the browser. Draw freehand, add boxes/decision diamonds/arrows/text, undo mistakes, and save your work — as a PNG image or as an editable project file.

**Live demo:** [aadimdhakal.github.io/Plan](https://aadimdhakal.github.io/Plan/)

Live in one file: `index.html`. No server, no build step, no npm install. Open it and start drawing.

## Features

- **Freehand pencil & eraser** with adjustable stroke width
- **Flowchart shapes** — rectangle ("box"), diamond ("decision"), and arrow
- **Text labels** for annotating boxes and arrows
- **Color palette** plus a custom color picker
- **Undo / Redo** for every action
- **Expandable canvas** — the board automatically grows as you draw near the bottom, and auto-scrolls while you draw near the edge of the screen
- **High-DPI aware** — crisp lines on retina and mobile screens
- **Touch, mouse, and pen support** via the Pointer Events API
- **Save / Open** your board as a `.json` project file, so you can pick up where you left off
- **Export PNG** to share or embed your flowchart anywhere
- **Keyboard shortcuts**: `P` pencil, `E` eraser, `R` box, `D` diamond, `A` arrow, `T` text, `Ctrl/Cmd+Z` undo, `Ctrl/Cmd+Shift+Z` or `Ctrl/Cmd+Y` redo

## Usage

1. Download or clone this repository.
2. Open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge).
3. Pick a tool from the bottom toolbar and start drawing.
4. Use the top toolbar to change color/width, undo/redo, clear the board, or save your work.

No installation, no accounts, no internet connection required after the page loads.

### Saving your work

- **Save** downloads a `flowchart.json` file containing your full board (shapes, strokes, text, colors). Use **Open** to load it back in later and keep editing.
- **PNG** exports a flattened image of your current board, for sharing or pasting elsewhere.

## Deploying

Because it's a single static HTML file with no build step, you can host it anywhere that serves static files, for example [GitHub Pages](https://pages.github.com/):

```bash
# from the repository root
git checkout -b gh-pages
git push origin gh-pages
```

Then enable GitHub Pages for the `gh-pages` branch in your repository settings.

## Project structure

```
.
├── index.html   # the entire app: markup, styles, and logic
├── README.md
└── LICENSE
```

## Contributing

Issues and pull requests are welcome. Since everything lives in one file, most changes are a matter of editing `index.html` directly and testing in a browser.

## License

MIT — see [LICENSE](LICENSE). You're free to use, modify, distribute, and sell this software, including in commercial and closed-source products.
