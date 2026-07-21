# Design Stretch / DreamHaus Landing Pages

A lightweight static website for two related landing experiences:
- Design Stretch, a registration-focused event page
- DreamHaus, a minimal coming-soon studio page

The project is built as a simple front-end site with no build step, making it easy to edit, preview locally, and deploy to static hosting.

## Project Overview

This repository contains a polished static landing experience for DreamHaus and its Design Stretch event. The site is organized into separate pages and shared assets so the content stays easy to maintain.

## Technology Stack

- HTML5
- CSS3
- JavaScript (lightweight interaction support)
- Tailwind CSS via CDN
- Static hosting compatible (GitHub Pages, Netlify, Vercel, Firebase Hosting, etc.)

## Folder Structure

```text
.
├── index.html                  # Root redirect page
├── assets/
│   └── images/                # Shared image assets
├── css/
│   ├── main.css               # Shared styles for Design Stretch
│   └── dreamhaus.css          # Styles for the DreamHaus page
├── js/
│   └── main.js                # Scroll reveal animation behavior
├── pages/
│   ├── design-stretch/        # Design Stretch route page
│   ├── dreamhaus/             # DreamHaus coming-soon page
│   └── home/                  # Legacy/home fallback page
├── backup/                    # Original project backup files
└── README.md                  # Project documentation
```

## Local Setup

Because this is a static website, you can preview it locally without installing dependencies.

### Option 1: Python HTTP server

From the project root, run:

```bash
python -m http.server 8000
```

Then open:

```text
http://127.0.0.1:8000/
```

### Option 2: VS Code Live Server

If you use VS Code, you can also open the project and launch a Live Server instance from the editor.

## Deployment

This site is suitable for static hosting.

### GitHub Pages

1. Push the repository to GitHub.
2. Open the repository settings.
3. Go to Pages.
4. Select the main branch and the root folder as the deployment source.
5. Save and wait for the deployment to finish.

### Netlify

1. Create a new site from GitHub.
2. Select this repository.
3. Use the default build settings.
4. Deploy the site.

### Vercel

1. Import the repository into Vercel.
2. Keep the default settings.
3. Deploy.

## Notes

- The root page redirects to the DreamHaus experience.
- The Design Stretch content is available at the dedicated route under the pages folder.
- If you add new pages, keep shared CSS/JS in the existing folders to preserve consistency.
