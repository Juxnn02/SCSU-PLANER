# SCSU Open House — Event Itinerary Builder

A responsive, single-page web application for building personalized itineraries for Southern Connecticut State University's Open House events. This lightweight tool helps prospective students and families quickly select sessions, detect scheduling conflicts, and export their final plan to a calendar file.

![SCSU Open House screenshot](https://github.com/user-attachments/assets/5a3849d7-8c8f-41c4-82e8-a415f5cb2dde)

Live embed (used by SCSU Admissions in Slate):  
https://apply.southernct.edu/portal/SCSU_OpenHouse

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Files of Interest](#files-of-interest)
- [How to Use](#how-to-use)
- [Integration Notes (Slate)](#integration-notes-slate)
- [Accessibility & Responsiveness](#accessibility--responsiveness)
- [Customizing & Theme](#customizing--theme)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview

This project provides an easy-to-use itinerary builder tailored for university Open House events. Attendees can:

- Browse curated tracks or build a custom schedule from available sessions.
- Filter sessions by interest and session type.
- Add sessions to an itinerary with conflict detection.
- Reorder items (drag-and-drop) and persist the plan in the browser.
- Export the final schedule as an `.ics` calendar file.

The app was developed for embedding into SCSU's Slate portal for a seamless attendee experience.

---

## Key Features

- Curated Tracks — Load pre-built schedules (e.g., "Direct Nursing", "Living on Campus") in one click.
- Dynamic Filtering — Chip-based filters for Interests (STEM, Business, etc.) and Session Types (Tour, Presentation).
- Automatic Conflict Detection — Prevents adding overlapping sessions and warns users.
- Persistent Storage — Itinerary saves automatically via localStorage.
- Drag-and-Drop Reordering — Rearrange itinerary items with an intuitive interface.
- Calendar Export — Download an `.ics` file compatible with Google Calendar, Apple Calendar, Outlook.
- Responsive Design — Desktop two-column layout and mobile-friendly stacked layout.
- No external frameworks — Built with vanilla HTML, CSS, and modern JavaScript (ES6+).

---

## Tech Stack

- HTML5 — Semantic structure and accessibility landmarks.
- CSS3 — Styling, layout (Flexbox/Grid), responsive rules, and small UI animations.
- JavaScript (ES6+) — DOM manipulation, filtering logic, conflict checks, localStorage handling, and .ics generation.
- localStorage API — Client-side persistence.

No build system or external libraries are required — drop the files into a static host and open in a modern browser.

---

## Files of Interest

(These are typical names used in this project. Your repo may contain similar or matching files.)

- TEST_improved.html — A modernized scaffold and example layout for the app (open in a browser).
- index.html or existing HTML — Main app HTML shell used when embedding in Slate.
- styles.css — Styling and responsive layout.
- app.js — Core application logic: session rendering, filtering, itinerary management, .ics export.
- assets/ — Images and any static assets (e.g., uploaded screenshot(s)).

---

## How to Use

1. Open TEST_improved.html (or your app's main HTML file) in any modern web browser (Chrome, Edge, Firefox, Safari).
2. Browse curated tracks (left) or filter sessions using the chip UI.
3. Click "+ Add" on sessions to append them to "My Itinerary" (right).
   - The app will warn if the selected session conflicts with an existing item.
4. Reorder items by dragging them within "My Itinerary".
5. Use "Clear" to reset the itinerary, or let the app persist the plan automatically.
6. Click "Add to calendar" or "Export" to download an `.ics` file for import to calendar applications.

Example: open TEST_improved.html and click "Load" on a curated track to populate the itinerary automatically.

---

## Integration Notes (Slate)

- This project was built to be embedded within Slate (Admissions portal). For embedding:
  - Use an iframe in Slate pointing to the hosted HTML page.
  - Ensure the host uses HTTPS.
  - If using cross-origin embeds, confirm any necessary Content Security Policy (CSP) or frame-ancestors settings are configured on the host.
- Keep the app static (no server-side code required). Host on any static file host (GitHub Pages, Netlify, S3 + CloudFront, institutional web server).

---

## Accessibility & Responsiveness

- Semantic HTML elements and ARIA landmarks are used where appropriate.
- Interactive elements (buttons, chips) are keyboard accessible.
- Layout adapts from a 2-column desktop view to a stacked mobile layout using CSS Grid and media queries.
- If you need WCAG-level improvements (contrast, focus styles, announcements for screen readers), open an issue and we can prioritize enhancements.

---

## Customizing & Theming

- The UI uses CSS variables for quick theming (colors, radii, shadows).
- To adjust brand colors or spacing, update the variables near the top of `styles.css`.
- You can replace fonts by editing the HTML head and loading web fonts if desired.

---

## Contributing

Contributions, improvements, and bug fixes are welcome. To contribute:

1. Fork the repository.
2. Create a branch for your change (e.g., `feature/ui-refresh`).
3. Make changes and test locally.
4. Open a pull request with a clear description and screenshots if applicable.

If you want help splitting work into issues or a roadmap, create an issue or ask in the repository — happy to help draft tasks.

---

## License

This project is provided under the MIT License. See LICENSE file for details (or add one if missing).

---

## Contact

Developed for Southern Connecticut State University — Admissions.  
For questions about this repository or embedding into Slate, contact the repo owner: @Juxnn02

---e .ics file.
