# Belle & Carrie — Rehabilitation Yoga

![HTML](https://img.shields.io/badge/HTML-Frontend-orange)
![CSS](https://img.shields.io/badge/CSS-Frontend-brightgreen)

A responsive, multi-page website for **Belle & Carrie Rehabilitation Yoga**, a welcoming studio focused on supportive movement, mobility, balance, strength, and restorative practice. The site is built with plain HTML and CSS and can be viewed locally or hosted as a static website.

## Pages

- **Home** (`index.html`) — Studio introduction and links to classes and studio information.
- **About** (`about.html`) — The studio's approach and instructor profiles.
- **Classes** (`classes.html`) — Class descriptions and a sample weekly schedule.
- **Blog** (`blog.html`) — Studio journal and mindful-movement articles.
- **Contact** (`contact.html`) — Contact details and a message form.

All pages share the stylesheet (`style.css`) and use images stored in `images/`.

## Features

- Responsive page layouts for desktop and smaller screens.
- Shared navigation and footer across the site.
- Semantic HTML, descriptive image alternative text, and labeled form fields.
- CSS-only styling with a forest-green, cream, and leaf-green palette.
- Reduced-motion preference support.
- No framework, package manager, build process, or JavaScript dependency is required.

## Getting started

### View locally

1. Clone the repository:

   ```bash
   git clone https://github.com/Honbia/yoga-website.git
   cd yoga-website
   ```

2. Open `index.html` in a browser.

For a local HTTP server, you can also run Python from the repository directory:

```bash
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Project structure

```text
yoga-website/
├── index.html           # Home page
├── about.html           # Studio and instructor information
├── classes.html         # Class descriptions and weekly schedule
├── blog.html            # Studio journal
├── contact.html         # Contact information and message form
├── style.css            # Shared responsive styles
└── images/              # Photography and graphic assets
```

The `images/` directory also contains supporting assets, including instructor and yoga photographs, icons, and a `mobile/` subdirectory. Keep referenced image paths and filenames in sync with the HTML when replacing or adding assets.

## Customization

- **Content and navigation:** Edit the relevant HTML page. Navigation links are ordinary links between the page files.
- **Colors and typography:** Update the CSS custom properties near the top of `style.css` (for example, `--forest`, `--paper`, and `--serif`).
- **Layout and breakpoints:** The responsive rules are in the media queries near the end of `style.css`.
- **Images:** Replace files in `images/` or update the corresponding `src` values in the HTML. Keep useful `alt` text for meaningful images.
- **Studio details:** Update the sample address, phone number, email, instructor names, class schedule, and hours before using the site for a real studio.

## Contact form note

The form in `contact.html` uses a `mailto:` action. This relies on the visitor having a configured email application and is not a server-side form submission service. For a production website, replace it with a suitable form backend or hosted form provider and verify the destination email address.

## Deployment

This is a static site: publish the HTML files, `style.css`, and the `images/` directory together on any static web host. GitHub Pages can also serve the site from the repository's configured publishing source; configure Pages in the repository settings and use `index.html` as the entry point. No compilation or build step is needed.

## Contributing

For a content or design change, update the relevant HTML/CSS and check the affected pages at both desktop and mobile widths. Confirm that local links and image paths work, and that form labels and image alternative text remain descriptive.

## License

No license is currently specified in this repository. Unless a license is added, reuse and redistribution of the code and assets are not granted by default. Check the rights for image assets before reusing them.
