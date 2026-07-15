# Academic Homepage

A clean, single-page academic personal website. No frameworks, no Jekyll, no JavaScript — just one HTML file and your content.

## What's Inside

- Responsive header with avatar, name, affiliation, bio, and links
- News section (date + event)
- Publication cards with venue badges, author highlighting, paper links
- Professional service section
- Automatic dark mode (via CSS `prefers-color-scheme`)
- Mobile-friendly layout

## How to Use

### 1. Replace your info
Open `index.html` and replace every placeholder:
- `Your Name` / `中文名` — your name
- `Your University`, `Prof. Advisor` — your affiliation
- `your@email.com` — your email
- Publication titles, authors, venues, links
- Google Scholar / GitHub / Twitter URLs
- News items

### 2. Add your avatar
Put a square photo named `avatar.jpg` in the `assets/` folder. Or remove the `<img>` tag if you don't want a photo.

### 3. Deploy

**Option A — GitHub Pages (free, recommended):**
1. Create a repository named `yourusername.github.io`
2. Push all files to the `main` branch
3. Go to Settings → Pages → enable
4. Your site goes live at `https://yourusername.github.io`

**Option B — Custom domain:**
1. Add a `CNAME` file with your domain
2. Configure your DNS to point to GitHub Pages

**Option C — Any static host:**
Upload `index.html` + `assets/` to Netlify, Vercel, or any web server.

### 4. Customize colors
Edit the CSS variables at the top of index.html:

```css
:root {
  --link: #2b6cb0;      /* link color */
  --badge: #ebf4ff;     /* conference badge background */
  ...
}
```

### 5. Add more papers
Copy the `<div class="pub">...</div>` block and fill in your paper details.

## Structure

```
academic-homepage/
├── index.html          ← the whole site
├── assets/
│   └── avatar.jpg      ← your photo
└── README.md           ← this file
```

## Browser Support
All modern browsers (Chrome, Safari, Firefox, Edge). No polyfills needed.
