# The UX Review Blog

A responsive, neo-brutalist blog landing page built with **pure HTML and CSS**. No JavaScript, no frameworks, no libraries.

**Live demo:** https://taha20353.github.io/ux-review-blog/

![Preview](./images/preview.png)

## Features

- Neo-brutalist design: thick black borders, hard offset shadows, bold colors
- Fully responsive layout (desktop, tablet, mobile)
- Mobile slide-in menu built with CSS only (`:target`)
- Sticky sidebar with trending posts and categories
- Hover animations: lifting cards, shifting buttons, moving shadows
- Smooth scrolling between sections
- Zero dependencies in the `<head>`

## Sections

| Section | Description |
|---|---|
| Navbar | Fixed floating navbar with a subscribe button |
| Hero | Headline, intro text, call-to-action buttons and featured image |
| Latest Articles | Article cards with a trending and categories sidebar |
| Authors | Three author cards with social links |
| Community | Perks list and testimonials |
| Footer | Categories, newsletter form and legal links |

## Tech Stack

- **HTML5**: semantic structure
- **CSS3**: Flexbox, Grid, custom properties, media queries, `:target`, `position: sticky`
- **Font**: [Exo](https://fonts.google.com/specimen/Exo) via Google Fonts (`@import` in the stylesheet)

## Project Structure

```
ux-review/
├── index.html
├── css/
│   └── style.css
├── images/
│   ├── hero-img.png
│   ├── user-engagement.jpg
│   ├── guide-to-typography.avif
│   ├── anti-instagram.jpg
│   ├── avatar-2.jpg
│   ├── avatar-4.avif
│   ├── avatar-5.jpg
│   ├── avatar-6.avif
│   └── icons/
│       └── *.png
└── README.md
```

## Getting Started

Clone the repository:

```bash
git clone https://github.com/taha20353/ux-review-blog.git
cd ux-review-blog
```

Open `index.html` in your browser, or serve it locally:

```bash
# Python
python -m http.server 5500

# or VS Code: install the "Live Server" extension and click "Go Live"
```

Then visit `http://localhost:5500`.

## Responsive Breakpoints

| Breakpoint | Changes |
|---|---|
| `max-width: 1279px` | Nav links collapse into the mobile menu |
| `max-width: 1024px` | Hero, articles and community grids become a single column; authors become 2 columns |
| `max-width: 768px` | Smaller headings, stacked article cards, single-column authors and footer |

## How the Mobile Menu Works

The menu uses no JavaScript. The toggle is a link to `#mobile-menu`, and the CSS `:target` selector reveals the overlay when the URL hash matches. The close button links to `#`, which removes the target and hides the menu.

```css
.mobile-menu { opacity: 0; visibility: hidden; }
.mobile-menu:target { opacity: 1; visibility: visible; }
```

## Deployment

Hosted on GitHub Pages:

1. Go to **Settings → Pages**
2. Set the source to branch `main`, folder `/ (root)`
3. Save and wait about a minute

## Credits

- Layout and design inspired by [The UX Review](https://the-ux-review-blog.vercel.app/)
- Icons: Font Awesome Free (exported as PNG)
- Font: Exo by Natanael Gama

## Author

**Mostafa Sultan**

- GitHub: [@taha20353](https://github.com/taha20353)
- LinkedIn: [mostafa-sultan](https://www.linkedin.com/in/mostafa-sultan-60a147262/)

## License

This project is for learning and portfolio purposes.
