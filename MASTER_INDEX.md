# 🗺️ Master Index — garrettadams23 GitHub Presence

> Complete map of every repo, file, workflow, and artifact built across this project.

---

## 📦 Repositories (4 total)

### 1. `garrettadams23/garrettadams23` — Profile README
> The special repo that powers your GitHub profile page

| File | Purpose |
|------|---------|
| `README.md` | Animated profile with stats, snake, WakaTime, roadmap, projects |
| `.github/workflows/snake.yml` | Daily contribution snake SVG generator |
| `.github/workflows/activity.yml` | 30-min auto-update of recent GitHub events |
| `.github/workflows/waka.yml` | Daily WakaTime coding stats updater |
| `.github/workflows/metrics.yml` | 6-hr advanced metrics card (optional) |
| `SETUP.md` | Step-by-step deployment checklist |

**Sections in README:** Header · Typing SVG · About Me (YAML) · CompTIA badges · Tech Stack · GitHub Stats · Streak · Trophies · Activity Graph · Snake · Recent Activity · Currently Studying · Cert Roadmap · Featured Projects (pinned cards) · Contact

**Run order after pushing:**
1. Settings → Actions → Read & Write permissions ✅
2. Run `snake.yml` manually once ✅
3. Run `activity.yml` manually once ✅
4. Add `WAKATIME_API_KEY` + `GH_TOKEN` secrets → run `waka.yml` ✅
5. Pin 4–6 repos from your profile page ✅

---

### 2. `garrettadams23/server-management-service` — IT Service Product
> The business documentation repo for your tiered server management offering

| File | Purpose |
|------|---------|
| `README.md` | Public landing page — tier comparison, pricing math, decision flowchart |
| `docs/PRICING.md` | Full pricing breakdown with worked examples at multiple profit levels |
| `docs/SCOPE_OF_WORK.md` | Formal deliverables, SLA table, responsibilities matrix |
| `docs/ONBOARDING.md` | 7-step client onboarding process (Day 1 → active service) |
| `docs/SERVICE_AGREEMENT.md` | Complete contract template with bracketed fields to fill in |

**Tier summary:**
| Tier | Setup | Monthly |
|------|-------|---------|
| 🥉 Starter | $500 | 2% net / $75 min |
| 🥈 Growth | $1,200 | 3.5% net / $150 min |
| 🥇 Pro | $2,500 | 5% net / $350 min |

---

### 3. `garrettadams23/nexus-dashboard` — AI Productivity Dashboard
> Personal command center: Anthropic API + Gmail/Calendar/Drive via MCP

| File | Purpose |
|------|---------|
| `README.md` | Architecture diagram, tech stack, setup guide, roadmap |
| `src-artifact.jsx` | Full 722-line React app (also runs as Claude artifact) |
| `docs/MCP_SETUP.md` | How to connect Google services via MCP in Claude.ai |

**Dashboard panels:**
- **Overview** — AI morning briefing from live Gmail + Calendar data
- **AI Chat** — Multi-turn Claude with Gmail, Calendar, Drive MCP context
- **Gmail** — Inbox reader with per-email AI summaries
- **Calendar** — 7-day event view with scheduling advice
- **Tasks** — Google Tasks with local toggle + add
- **MCP Status** — Live health checks with latency for all 3 servers

---

### 4. `garrettadams23/portfolio-db` — PostgreSQL Schema
> The data layer for myitguy.netlify.app, hosted on Neon Console

| File | Purpose |
|------|---------|
| `README.md` | Schema diagram, setup instructions, view index |
| `schema.sql` | Full DDL — 9 tables, 2 custom ENUMs, indexes, FTS, triggers |
| `seed.sql` | Complete sample data for all tables |
| `views.sql` | 6 reusable views for the application layer |
| `queries/profiles.sql` | Profile SELECT library (4 queries) |
| `queries/projects.sql` | Projects SELECT library (10 queries) |
| `queries/all_queries.sql` | Skills · Experience · Certs · Testimonials · Contacts · Analytics |

**Schema tables:** `profiles` · `skills` · `certifications` · `experience` · `projects` · `project_tags` · `testimonials` · `contacts`

**Views:** `v_featured_projects` · `v_project_summary` · `v_full_profile` · `v_skills_by_category` · `v_career_timeline` · `v_approved_testimonials`

**Seed data totals:** 1 profile · 24 skills · 3 certs · 3 experience records · 6 projects · 18 tags · 3 testimonials · 2 contacts

---

## ⚙️ Standalone Artifacts

| File | Description |
|------|-------------|
| `client-portal.jsx` | AI-powered profit reporting portal for server management clients. 3-step form, animated fee calculator, AI insight note, invoice preview. Tier-aware. |
| `nexus-dashboard.jsx` | The full Nexus Dashboard — runs as a live Claude artifact with your connected Google MCP services |
| `profile-preview.jsx` | Interactive GitHub profile preview with section navigator + deployment checklist sidebar |

---

## 📊 Total Output Summary

| Category | Count |
|----------|-------|
| GitHub repos documented | 4 |
| Markdown files | 12 |
| SQL files | 6 |
| SQL lines written | 934 |
| YAML workflow files | 4 |
| React artifact files | 3 |
| React lines written | ~1,600 |
| GitHub Actions workflows | 4 (snake · activity · waka · metrics) |
| Database tables | 9 |
| Database views | 6 |
| SELECT queries written | 40+ |

---

## ✅ Deploy Checklist (in order)

- [ ] Create `garrettadams23` repo → push profile README + workflows
- [ ] Enable Actions read/write → run snake + activity workflows manually
- [ ] Add WakaTime extension in VS Code → add secrets → run waka workflow
- [ ] Create `server-management-service` repo → push all 5 files
- [ ] Create `nexus-dashboard` repo → push README + src-artifact.jsx
- [ ] Create `portfolio-db` repo → push schema → run `schema.sql`, `seed.sql`, `views.sql` on Neon
- [ ] Pin 4–6 repos from your GitHub profile page
- [ ] Update LinkedIn + email badges in profile README
- [ ] Fill in bracketed fields in `SERVICE_AGREEMENT.md` before using with clients

---

*Built by Claude for Garrett Adams — [myitguy.netlify.app](https://myitguy.netlify.app)*
