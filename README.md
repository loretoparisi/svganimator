# SVG Animator

SVG Animator is a single-file browser app for turning static SVG diagrams into step-by-step animations. It runs entirely in the browser from `svg-animator.html`: no build step, server, or backend is required.

## Features

- Load an SVG file by drag and drop, file picker, or the built-in demo diagram.
- Detect animatable SVG elements such as groups, rectangles, circles, paths, lines, polygons, polylines, and text.
- Play the SVG progressively with transport controls for play, rewind, step backward, step forward, jump to end, and seek.
- Choose animation order: document order, boxes before lines and text, lines before boxes and text, or random.
- Choose animation effect: fade and grow, stroke drawing, slide in, or pop.
- Tune playback speed and delay between elements.
- Inspect and jump through the detected element list.
- Export the current frame as a PNG snapshot.
- Record the full animation to a WebM video using the browser MediaRecorder API.
- Use keyboard shortcuts for quick playback: Space, arrow keys, Home, End, P, and R.

## Usage

Open `svg-animator.html` in a modern browser.

```text
svg-animator.html
```

Then load an SVG using the drop zone or click **Load Demo SVG** to try the built-in sample diagram.

## Browser Support

Core playback works in modern desktop browsers with SVG and Canvas support. Video recording requires browser support for `MediaRecorder` and canvas capture streams, so WebM export availability depends on the browser.

## Project Structure

```text
.
|-- LICENSE
|-- README.md
`-- svg-animator.html
```

## License

MIT License. See `LICENSE`.
