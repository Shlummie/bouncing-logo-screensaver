# Bouncing Logo Screensaver

A single-file browser animation inspired by the familiar bouncing disc-video logo screensaver. The canvas-drawn mark moves around the viewport, changes color after impacts, and highlights exact corner hits.

## Run

No build step or dependency installation is required. Open `dvd-screensaver.html` in a modern browser, or serve the directory with any static file server.

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000/dvd-screensaver.html`.

## Implementation

- Uses one full-window `<canvas>`.
- Advances position with `requestAnimationFrame`.
- Reflects velocity at viewport boundaries.
- Cycles through a color palette on collision.
- Detects simultaneous horizontal and vertical impacts as corner hits and draws a short sparkle effect.
- Recalculates bounds after window resizing.

The logo is drawn procedurally; the source folder does not contain a `dvd.png` file. Nothing is fetched from a server and no user data is stored.

## Trademark notice

The stylized DVD mark is used as a cultural reference in this small demonstration. DVD-related names and marks belong to their respective owners. This project is not affiliated with or endorsed by those owners.

## License

The HTML, JavaScript, and original animation code are MIT licensed. The license does not grant rights to third-party trademarks.
