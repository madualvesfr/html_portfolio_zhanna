# Zhanna Bielash — Portfolio

> *"Notes on a life lived awake."*

A personal portfolio site for **Zhanna Bielash**, a web developer from Netishyn, Ukraine. Built as a quiet, editorial magazine — warm paper, classical serifs, a single deep accent. No frameworks, no build step.

## Design direction

This isn't a generic "developer portfolio." It's designed as a **small printed journal**: cream paper, Playfair Display for headlines, Source Serif 4 for reading, JetBrains Mono for labels. Subtle paper grain, double-rule dividers, drop caps, pull quotes, and numbered entries — the visual language of a magazine, not a dashboard.

- **Palette**: Cream `#f4ede0` paper on near-black ink, with a deep sepia-red `#8b2c0f` accent used only sparingly.
- **Type**: Playfair Display (display) + Source Serif 4 (body) + JetBrains Mono (labels).
- **Motion**: Restrained — only scroll fade-ins. No glassmorphism, no gradients, no 3D tilt.
- **Dark mode**: A warm "lamp-lit" version, not the usual blue-black.

## Structure

```
html_portfolio/
├── index.html              # Masthead + two "Selected Works"
├── public/
│   ├── about.html          # Editorial portrait + drop-cap lede + pull quote
│   ├── contact.html        # Correspondence card
│   ├── movie_ranking.html  # Essay with numbered film entries
│   └── birthday_invite.html
├── assets/
│   ├── css/style.css       # Design system
│   ├── js/main.js          # Theme toggle + IntersectionObserver reveal
│   └── images/
└── README.md
```

## Run locally

```bash
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000).

## Editorial elements available

When writing new pages, the stylesheet provides:

| Class | Purpose |
|---|---|
| `.page-kicker` | Small uppercase tag above the headline (*"Essay · 01 · On Cinema"*) |
| `.page-deck` | Italic sub-headline / standfirst |
| `.lede` | First paragraph — gets an automatic drop cap |
| `.pullquote` | Large italic quote with a side rule |
| `.movie-item` | Auto-numbered entry (01, 02, 03…) with a ghosted numeral |
| `.hero-meta` | Issue / date / location line under the masthead |
| `.section-title[data-num]` | Section header with a right-aligned italic label |

## Credits

Built by **Madu** for **Zhanna Bielash**. Content © Zhanna. Design inspired by the typographic traditions of independent print magazines.
