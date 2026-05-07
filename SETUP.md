# 🛠️ Profile Repo Setup Guide

This is the source for the **garrettadams23** GitHub profile README.
Follow these steps to get everything working, including live stats and the snake animation.

---

## 📁 Repo Structure

```
garrettadams23/
├── README.md                          ← Your public profile (edit this)
├── SETUP.md                           ← This file
└── .github/
    └── workflows/
        ├── snake.yml                  ← Auto-generates contribution snake SVG (daily)
        ├── activity.yml               ← Auto-updates recent GitHub activity (every 30 min)
        └── metrics.yml                ← (Optional) Advanced metrics card
```

---

## ✅ Step 1 — Create the Profile Repo

1. Go to [github.com/new](https://github.com/new)
2. Set the repo name to exactly: `garrettadams23`  
   *(must match your username exactly)*
3. Set it to **Public**
4. **Do NOT** initialize with a README (you'll push your own)
5. Click **Create repository**

---

## ✅ Step 2 — Push Your Files

```bash
# Clone or init locally
git init garrettadams23
cd garrettadams23

# Copy in your README.md and .github/ folder, then:
git add .
git commit -m "init: profile readme"
git branch -M main
git remote add origin https://github.com/garrettadams23/garrettadams23.git
git push -u origin main
```

---

## ✅ Step 3 — Enable the Snake Animation

The snake reads your contribution graph and generates an SVG automatically.

1. In your repo, go to **Settings → Actions → General**
2. Under **Workflow permissions**, select **Read and write permissions**
3. Save.
4. Go to **Actions** tab → select **Generate Snake Animation** → click **Run workflow**

The snake SVGs will be pushed to an `output` branch automatically.  
After the first run, the snake in your README will be live. ✅

> The workflow then re-runs every 24 hours on a cron schedule.

---

## ✅ Step 4 — Enable Recent Activity Auto-Updates

The `activity.yml` workflow uses [jamesgeorge007/github-activity-readme](https://github.com/jamesgeorge007/github-activity-readme) to automatically populate your last 6 GitHub events into the README every 30 minutes.

1. **No secrets needed** — it uses the built-in `GITHUB_TOKEN`
2. Make sure **Read and write permissions** are enabled (same as Step 3)
3. Trigger manually: **Actions → Update Recent Activity → Run workflow**
4. The content between `<!--START_SECTION:activity-->` and `<!--END_SECTION:activity-->` in your README will be replaced with live data ✅

> Events tracked: pushes, PRs, issues, comments, stars, forks, code reviews.

---

## ✅ Step 5 — (Optional) Metrics Workflow

The `metrics.yml` workflow uses [lowlighter/metrics](https://github.com/lowlighter/metrics) to generate an advanced stats image.

1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Generate a **classic** token with `read:user` and `repo` scopes
3. In your profile repo, go to **Settings → Secrets and variables → Actions**
4. Add a secret named `METRICS_TOKEN` with your token value
5. Go to **Actions → Update README Stats → Run workflow**

---

## 🎨 Customization Tips

| What to change | Where |
|---|---|
| Accent color (`#00b4d8`) | Search & replace in `README.md` |
| Stats theme | Change `tokyonight` to any [theme name](https://github.com/anuraghazra/github-readme-stats/blob/master/themes/README.md) |
| Typing SVG lines | Edit the `lines=` param in the typing SVG URL |
| Featured projects table | Edit the table in `README.md` manually |
| About Me YAML block | Edit the code block near the top |

---

## 🔗 Services Used (all free)

| Service | Purpose |
|---|---|
| [capsule-render](https://github.com/kyechan99/capsule-render) | Animated wave header/footer |
| [readme-typing-svg](https://github.com/DenverCoder1/readme-typing-svg) | Typing animation |
| [github-readme-stats](https://github.com/anuraghazra/github-readme-stats) | Stats, top languages & pinned repo cards |
| [github-readme-streak-stats](https://github.com/DenverCoder1/github-readme-streak-stats) | Streak counter |
| [github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy) | Trophy display |
| [github-readme-activity-graph](https://github.com/ashutosh00710/github-readme-activity-graph) | Activity graph |
| [platane/snk](https://github.com/Platane/snk) | Contribution snake SVG (via Actions) |
| [jamesgeorge007/github-activity-readme](https://github.com/jamesgeorge007/github-activity-readme) | Auto-updated recent activity section (via Actions) |
| [komarev/ghpvc](https://github.com/antonkomarev/github-profile-views-counter) | Profile view counter |
