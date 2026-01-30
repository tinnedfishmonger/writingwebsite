# Website Redesign Brief: audreymorganlee.com

## Overview

Redesign of Audrey Lee's personal writing website (audreymorganlee.com) to follow the visual and structural conventions of the Berkshire Hathaway website (berkshirehathaway.com). The goal is a radically minimal, text-first, no-frills design that prioritizes content and links over visual ornamentation.

---

## Design Principles (Derived from Berkshire Hathaway)

1. **Plain white background** with black text — no gradients, hero images, or color accents
2. **Default browser serif font** (e.g., Times New Roman) — no custom web fonts
3. **No CSS framework, no JavaScript UI** — static HTML with minimal inline or embedded CSS
4. **Centered, narrow content column** — text and links are centered on the page
5. **Horizontal rules** (or asterisk/character borders) to separate content sections
6. **Bulleted or plaintext link lists** — no buttons, cards, or styled navigation bars
7. **No header/footer chrome** — no sticky nav, hamburger menu, or footer widgets
8. **Copyright notice** at the bottom of each page

---

## Site Map

| Page                  | URL Path         |
|-----------------------|------------------|
| Homepage              | `/`              |
| Books                 | `/books`         |
| Publications          | `/publications/` |
| Interviews and Press  | `/media/`        |

---

## Page-by-Page Specifications

### Homepage (`/`)

The homepage mirrors the structure of berkshirehathaway.com's single-page layout.

**Header / Heading Area:**

Centered at the top of the page:

```
AUDREY LEE
Author of Utter Goodness
```

- "AUDREY LEE" in a large, bold serif font (analogous to the "BERKSHIRE HATHAWAY INC." heading)
- "Author of Utter Goodness" directly below in regular-weight serif, smaller size (analogous to the Berkshire Hathaway Omaha address block)

**Main Navigation Links:**

A centered list of links, styled as a bulleted list or as simple plaintext links separated by line breaks — matching Berkshire Hathaway's link list format:

- **Books** — links to `/books`
- **Publications** — links to `/publications/`
- **Interviews and Press** — links to `/media/`

**Social Links:**

A separate section (below a horizontal rule or asterisk divider) with plaintext links:

- Substack
- X / Twitter
- Instagram
- Goodreads

These should be rendered as simple underlined hyperlinks, not icons or buttons.

**Contact / Footer Text:**

Below another horizontal rule divider, include the following text centered on the page:

> If you have any comments, please contact me at audreymorganlee@gmail.com

("audreymorganlee@gmail.com" should be a clickable `mailto:` link.)

**Copyright:**

At the very bottom of the page:

```
Copyright © 2025 Audrey Lee
```

---

### Books Page (`/books`)

**Header:**

Centered page title in bold serif:

```
BOOKS
```

With a link back to the homepage ("Return to Home Page" or similar, matching Berkshire Hathaway's back-link convention).

**Content:**

A section for each book. Based on the current site, the primary book is:

- **Utter Goodness** — forthcoming short story collection, published by Farthest Heaven (2026)

Display as plaintext with the title in bold or as a subheading. Include a brief description or publication details as a short paragraph beneath the title.

As more books are added, each should appear as a new plaintext block separated by a horizontal rule.

**Footer:**

Same copyright line as homepage.

---

### Publications Page (`/publications/`)

**Header:**

Centered page title in bold serif:

```
PUBLICATIONS
```

With a link back to the homepage.

**Content:**

Organized by genre with simple subheadings and bulleted lists of linked titles. Each entry is a hyperlink to the publication venue.

**Fiction:**
- "New Year's Eve" — Post Pop Lit, 2026
- "Utter Goodness" — Apocalypse Confidential, 2025
- "Engineer" — Hobart, 2025
- "The Ostrich Economy" — X-R-A-Y, 2024
- "Harvesting Bunnies" — Necessary Fiction, 2023

**Poetry:**
- "Quality of Life" — Spectra Poets, 2026
- "Saucers" — Poet's Row, 2025
- "Floss and Taking the Train to Atlantic City..." — Wax Nine, 2022

**Non-Fiction:**
- "An Absurdly American Life: On the Passing of David Lynch" — Athwart, 2025

Each title should link to the original publication. Venue names and years appear as plaintext after the link.

**Footer:**

Same copyright line as homepage.

---

### Interviews and Press Page (`/media/`)

**Header:**

Centered page title in bold serif:

```
INTERVIEWS AND PRESS
```

With a link back to the homepage.

**Content:**

A bulleted or line-separated list of interviews and media appearances, each as a hyperlink:

- Heavy Bored episode #114: "Feminine Goodness" — Patreon / Substack
- Tales From the Mall ep. #175 — Patreon
- Melee: "Method and Madness" — Substack
- Victim Radio — Patreon
- BBC4's "The Poetry Detective" (hosted by Vanessa Kisuule) — BBC

Each entry title should be a hyperlink to the relevant platform. Platform names appear as plaintext after the link.

**Footer:**

Same copyright line as homepage.

---

## Shared Style Rules (All Pages)

| Property            | Value                                              |
|---------------------|----------------------------------------------------|
| Background          | `#FFFFFF` (white)                                  |
| Text color          | `#000000` (black)                                  |
| Font family         | `Times New Roman, Times, serif` (browser default)  |
| Link color          | Browser default blue (`#0000EE` unvisited, `#551A8B` visited) |
| Link style          | Underlined (browser default)                       |
| Text alignment      | Centered                                           |
| Max content width   | ~600–800px, centered on page                       |
| Section dividers    | `<hr>` or a row of asterisks (`* * * * *`)         |
| Page title element  | Bold, uppercase, larger font size                  |
| Navigation          | No navbar — plaintext link back to homepage on subpages |
| Images              | None (text only, matching Berkshire Hathaway's approach) |
| JavaScript          | None required                                      |
| Responsive behavior | Naturally responsive due to minimal styling         |

---

## Technical Notes

- The site can be implemented as four static HTML files with a single shared CSS block (embedded or in one small stylesheet).
- No build tools, CMS, or JavaScript framework required.
- The current WordPress site content (bio details, publication links, media links) should be carried over into the new static pages.
- Hosting can remain on any platform that serves static files.

---

## Reference Comparison

| Berkshire Hathaway Element           | Audrey Lee Equivalent                          |
|--------------------------------------|------------------------------------------------|
| "BERKSHIRE HATHAWAY INC."            | "AUDREY LEE"                                   |
| Omaha address block                  | "Author of Utter Goodness"                     |
| Bulleted link list (reports, filings)| Bulleted link list (Books, Publications, Media) |
| GEICO ad section                     | Social links section (Substack, X, etc.)        |
| Contact/response disclaimer text     | "If you have any comments, please contact me at audreymorganlee@gmail.com" |
| Copyright © 1978-2025               | Copyright © 2025 Audrey Lee                    |
