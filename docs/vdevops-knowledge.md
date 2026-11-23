# vdevops — knowledge

As of 19 Nov 2026. Built from Rakesh's ChatGPT and Gemini history and this session. Items marked **[confirm]** need Rakesh.

## What vdevops is
A DevOps hub with three jobs:
1. **Mentoring:** a free group session (first run on ADPList, 24 Sep 2026), then paid one-to-one mentoring with real assignments. Charging is deliberate, to keep both sides regular.
2. **Network and hiring:** mentees build a portfolio from their assignments; companies come to hire DevOps people from the network. Consulting from Rakesh sits alongside.
3. **Knowledge:** practical write-ups from real production work.

Longer term: mentees help build tools for Rakesh's wider ecosystem (anubandhlife.org and others) and become subscribers to vdevops.

## Audience
- Developers, support engineers and sysadmins moving into DevOps (mentoring).
- Small and mid-size companies needing a DevOps engineer or a short fixed-scope engagement (hire and consulting).

## What Rakesh can credibly offer (from his own work)
- AWS (EC2, ALB, S3, IAM, CloudWatch, Lambda, Bedrock), Linux (Amazon Linux 2023), Nginx, MongoDB.
- GitLab CI/CD on small runners, build-and-deploy scripting, monitoring with alerts only on state change, Ansible checks.
- LLM cost and usage attribution on AWS Bedrock (request metadata, invocation logging, inference profiles).
- Do not name eaciit, JKLC or any client on the site.

## Offer details
- 1:1 price and session length: **[confirm]**. The site says "Price on request".
- Booking: ADPList profile link **[confirm]**.
- Contact email: **[confirm]**. The site shows hello@vdevops.in; check the mailbox exists.
- Payment method for 1:1 (UPI, Razorpay link, ADPList paid sessions): **[confirm]**.

## Site history
| When | What |
| --- | --- |
| Mar 2023 | GitHub org `vdevops-in` created; `frontend` repo initialised, still empty. |
| Nov 2024 | `vdevops-in/scripts` repo, last pushed. |
| Apr 2025 | vdevops.in listed among Rakesh's domains (Hostinger). |
| Mar 2026 | vdevops.in not resolving. |
| Sep 2026 | Next.js site generated with v0 by Vercel (talent-network landing, hire/intake forms, Neon DB, Resend email). Exported as zip, pushed to a vdevops-in repo, deployed on Hostinger's Node web app. The application form failed ("We couldn't submit your application"). |
| 19 Nov 2026 | Decided to replace it with a plain HTML/CSS site. First version pushed to `vdevops-in/website` (commit bbee965). |
| 19 Nov 2026 | Checked live: DNS on Hostinger nameservers (`dns-parking.com`), `www` via Hostinger CDN, old Next.js site still serving. Decided to host the new site on Vercel and delete the Hostinger web app. |

The old Next.js repo isn't visible to Claude's GitHub access, and its exact name is **[confirm]**. The decision is to overwrite or retire it, not to merge.

## Open items
- [x] Confirm how vdevops.in is deployed today: Hostinger Node web app, DNS on Hostinger (checked 19 Nov 2026).
- [x] Import `vdevops-in/website` into Vercel (done 23 Nov 2026).
- [ ] Add `vdevops.in` and `www.vdevops.in` as domains in Vercel.
- [ ] Set the DNS records Vercel shows, in Hostinger's DNS panel; check the new site is live.
- [ ] Delete the old Hostinger web app and its Neon/Resend setup (after the new site is live).
- [ ] Fill the three placeholders: ADPList link, price/session length, contact email.
- [ ] Decide whether `vdevops-in/frontend` (empty) should be deleted.
- [ ] First resource posts: Bedrock cost attribution; a fast GitLab pipeline on one small runner; health checks that alert on change; splitting one EC2 dev box into UAT app and DB.

## Business rules that apply (from Rakesh's ventures plan)
- Push toward the first paying mentee, not toward more pages.
- No new site features unless they help someone book or pay.
