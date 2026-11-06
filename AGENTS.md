# AGENTS.md

Rules for any AI agent working on this site (Gabriele-Usai.github.io), the personal website of Gabriele Usai.

## Source of truth

- Gabriele's resume is the source for all career content. Do not invent, round, or embellish numbers, titles, dates, or employers.
- Exception: the IDC bullets were rewritten by Gabriele on Nov 5, 2026 (internal AI-initiatives platform, production agent with the CFO, AI enablement workshops). They are approved and live in `index.html`.
- Exception: the IDC title on the site is "AI Specialist Intern" (the resume says "AI Finance Intern"). Gabriele chose this. Do not change it back.
- Exception: the header tagline (two lines: "AI Specialist Intern at IDC" / "Master's Graduate at Fordham University") was written by Gabriele and is approved. "Graduate" is capitalized.
- Keep bullet wording as Gabriele wrote it. Fix only obvious typos and say what you fixed.
- If the site and the resume disagree, tell Gabriele. Do not silently "fix" either one.
- Sections, in order: Education (left column), Experience (right column), Projects. On phones they stack in that order.

## Never publish

- Phone number, home address, date of birth, or any government ID.
- Salary, compensation, or offer details.
- Confidential employer material (IDC, United Nations, Banca Generali): internal documents, decks, screenshots, data, or the names of internal tools beyond what the resume says.
- Secrets of any kind: API keys, tokens, passwords, `.env` files.
- Photos of other people, or names of colleagues, classmates, or references.

## Approved so far

- Email: usaigabrialberto@gmail.com (the "Send message" button).
- LinkedIn: https://www.linkedin.com/in/gabriele-usai/
- GitHub: https://github.com/Gabriele-Usai (the Projects button).
- Headshot: `assets/logos/photo.jpg` (Gabriele keeps it in the logos folder on purpose; the page loads it from there).
- Logos in `assets/logos/`, supplied by Gabriele to identify his schools and employers: `fordham.edu.png`, `unicatt.it.png`, `lse.ac.uk.png`, `idc.com.png`, `un.org.png`, `bancagenerali.it.png`.

## Working on the site

- Gabriele makes changes by asking in chat. When he asks for a change, make it, check it, commit to `main`, and push. No need to ask again.
- Ask Gabriele first before:
  - deleting or overwriting files he uploaded himself,
  - changing GitHub settings, Pages settings, or the domain,
  - adding new pages or sections he didn't ask for,
  - adding third-party scripts, analytics, trackers, cookies, or forms,
  - adding any contact detail, photo, or profile not listed above.
- After pushing, the "Deploy site" workflow (`.github/workflows/deploy.yml`) publishes the site in about 30 seconds. Check that the run succeeded before saying the change is live. Never delete this workflow: without it, changes stop going live.
- Commit messages: short and plain ("Update IDC bullets", "Add new headshot").

## Hosting

- Live at https://gabriele-usai.github.io (GitHub Pages, repo `Gabriele-Usai/Gabriele-Usai.github.io`, branch `main`).
- `.nojekyll` tells GitHub to publish the files as they are. Keep it.
- If a custom domain is added later, it goes in a `CNAME` file at the repo root. Never delete or edit that file without asking, or the domain breaks.

## Style

- Professional and restrained. White background; the work and the experience are the focus, not effects.
- Favicon: 💼 (briefcase), Gabriele's choice. It is the only emoji on the site.
- Colors: white `#FFFFFF`, ink `#0E1A2B`, navy accent `#2B4C9B`, plus grays derived from them. No other colors except inside the logos.
- Typography: one family, DM Sans (loaded from Google Fonts). No decorative fonts.
- Layout: photo and name top left with the two-line tagline; "Send message" then "LinkedIn" buttons top right. Education on the left, Experience on the right. Every role and school is a dropdown: the closed card shows logo, title, organization, dates, and location; opening it shows the bullets.
- Projects: a single "See my projects on GitHub" button. No project cards.
- Plain static HTML and CSS in one `index.html`. No frameworks or build steps unless Gabriele asks.
- Must work on phones (no horizontal scroll) and be accessible: semantic HTML, alt text, visible focus states, enough contrast.
- Link previews: keep `og:description` and the meta description in sync with the header tagline.
- Writing: plain language, no buzzwords, no exaggeration. Keep text light.
