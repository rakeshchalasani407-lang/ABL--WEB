# Three Static Websites: Portfolio, E-Commerce and Esports

Three single-file websites built with plain **HTML and CSS**. There is no JavaScript, no framework and no build step. Each file is self-contained and opens directly in a browser.

| # | Project | File | Theme |
|---|---------|------|-------|
| 1 | Personal Portfolio | `portfolio.html` | Purple, light |
| 2 | MyShop (E-Commerce) | `ecart_website.html` | Orange, light |
| 3 | ArenaX Esports | `gaming_website.html` | Dark with gold accent |

> Screenshots are in `Screenshots.pdf`. Detailed notes are in `Documentation.pdf`.

---

## Quick start

1. Download the three `.html` files into one folder.
2. Double-click any file to open it in Chrome, Edge, Firefox or Safari.

No installation or server is needed. For a live preview while editing, use the VS Code *Live Server* extension.

---

## 1. Portfolio (`portfolio.html`)

A one-page personal portfolio for a B.Tech CSE (AI & ML) student.

**Sections:** Home, Education, Skills, Projects, Hobbies, Achievements, Resume, Contact.

**Features**
- Sticky top navigation with smooth scrolling and a hover underline
- Hero section with a bouncing initials avatar and fade-in text
- Animated skill bars for HTML, CSS, C and Python
- Project and hobby cards that lift on hover
- Education and achievements as bordered list items that slide on hover
- Resume card with a download button
- Responsive layout (breakpoint at 600 px)

## 2. MyShop (`ecart_website.html`)

A storefront landing page styled like a typical Indian e-commerce site.

**Sections:** Top offer strip, sticky navbar with search box, category pills, "Mega Sale" banner, promo tiles, Featured Products grid, footer.

**Features**
- Six product cards, each with an emoji image, discount badge, star rating, price, old price and discount percentage
- "Add to Cart" and "Buy Now" buttons
- Pulsing call-to-action button on the banner
- Hover effects on the menu, category pills, promo tiles and product cards
- Prices in rupees (₹) and a free-delivery message above ₹499
- Responsive layout (breakpoint at 600 px)

## 3. ArenaX Esports (`gaming_website.html`)

A dark-themed esports tournament site with a fixed left sidebar.

**Sections:** Home (live match banner), Games, Schedule, Teams (standings table), Players, Leaderboard, News.

**Features**
- Fixed sidebar navigation that turns into a top bar on small screens (breakpoint at 800 px)
- Blinking "LIVE NOW" tag and a pulsing "VS" between the finalist teams
- Four game profile cards, a tournament schedule with date boxes and prize money, and two data tables (team standings and player leaderboard)
- Player cards with animated stat bars
- News layout with one featured story and three smaller ones

---

## Technologies

- **HTML5**: semantic sections, tables and anchor links
- **CSS3**: Flexbox, `position: sticky` and `fixed`, transitions, `@keyframes` animations, media queries
- Emoji are used in place of image files, so there are no external assets

## File structure

```
project/
├── portfolio.html
├── ecart_website.html
├── gaming_website.html
├── README.md
├── Screenshots.pdf
└── Documentation.pdf
```

## Customising

- **Portfolio:** change the name, education and contact details in the HTML. Colours are `#4b2fd6` (main purple) and `#ff6b5b` (button hover).
- **MyShop:** copy a `.card` block to add a product. The main colour is `#ff6b00`.
- **ArenaX:** edit the `.match` rows for the schedule and the `<tr>` rows for the tables. The accent colour is `#ffb400`.

## Known issues and suggested fixes

| File | Issue | Fix |
|------|-------|-----|
| `portfolio.html` | "Send Email" link has no `mailto:` prefix, so it will not open a mail app | Use `href="mailto:rakeshchalasani407@gmail.com"` |
| `portfolio.html` | "Download Resume" points to `resume.pdf`, which is not included | Add `resume.pdf` in the same folder |
| `portfolio.html` | Footer still reads "© 2026 Your Name" | Replace with your name |
| `portfolio.html` | GitHub and LinkedIn buttons go to the generic home pages | Link to your own profiles |
| `portfolio.html` | Achievement dates have square brackets, e.g. `[2023]` | Remove the brackets |
| `portfolio.html`, `ecart_website.html` | The sticky navigation is not offset for anchor jumps, so section headings can sit partly under it | Add `scroll-margin-top` to sections |
| `ecart_website.html` | Search box, Wishlist, Cart and category links are not functional (static page) | Add JavaScript or a backend |
| `gaming_website.html` | The Teams section is a table only; no per-team pages | Add team detail sections |

## License

Free to use for learning and personal projects.
