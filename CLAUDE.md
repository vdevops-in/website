# vdevops.in

Website for **vdevops**: a DevOps learning hub and network run by Rakesh Verma (DevOps lead, 15+ years, AWS SA, CKA). Purpose, in order:
1. Sell paid one-to-one DevOps mentoring (free ADPList group session → paid 1:1 with real assignments).
2. Offer consulting and "hire from the network" to companies.
3. Publish practical DevOps write-ups from real production work.

## Stack
- Plain HTML + one CSS file. No build step, no npm, no frameworks, no external scripts or fonts.
- Hosted on **Vercel**, connected to GitHub `vdevops-in/website`. Push to `main` = production deploy; every other branch/PR gets a preview URL.
- `vercel.json`: clean URLs (`/mentoring` serves `mentoring.html`) and basic security headers.
- Domain `vdevops.in` is registered at Hostinger; DNS records point to Vercel.

## Files
- `index.html` — single landing page: hero, three pillars, mentoring, companies, resources, contact.
- `styles.css` — all styling; light and dark via `prefers-color-scheme`; mobile breakpoint 760px.
- `404.html`, `favicon.svg`.
- Placeholders still to fill are marked with a `data-todo="…"` attribute. Find them with `grep -n data-todo *.html`.

## Rules for changes
- Keep it fast and simple: no dependencies unless Rakesh asks. If a blog is needed later, propose Astro first and wait for approval.
- Test at 375px and 1280px wide before committing.
- Never commit secrets, keys or personal data.
- Small commits with clear messages; open a PR for anything beyond copy edits.
- Be crisp; ask before large rewrites.
