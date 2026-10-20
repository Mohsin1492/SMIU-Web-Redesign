# SMIU University Website Redesign

Independent **Web Engineering assignment** project: a responsive, multi-page static website for **Sindh Madressatul Islam University (SMIU), Karachi, Pakistan**. This is **not** the official university site and is not affiliated with or endorsed by SMIU.

- **GitHub repository URL:** _[add your repo URL here]_
- **Live website URL:** _[add GitHub Pages or Netlify URL after deployment]_

## Purpose

Demonstrate HTML5 and CSS3 fundamentals—semantic structure, shared styling, responsive layout, and accessible navigation—using real university information where verified from public official sources.

## Technologies

- HTML5 only (10 pages)
- CSS3 only (`css/style.css`)
- No JavaScript, frameworks, CSS libraries, or build tools

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home — hero, introduction, featured areas, campus preview, news preview |
| `about.html` | History, Quaid-e-Azam connection, mission & vision |
| `admissions.html` | Application steps, eligibility overview, official portal links |
| `programs.html` | Undergraduate, graduate, and doctoral program summaries |
| `departments.html` | Department cards with official links |
| `faculty.html` | Verified leadership profiles; links for other faculty |
| `campus.html` | Location, heritage, library, labs, and facilities |
| `news.html` | News grid with clearly labeled sample entries |
| `gallery.html` | CSS Grid photo gallery with hover effect |
| `contact.html` | Verified contact details + non-functional demo form |

## Directory structure

```
SMIU-Redesign-Website/
├── index.html
├── about.html
├── admissions.html
├── programs.html
├── departments.html
├── faculty.html
├── campus.html
├── news.html
├── gallery.html
├── contact.html
├── css/
│   └── style.css
├── images/
└── README.md
```

## Navigation architecture

Every page includes the same header (`site-header`) and footer (`site-footer`):

- Sticky top bar with text wordmark linking to Home
- Primary nav: Home, About, Admissions, Programs, Departments, Faculty, Campus, News & Events, Gallery, Contact
- Current page uses class `active` and `aria-current="page"` on the matching link
- Footer quick links, disclaimer, and summary contact details

All internal links use relative paths to sibling `.html` files so the site works when opened locally or hosted at the domain root.

## Shared stylesheet

`css/style.css` provides:

- `:root` custom properties (colors, spacing, shadows)
- Global box-sizing reset and typography
- `.container` max-width layout
- Flexbox: header, nav, hero, buttons, footer
- CSS Grid: cards, gallery, profile grid
- Media queries: mobile (≤600px), tablet (601–900px), desktop (>900px)
- Focus-visible styles, link/card hover transitions
- Components: `.hero`, `.page-hero`, `.card-grid`, `.gallery-grid`, `.contact-form`, tables, notices

No inline or embedded CSS is used on pages.

## Accessibility & responsive design

- Skip link to `#main-content`
- Semantic landmarks: `header`, `nav`, `main`, `section`, `footer`
- Unique `<title>` and meta description per page
- Descriptive `alt` text on images
- Logical heading order (`h1` then `h2`/`h3`)
- Sufficient color contrast on text and buttons
- Nav wraps on small screens (no JS hamburger)

## Images

Campus photos load from **Wikimedia Commons** (CC BY-SA 4.0, Adnanchanna). See `images/README.md` for optional local copies. **Internet access is required** for images unless you download them into `images/`.


## Content disclaimer

Facts (address, phone, programs, mission text, etc.) were taken from [smiu.edu.pk](https://www.smiu.edu.pk/) and related public documents where noted. **Admission dates, fees, and news** must be confirmed on official channels before use. News cards marked “Sample content” are layout placeholders only.

## License note for photos

Third-party photos remain under their original licenses (Wikimedia Commons). Your HTML/CSS in this assignment is your own coursework unless your instructor specifies otherwise.