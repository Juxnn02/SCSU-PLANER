# SCSU Admissions Event Navigator & Itinerary Builder

A production-ready, single-page web application engineered for the Southern Connecticut State University Admissions department. This custom digital tool was developed specifically to optimize campus navigation and event coordination for over 2,000 Open House guests. 

By providing a responsive, frictionless interface for building personalized schedules, this application significantly reduces attendee confusion, detects scheduling conflicts in real-time, and bridges the gap between web planning and on-campus execution.

**Live Production Embed (Deployed via Slate CRM):** https://apply.southernct.edu/portal/SCSU_OpenHouse

---

## Table of Contents

- [Overview & Impact](#overview--impact)
- [Key Features](#key-features)
- [Front-End Architecture](#front-end-architecture)
- [Usage & User Flow](#usage--user-flow)
- [System Integration (Slate CRM)](#system-integration-slate-crm)
- [Accessibility & Responsiveness](#accessibility--responsiveness)
- [Contributing](#contributing)

---

## Overview & Impact

University Open House events involve hundreds of overlapping informational sessions, tours, and presentations, often leading to navigation fatigue for prospective students and their families. 

This tool provides a centralized, intuitive itinerary builder to solve that logistical bottleneck. Attendees can:
- Browse curated, department-specific tracks or build a custom schedule from scratch.
- Instantly filter sessions by academic interest and event type.
- Seamlessly reorder their day via drag-and-drop functionality.
- Export their finalized plan directly to their personal devices via an `.ics` calendar file.

The application was architected specifically to be embedded directly into SCSU's Slate portal, ensuring a unified and branded user experience without requiring additional account creation or logins.

---

## Key Features

- **Automated Conflict Detection:** Complex front-end logic prevents users from double-booking time slots and provides immediate UI warnings.
- **Client-Side Persistence:** Utilizes the `localStorage` API to automatically save the user's itinerary, allowing them to close the browser and return later without data loss.
- **Dynamic Filtering System:** A clean, chip-based UI allows users to instantly sort through hundreds of sessions based on specific tags (e.g., STEM, Business, Campus Tours).
- **Curated Track Loading:** One-click population of pre-built, optimized schedules (e.g., "Direct Nursing", "Living on Campus").
- **Drag-and-Drop Reordering:** An intuitive interface for users to manually adjust the flow of their day.
- **Cross-Platform Calendar Sync:** Generates and downloads a formatted `.ics` file compatible with Google Calendar, Apple Calendar, and Outlook.

---

## Front-End Architecture

Built with a focus on lightweight performance and maximum compatibility, requiring no external frameworks or build systems:
- **HTML5:** Semantic structure emphasizing accessibility and ARIA landmarks.
- **CSS3:** Custom theming, Flexbox/Grid layouts, and smooth UI animations optimized for both desktop and mobile viewports.
- **JavaScript (ES6+):** Handles all DOM manipulation, complex filtering algorithms, conflict validation, and dynamic `.ics` file generation.
- **Web Storage API:** Manages session state via `localStorage`.

---

## Usage & User Flow

1. **Access:** Open the application in any modern web browser.
2. **Discover:** Browse curated tracks (left column) or filter individual sessions using the dynamic chip UI.
3. **Build:** Click "+ Add" on desired sessions. The application evaluates the selection against the current itinerary to prevent time conflicts.
4. **Customize:** Rearrange itinerary items by dragging and dropping them into the preferred order.
5. **Deploy:** Click "Export" to download the `.ics` file and sync the itinerary with a personal mobile or desktop calendar.

---

## System Integration (Slate CRM)

This tool was engineered to operate seamlessly within higher-education CRM environments, specifically Slate.
- **Implementation:** Embedded via an `iframe` pointing to the secure, HTTPS-hosted HTML document.
- **Security:** Fully compliant with standard Content Security Policy (CSP) and `frame-ancestors` directives required for cross-origin embeds.
- **Hosting:** 100% static architecture requiring no server-side execution, allowing it to be hosted on any standard static file host (AWS S3, Netlify, GitHub Pages, or institutional servers).

---

## Accessibility & Responsiveness

- Built with a "mobile-first" approach, adapting seamlessly from a stacked mobile layout to a comprehensive two-column desktop view using CSS Grid and media queries.
- Incorporates semantic HTML elements and ARIA landmarks to ensure broad accessibility.
- Interactive elements (buttons, filter chips) are fully keyboard accessible.

---

## Contact

Engineered for Southern Connecticut State University — Admissions.  
For technical questions regarding the architecture or CRM embedding, contact the developer: [@Juxnn02](https://github.com/Juxnn02)

