# NBTI · Nextgen Connect — CAIF Toronto 2026

**Official digital presence for the National Board for Technology Incubation (NBTI) delegation at the Canada–Africa Innovation Festival, Toronto — May 29–30, 2026.**

Built and produced by **UKALD** in partnership with **NBTI, Abuja**.

---

## Overview

A three-page standalone web suite serving two audiences — public stakeholders connecting with the NBTI delegation, and the delegation team managing leads on the festival floor.

| File | Purpose | Audience |
|---|---|---|
| `index.html` | Public-facing microsite — delegation brief, registration form | Investors, partners, government, corporates |
| `investor-capture.html` | Live workspace — lead capture, scoring, analytics, follow-ups | NBTI delegation team |
| `user-guide.html` | Screen-by-screen operational guide | Delegation staff, festival team |

---

## Pages

### `index.html` — Nextgen Connect
The public microsite. Explains the NBTI mission, showcases the delegation brief, and allows stakeholders to register their interest via a structured connection form. Every submission is routed directly to `topeomojayogbe@ukald.com` via FormSubmit with a generated ledger token for tracking.

### `investor-capture.html` — Investor Capture Workspace
A five-tab internal dashboard for the delegation team. Features:
- **Overview** — live lead stream with filter chips and search
- **All Leads** — full paginated lead list with tag filtering
- **Analytics** — lead mix breakdown, hourly capture chart, country distribution
- **Meetings** — scheduled follow-up sessions
- **Exports** — CSV, PDF, vCard, Salesforce and HubSpot export options

Opening any lead card reveals a full detail panel with lead score, contact info, notes, and one-click actions including **Send follow-up email** (routes to `topeomojayogbe@ukald.com`), schedule meeting, mark as hot lead, export vCard, and call.

### `user-guide.html` — User Guide
A clean operational reference guide for delegation staff and festival team. Eight sections covering access, lead capture, follow-up, stakeholder review, exports, tips, and FAQ. Standalone — no login required.

---

## Technical Notes

- **Pure HTML/CSS/JS** — no framework, no build step, no dependencies
- **Self-contained** — all logos embedded as Base64; no external asset requests required
- **Cross-linked** — Nextgen Connect header links to Investor Capture; Investor Capture back-links to Nextgen Connect
- **Form delivery** — [FormSubmit.co](https://formsubmit.co) used as a no-backend mail relay; no server required
- **Fonts** — Cormorant Garamond, Inter, JetBrains Mono via Google Fonts

---

## Deployment

### Vercel (recommended)
1. Import this repository at [vercel.com](https://vercel.com)
2. Set Framework Preset to **Other**
3. Leave Build Command and Output Directory blank
4. Deploy

Live URLs after deployment:
```
yoursite.vercel.app                          → Nextgen Connect (index)
yoursite.vercel.app/investor-capture.html    → Investor Capture
yoursite.vercel.app/user-guide.html          → User Guide
```

### Local
Open any `.html` file directly in a browser. All three files must be in the same folder for cross-navigation to work.

---

## File Structure

```
/
├── index.html               ← Nextgen Connect (public microsite)
├── investor-capture.html    ← Investor Capture (delegation workspace)
├── user-guide.html          ← User Guide (operational reference)
└── README.md
```

---

## Contacts

| Role | Contact |
|---|---|
| Programme facilitation & technical | topeomojayogbe@ukald.com |
| Festival lead on the floor | Amaka Obi |

---

## Partners

| Organisation | Role |
|---|---|
| **NBTI — National Board for Technology Incubation** | Convening body · Federal Republic of Nigeria |
| **UKALD** | Production partner · Programme facilitator |
| **CAIF — Canada–Africa Innovation Festival** | Host event · Toronto, Ontario · May 2026 |

---

*© 2026 Federal Republic of Nigeria · National Board for Technology Incubation. All institutional marks used under official engagement.*
