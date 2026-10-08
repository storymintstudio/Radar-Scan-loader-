# Radar Scan Loader

A radar-style loading component with a rotating sweep, flashing blips, and a jet that flies along a flight path as the progress fills. Pure HTML, CSS and JavaScript, no libraries.

## Features

- Rotating radar sweep with blips that flash in sync as the line passes them
- Jet that follows a curved path, driven by the same progress value as the counter
- Status text that changes through each stage, ending in "Mission complete ✓"
- Click the card to replay
- Glassmorphism card, responsive, respects reduced motion

## Usage

1. Download `index.html` (or `radar-loader.html`).
2. Open it in any browser.

No install or build step.

## Customize

Change the colors at the top of the CSS:

```css
:root {
  --accent: #4de1ff;  /* sweep, rings, progress line */
  --signal: #ffb347;  /* jet and blips */
}
```

In the script:

- `DURATION` sets how long the load takes in milliseconds (default `6000`)
- `steps` holds the status messages and the percentage where each one appears

To add a blip, copy one `<i class="blip">` line and set `--a` (angle in degrees) and `--r` (distance from center, 0 to 1).

## Tech

HTML, CSS (conic-gradient, backdrop-filter), vanilla JavaScript, SVG path animation.

## Credits

First draft generated with AI, customized and crafted by Storymint Studio.

Follow for a new UI drop every week: [@storymint.studio](https://instagram.com/storymint.studio)
