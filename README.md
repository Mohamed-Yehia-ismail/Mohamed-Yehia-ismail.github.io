# Mohamed Yehia · Portfolio

Personal website of Mohamed Yehia, software engineer and web developer, in English and Arabic.

**Live demo:** https://mohamed-yehia-ismail.github.io/

## Features

- Code editor in the hero that types out the intro with syntax highlighting, with a Run button
- Projects grid with generated previews and a case study for each project
- Command palette (Ctrl / Cmd + K) with fuzzy search
- Interactive terminal: help, projects, open <n>, skills, contact, history and tab completion
- Full Arabic / English switch, light and dark themes
- Contact form that prepares a message to send by email or LinkedIn

## Engineering notes

- Links and contact details live in `CONFIG` at the top of the script.
- Live demo links point to GitHub Pages under the same account.
- Schema.org `Person` JSON-LD.

## Performance and scale

The site is a single static file: no server, no database, no build step. Every visitor's browser does its own work, so traffic only reaches the CDN that serves the file (GitHub Pages), which is built for very high traffic. Orders and bookings go straight to WhatsApp, so there is no backend that can fail under load. Fonts load with `display=swap`, and state is kept in `localStorage` with safe fallbacks.

## Tech

HTML5, CSS3 (custom properties, grid, logical properties for RTL), vanilla JavaScript, inline SVG. No frameworks. Fonts from Google Fonts.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Author

Mohamed Yehia · [GitHub](https://github.com/Mohamed-Yehia-ismail) · [LinkedIn](https://www.linkedin.com/in/mohamed-yehia-ismail)
