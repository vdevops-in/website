# vdevops.in — website repo

Code for the public site **vdevops.in**. Owner: Rakesh Verma (DevOps lead, 15+ years; AWS Solutions Architect; CKA). Background and goals: `docs/vdevops-knowledge.md`.

## Pipeline
- **Source of truth:** GitHub `vdevops-in/website`, branch `main`.
- **Change flow:** edit locally → test → commit → push. Small copy fixes go straight to `main`. Anything larger goes on a branch with a PR.
- **Deploy target:** Vercel (static, no build), decided 19 Nov 2026. Repo connected to Vercel (23 Nov 2026): `main` is production, other branches get preview URLs. The domain is not pointed at Vercel yet, so vdevops.in still shows the old site until DNS is switched.
- **Domain:** `vdevops.in`, registered at Hostinger. As of 19 Nov 2026, DNS is on Hostinger nameservers and still serves the old Next.js site from Hostinger's Node web app. Rakesh will point it at Vercel and delete the old Hostinger setup.
- **Do not** touch Vercel, Hostinger, DNS or GitHub settings from the browser. Rakesh does those himself.

## Stack
- Plain HTML + one CSS file. No build step, no npm, no frameworks, no external scripts or fonts.
- `vercel.json`: clean URLs (`/mentoring` serves `mentoring.html`) and basic security headers. Harmless if hosted elsewhere.

## Files
- `index.html`: single landing page with hero, three pillars, mentoring, companies, resources and contact.
- `styles.css`: all styling; light and dark via `prefers-color-scheme`; mobile breakpoint 760px.
- `404.html`, `favicon.svg`, `README.md`.
- Placeholders still to fill carry a `data-todo="…"` attribute: `grep -n data-todo *.html`.

## Rules
- Keep it fast and simple. No dependencies unless Rakesh asks. If a blog is needed, propose Astro first and wait for approval.
- Check at 375px and 1280px wide, light and dark, before committing.
- Never commit secrets, keys, tokens or personal data.
- Small commits with clear messages.
- Be crisp. Ask before large rewrites, and ask instead of assuming architecture or deploy decisions.
- Push only when Rakesh says so.
