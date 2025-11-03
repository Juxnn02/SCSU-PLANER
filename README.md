#University Open House - Event Itinerary Builder

A responsive, single-page web application designed to help prospective students and families build a personalized schedule for a university open house. This tool allows users to load pre-built tracks, filter hundreds of sessions, and create a custom itinerary with automatic conflict detection.

This project was developed for Southern Connecticut State University (SCSU) - Admissions Department, to be embedded within their Slate portal, providing a seamless experience for registered attendees.
https://apply.southernct.edu/portal/SCSU_OpenHouse
<img width="1367" height="863" alt="image" src="https://github.com/user-attachments/assets/5a3849d7-8c8f-41c4-82e8-a415f5cb2dde" />


##🚀 Key Features

-Curated Tracks: Users can load pre-built schedules (e.g., "Direct Nursing," "Living on Campus") with a single click.

-Dynamic Filtering: A unified chip-based filter system allows users to find sessions by Interest (e.g., "STEM," "Business") and Session Type (e.g., "Tour," "Presentation").

-Automatic Time-Conflict Detection: The itinerary builder is smart! It checks for time overlaps and warns the user before adding a conflicting session.

-Persistent Itinerary: The user's custom plan is automatically saved to their browser's localStorage, allowing them to close the page and return later without losing their work.

-Drag-and-Drop Reordering: Users can easily re-order sessions in their itinerary.

-Calendar Export: Users can export their final itinerary as a .ics file to add directly to their phone or desktop calendar (i.e., Google Calendar, Apple Calendar).

-Fully Responsive: The layout seamlessly transitions from a two-column desktop view to a stacked, single-column layout for mobile devices.

##💻 Tech Stack

-This project is built with vanilla HTML, CSS, and JavaScript (ES6+), with no external libraries or frameworks.

-HTML5: For semantic structure.

-CSS3: For all styling, animations, and responsive design (using Flexbox, Grid, and media queries).

-JavaScript (ES6+): For all DOM manipulation, event handling, data filtering, and application logic.

-localStorage API: For client-side persistence of the user's itinerary

##🔧 How to Use

1. Open TEST_improved.html in any modern web browser.

2. Load a Track: Click "Load" on a curated track to populate your itinerary instantly.

###Build Your Own:

3. Click on filter chips (e.g., "STEM," "Tour") to see matching sessions.

4. Click the "+ Add" button on any session.

###Manage Your Itinerary:

Drag sessions in the "My Itinerary" panel to re-order them.

Click "Remove" to delete a session.

Click "Clear" to start over.

Save & Export:

Your plan saves automatically to the browser.

Click "Add to calendar" to download the .ics file.
