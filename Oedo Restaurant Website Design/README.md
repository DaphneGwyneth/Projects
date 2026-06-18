# Oedo Japanese Restaurant — Website

A modern, single-page website for **Oedo Japanese Restaurant**, a Japanese dining spot in Banawe, Quezon City, Philippines with 12+ years in business and a 4.5-star Google rating across 1,295 reviews.

The site is built to showcase the restaurant's menu, story, and customer reviews, and to drive reservations through Google Maps and Messenger — no backend required.

## Live Demo



https://github.com/user-attachments/assets/0955ccb5-36bb-4c75-85a1-db407a1c96a2



## Features

- **Cinematic hero section** with a clear call-to-action to reserve via Messenger or explore the menu
- **Trust bar** highlighting rating, review count, and years in business
- **About section** telling the restaurant's story alongside a photo
- **"The Oedo Difference"** — a 3-card feature section covering portions, authenticity, and service
- **Scrollable / arrow-navigable menu carousel** listing signature dishes (Oedo Maki, Sukiyaki, Teppanyaki, Chirashi, and more)
- **Auto-looping review slider** pulling real customer quotes from Google Reviews
- **Location section** with a direct link to Google Maps
- **Reservation CTAs** throughout the page linking to Google's reservation flow and Facebook Messenger
- Fully responsive layout using Google Fonts (`Playfair Display` + `Inter`)

## Tech Stack

- **HTML5** — semantic single-page structure (`index.html`)
- **CSS3** — custom styling (`style.css`)
- **Vanilla JavaScript** — menu carousel and review slider interactivity (`script.js`)
- **Google Fonts** — Playfair Display (headings) and Inter (body text)
- No frameworks, build tools, or dependencies — runs directly in the browser

## Project Structure

```
oedo-website/
├── index.html      # Main page markup and content
├── style.css        # All styling (layout, colors, typography, animations)
├── script.js         # Menu carousel + review slider behavior
└── README.md
```

## Getting Started

This is a static site with no build step.

### Run locally

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
2. Open `index.html` directly in your browser, or serve it locally:
   ```bash
   npx serve .
   ```
   (or use the VS Code "Live Server" extension, Python's `http.server`, etc.)

### Deploy

Since this is a static site, it can be deployed for free on any of the following:

- **GitHub Pages** — push to a `gh-pages` branch or enable Pages on `main`
- **Netlify** — drag-and-drop the project folder or connect the repo
- **Vercel** — import the repo as a static project

## Content & Sections Overview

| Section | Purpose |
|---|---|
| Nav | Logo + links to Menu, About, Find Us, and a "Reserve via Google" button |
| Hero | Headline, subheadline, and primary CTAs (Messenger reservation, menu link) |
| Trust Bar | Quick credibility signals (rating, reviews, years open) |
| About | Restaurant story and photo |
| The Oedo Difference | Three value propositions: portions, authenticity, service |
| Menu | Carousel of signature dishes |
| Reviews | Auto-scrolling slider of real customer testimonials |
| Find Us | Location details and Google Maps link |
| CTA | Final reservation prompt before the footer |
| Footer | Closing tagline |

## Customization Notes

- **Reservation links**: The "Reserve via Google" and "Reserve via Messenger" buttons currently point to the restaurant's live Google Maps booking URL and Facebook page — update these if the business listing changes.
- **Images**: Several images are currently hotlinked from Facebook's CDN (`scontent-*.fbcdn.net`). These URLs can expire or break; it's recommended to download and self-host these images (e.g. in an `/assets` or `/images` folder) for long-term reliability.
- **Menu items**: Dishes are listed as plain text in the `#menu` section — update the `.item` divs in `index.html` to add, remove, or reprice dishes.
- **Reviews**: Review cards are duplicated in the markup to create a seamless looping effect in the slider; if you add or remove reviews, keep the loop duplication in mind.

## Roadmap / Possible Improvements

- [ ] Self-host all images instead of relying on external CDN links
- [ ] Add an actual embedded Google Map (iframe) in the "Find Us" section
- [ ] Add menu item prices and photos
- [ ] Add a contact form or click-to-call button
- [ ] Add SEO meta tags (description, Open Graph, favicon)
- [ ] Add accessibility improvements (alt text audit, keyboard navigation for carousel/slider)

## Acknowledgements

- Customer review excerpts sourced from Oedo Japanese Restaurant's Google Business listing
- Fonts via [Google Fonts](https://fonts.google.com/)
