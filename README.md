# K13ruuu.github.io

Personal portfolio site for **James Kenneth A. Tamaca** — Electronics Engineering graduate specializing in embedded systems, LoRaWAN/IoT, and applied data/AI. Built to support job applications in software development, AI engineering, and data annotation.

**Live site:** https://K13ruuu.github.io

## About

Single-page portfolio covering:

- **About** — background and current focus
- **Skills** — programming, IoT/embedded, web development, data & AI, tools
- **Thesis case study** — *Development of a LoRaWAN-Enabled Per-Tree Monitoring Device for Geolocation and Forest Disturbance Detection*, built with DENR-CENRO Sta. Cruz, Laguna
- **Projects** — showcase work, with room to add more
- **Certifications** — Cisco, Yeastar, AWS
- **Experience** — internship, org leadership, education
- **Contact** — email, GitHub, LinkedIn, resume

## Stack

Plain HTML, CSS, and JavaScript — no build step, no framework. Everything lives in a single `index.html` so it's easy to read, edit, and deploy as-is on GitHub Pages.

- Fonts loaded from Google Fonts (Space Mono + Inter)
- No external JS dependencies
- No backend — the contact section links out to email/GitHub/LinkedIn rather than using a form

## Before you publish: things to fill in

Search `index.html` for the `EDIT-ME` comment near the bottom of the `<script>` tag. Update:

| What | Where | Current placeholder |
|---|---|---|
| Email | `emailLink` | `YOUR.EMAIL@example.com` |
| GitHub profile | `githubLink` | `https://github.com/K13ruuu` (confirm this is correct) |
| LinkedIn profile | `linkedinLink` | `YOUR-LINKEDIN-HANDLE` |
| Resume file | `resumeLink`, `resumeLink2` | expects a file named `resume.pdf` in the repo root |
| FORGED Youth project | `forgedProjectLink` + the project card copy in `#projects` | placeholder link and an empty description — fill in what the site is, your role, and the link |

To add your resume: drop a PDF named `resume.pdf` in the same folder as `index.html`.

## Photo

`profile.jpg` is included in this repo and is already wired up in the hero section (`<img src="profile.jpg" ...>`). Keep the filename as-is, or update the `src` in `index.html` if you rename it.

## Running locally

No build tools needed. Either:

1. Open `index.html` directly in a browser, or
2. Serve it locally for a closer-to-production preview:
   ```bash
   python3 -m http.server 8000
   ```
   then visit `http://localhost:8000`

## Deploying to GitHub Pages

This repo is already named `K13ruuu.github.io`, which GitHub Pages treats as a special **user site** — it publishes automatically from the `main` branch with no extra configuration.

1. Commit `index.html` (and `resume.pdf`, once added) to the `main` branch
2. Push to GitHub: `git push origin main`
3. In the repo, go to **Settings → Pages** and confirm the source is set to `main` / `root`
4. The site will be live at `https://K13ruuu.github.io` within a few minutes

## Updating content later

Everything is in `index.html`, organized into clearly commented sections (`HERO`, `ABOUT`, `SKILLS`, `THESIS CASE STUDY`, `PROJECTS`, `CERTIFICATIONS`, `EXPERIENCE`, `CONTACT`). To add a new project, copy an existing `.project-card` block inside `#projects` and edit the text. To add a certification, copy a `<tr>` row inside the `#certifications` table.

## License

Personal portfolio — content and copy belong to James Kenneth A. Tamaca. Feel free to reference the structure/CSS for your own site.
