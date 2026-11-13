# CorporateEnergies Limited — Website

Static website (HTML, CSS, JavaScript). No build step required.

## Pages
| File | Page |
|---|---|
| index.html | Home |
| about.html | About Us |
| services.html | Services overview |
| energy-training.html | Energy Education & Training |
| hse.html | HSE, Risk & Compliance |
| competency.html | Competency & Assessment |
| professional-development.html | Executive & Professional Development |
| workforce-advisory.html | Workforce & Institutional Advisory |
| corporate-training.html | Corporate Training Solutions |
| contact.html | Contact & Request a Proposal (the only form) |
| thank-you.html | Shown after the form is submitted |

Shared styles are in `css/style.css`, the mobile menu and scroll animations in `js/main.js`, images in `assets/img/`.

## Push to GitHub
```bash
cd corporateenergies-website
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/corporateenergies-website.git
git push -u origin main
```
(Create the empty repository on github.com first.)

## Deploy on Netlify
1. In Netlify: **Add new site → Import an existing project → GitHub**, pick this repository.
2. Leave the build command empty; publish directory is `.` (already set in `netlify.toml`).
3. Deploy. Every push to `main` redeploys automatically.
4. **Domain:** Site configuration → Domain management → add `corporateenergies.com`, then update your DNS as Netlify instructs.

## Contact form
The form on `contact.html` uses **Netlify Forms** (`data-netlify="true"`). After the first deploy:
- Submissions appear under **Forms → proposal-request** in Netlify.
- To get them by email: **Forms → Form notifications → Add notification → Email notification**.

## Before going live
Replace these placeholders (search the files for `[`):
- `[Insert verified business address]`, `[Insert verified official email address]`, `[Insert approved phone / WhatsApp number]` in `contact.html`
- `[Official email address]`, `[Phone / WhatsApp]`, `[Business address]` in the header strip and footer of every page

Photos are from Pexels (free to use). The hero photo shows another company's logo on the hard hats; consider replacing it.
