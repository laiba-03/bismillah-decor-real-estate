# Bismillah Decor & Real Estate

A responsive, single-page business website for **Bismillah Decor & Real Estate**, a Maharashtra-based company that offers interior design and real estate services with equal importance.

**Tagline:** *Design Your Space. Find Your Place.*

## Features

- Hero section, service sections and About section for both interior design and real estate
- Property search (Buy/Rent, type, location, budget, BHK, status, area) with working filters, detail pop-ups and WhatsApp inquiry buttons
- Completed-projects gallery sorted by room (Living Room, Bedroom, Kitchen, Bathroom, Commercial) and by project, with a photo viewer
- Design Inspiration gallery and 3D Visualizations (AI-generated concept images, each labelled as AI)
- Interior packages, furniture and materials close-ups, Instagram section
- Property visit booking, sell-your-property and contact forms (Netlify Forms)
- Responsive layout with mobile menu, light and dark mode (follows the device setting), SEO title and description

## Technologies

- HTML5, CSS3 (custom properties, grid, flexbox), vanilla JavaScript (no framework, no build step)
- Google Fonts: Playfair Display and Inter
- Netlify Forms for form submissions when hosted on Netlify

There is no React, npm or build configuration. The site is static, so no installation is needed.

## Project structure

```
.
├── index.html            Page structure and content
├── css/
│   └── style.css         All styling and the colour palette
├── js/
│   └── script.js         Settings, property data, filters, galleries, forms
├── images/
│   ├── projects/         Real photos of completed projects
│   ├── inspiration/      AI-generated design inspiration images
│   ├── 3d/               AI-generated 3D visualization concepts
│   └── properties/       AI-generated demo property images
├── .gitignore
└── README.md
```

## Run locally

1. Download or clone the project.
2. Double-click `index.html` to open it in a browser.

Or serve it with a local server (recommended):

```bash
python -m http.server 8000
```

Then open http://localhost:8000. The Google Fonts need an internet connection. The forms only submit when the site is hosted on Netlify; locally they show a "could not send" message.

## Customise

- **Contact details:** edit the `CFG` block at the top of `js/script.js` (phone numbers, email, WhatsApp number with country code, Instagram ID).
- **Properties:** edit the `P` list in `js/script.js`. Prices are in lakhs (100 = 1 crore). The listings and images shipped here are demo examples.
- **Project photos:** add the image to `images/projects/` and add an entry to the `IMG` list in `js/script.js` (file path, room tags, project number).
- **Replace a photo:** save the new file with the same name in the same folder. Keep files under about 300 KB.
- **Colours:** edit the variables at the top of `css/style.css`.

## Deploy

- **Netlify (recommended):** drag the project folder onto https://app.netlify.com/drop. The three forms (`contact`, `visit`, `sell-property`) then appear under Forms in your Netlify dashboard, and you can add an email notification there.
- **GitHub Pages:** works for everything except the forms, which need Netlify.

## Images and labelling

Photos in `images/projects/` are real completed work. Images in `inspiration`, `3d` and `properties` are AI-generated concepts, and listings are demo examples with no real availability or prices. The website labels them as such. Keep those labels unless you replace them with real photos.

## Note

Contact details in `js/script.js` are the real business details and become public if the repository is public.
