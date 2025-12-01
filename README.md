# Results Summary Component

Simple responsive UI that reproduces the "Results Summary" card (Frontend Mentor style). Built with plain HTML and CSS.

## Preview
See the screenshot in the repository (desktop layout). The component shows:
- Left: gradient result card with a circular score badge.
- Right: summary list with icon rows and a centered CTA button.

## Files
- index.html — markup
- style.css — styling

## Features
- Two-column card layout
- Circular score badge that can overlap the card edge
- Iconed summary rows with right-aligned scores
- Centered CTA button
- Responsive-friendly using flexbox

## Quick setup (Windows)
1. Open the project folder in VS Code:
   - `code .`
2. Open the page in your browser:
   - Double-click `index.html` or in Terminal run:
     - `start index.html`
   - Or use Live Server extension.

## Helpful CSS tips (what to tweak)
- Center page: body uses flexbox (min-height: 100vh; display: flex; align-items: center; justify-content: center).
- Make the circular score overlap the top: give `.your-result .number` a negative top margin (e.g. `margin-top: -80px`) and set `.your-result { overflow: visible; }`.
- Resize SVG icons: change `.entries svg { width: 20px; height: 20px; flex: 0 0 20px; }`.
- Right-align score text: `.entries .percent { margin-left: auto; }`.
- Center button: `button { display: block; margin: 20px auto 0; }`.

## Structure
- `.your-result` — left card (gradient)
- `.number` — circular badge with score
- `.summary` — right card, contains `.entries` rows
- `.entry-*` — individual row, each is a flex row with icon, label and `.percent`

## License & Credits
- Project scaffold based on Frontend Mentor challenge ideas.
- Use freely for practice and portfolio.
