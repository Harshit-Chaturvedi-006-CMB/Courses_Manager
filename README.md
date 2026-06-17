## Course Manager — Developer Guide



Files:
- [courses.html](courses.html) — single static HTML file containing the UI and any embedded styles/scripts.
- [README.md](README.md) — this developer guide.


# Course Manager

A small static project that lists and displays course information in a single HTML file. This document is formatted for a GitHub repository: it explains the purpose, how to run and develop the project, and where to start when contributing.

## Table of Contents

- [About](#about)
- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage & Examples](#usage--examples)
- [Development](#development)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
A small static project that lists and displays course information in a single HTML file.

This README is written for end users who will view and use the site (not for developers). It explains how to open the site, read course entries, and solve common problems.

## Quick Start

1. Open the project folder and double-click `courses.html` to open it in your browser.
2. (Optional) Serve the folder and open it from a local server for the best results:

```powershell
python -m http.server 8000
# then visit http://localhost:8000/courses.html
```

## What you will see

- A list of course items. Each entry shows the course title, a short description, and any metadata (duration, level).
- Links or buttons for more details may be present depending on the file contents.

## How to read a course entry

- Title: the course name in bold or large type.
- Description: one or two lines describing the course content and prerequisites.
- Metadata: look for duration, level (Beginner/Intermediate/Advanced), and course ID.
- Actions: `Details`, `Enroll`, or similar links may be shown — click to navigate if provided.

## Common tasks

- Searching: if a search box is present, type keywords and press Enter to filter visible courses.
- Filtering: if filter buttons or tags are visible, click them to narrow results.
- Details: click a course's `Details` link to see more info (if provided).

## Troubleshooting

- Page is blank or layout looks wrong:
	- Try refreshing the page (F5).
	- Open the file with a different browser.
- Images or links not loading:
	- If running directly from the file system some resources may be blocked; run a simple local server (see Quick Start).
- Search or interactive features don't work:
	- Those features rely on JavaScript. Ensure JS is enabled in your browser.

## Accessibility & Tips

- Use browser zoom (Ctrl+Plus / Ctrl+Minus) to change font size.
- Use the browser's find feature (Ctrl+F) to locate course titles or keywords on the page.

## Frequently Asked Questions

- Q: Can I use this on mobile?  
	A: Yes — the page is static and should work on mobile browsers, though layout depends on how `courses.html` was authored.

- Q: How do I get updates?  
	A: If this project is hosted on GitHub, watch or star the repository to get notifications of releases or changes.

## Contact / Help

If you need help or want improvements (search, mobile layout, enrollment links), tell the repository owner or open an issue on the project's GitHub page.

Would you like me to add a short screenshot section or an example of a course entry rendered on-screen? Reply and I'll update `README.md` accordingly.
		container.innerHTML = '';

		courses.forEach(c => {

			const el = document.createElement('article');

			el.className = 'course';
