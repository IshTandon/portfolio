# Ishaan Tandon — AI Product Manager Portfolio

A minimal, editorial portfolio site built to showcase AI/GenAI product management work, case studies, and shipped products.

**Live:** Deploy to any static host (Netlify, Vercel, GitHub Pages, Cloudflare Pages).

## Features

- **Single-page static site** — zero dependencies, no build step, just `index.html`
- **Light / Dark mode** with system preference detection and manual toggle (persisted via `localStorage`)
- **Responsive** — optimized layouts for desktop, tablet, and mobile with a hamburger menu on small screens
- **Tabbed work experience** — company logos, timelines, and quantified bullet points
- **AI Builds section** — HealthIsh and MindTheGap with structured Problem → Approach → Outcome format
- **Case studies** — featured case study with horizontal scroll grid and detailed KPI breakdowns
- **"What I'm looking for" section** — cards highlighting role preferences
- **"How I think" philosophy cards** — product management principles
- **"How I work" process strip** — Discover → Define → Build → Measure
- **Writing & Thinking section** — grounded to actual work and shipped products
- **Social proof strip** — quantified career highlights
- **Animated text reveals** — word-by-word scroll-triggered animations via IntersectionObserver
- **Typewriter hero tagline** — cycling phrases in the hero section
- **Marquee ticker** — infinite-scroll metrics strip
- **Lenis smooth scroll** — buttery smooth scrolling experience
- **Subtle grain texture** — SVG noise overlay for editorial depth
- **Preloader** — branded page entrance animation
- **Magnetic buttons** — hover pull effect on CTAs
- **Card tilt** — 3D perspective on hover for build cards
- **Floating Resume FAB** — always-accessible resume download
- **Back-to-top button** — appears on scroll
- **Scroll progress indicator** — top bar showing read progress
- **Keyboard-accessible tabs** — arrow key navigation for work experience
- **Skip-to-content link** — accessibility first
- **Reduced motion support** — respects `prefers-reduced-motion`
- **Open Graph & Twitter Card meta** — optimized social sharing with custom OG image
- **JSON-LD structured data** — SEO-ready Person schema
- **Print stylesheet** — clean print layout with UI chrome hidden

## Project Structure

```
├── index.html                  # Entire site (HTML + CSS + JS)
├── portrait.webp               # Hero portrait photo
├── og-card.png                 # Open Graph social sharing image
├── Ishaan_Tandon_Resume.pdf    # Downloadable resume
├── logo-naukri.png             # Company logos
├── logo-et.webp
├── logo-mmt.png
├── logo-mdi-converted.png
├── logo-amazon.png
├── logo-wipro.png
├── logo-thapar.png
├── .gitignore
└── README.md
```

## Running Locally

No build step needed. Serve the directory with any static server:

```bash
# Python
python3 -m http.server 8000

# Node.js
npx serve .

# Or just open index.html in a browser
```

Then visit `http://localhost:8000`.

## Deployment

### GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch** → `main` → `/ (root)`
4. Your site will be live at `https://<username>.github.io/<repo-name>/`

### Netlify / Vercel

1. Connect the repo
2. No build command needed — publish directory is `/`
3. Auto-deploys on every push

## Customization

All content, styling, and behavior live in `index.html`:

- **Colors:** Edit CSS variables in the `:root` block at the top of `<style>`
- **Fonts:** Currently uses Playfair Display (headings), Inter (body), JetBrains Mono (accents) via Google Fonts
- **Content:** Directly edit the HTML sections — work experience, case studies, builds, skills, contact info
- **Dark mode colors:** Override variables under `[data-theme="dark"]`
- **Resume:** Replace `Ishaan_Tandon_Resume.pdf` with your updated file

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | Semantic HTML5 |
| Styling | Vanilla CSS (custom properties, Grid, Flexbox) |
| Interactivity | Vanilla JavaScript (no frameworks) |
| Smooth scroll | [Lenis](https://github.com/darkroomengineering/lenis) (CDN) |
| Fonts | Google Fonts (Playfair Display, Inter, JetBrains Mono) |
| Hosting | Any static host |

## License

This portfolio is personal work. Feel free to use the structure and techniques as inspiration for your own portfolio.

---

Built by Ishaan Tandon
