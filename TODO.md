# Dre's Grind — TODO

## Current State
Single HTML file (`index.html`) on branch `feature/v3-recipe-hub`.
Live at: https://dretheprophet-pixel.github.io/dres-grind
Repo: https://github.com/dretheprophet-pixel/dres-grind

v2 complete — sage design system, Whole30 tracker, no-drink streak,
meal prep hub, San Diego countdown, weight tracking, heatmaps.

---

## Milestone: v2 — Full Redesign ✅ COMPLETE

- [x] Issue #1 — Design system: light mode + sage accent
- [x] Issue #2 — Today page: countdown, Whole30, no-drink streak
- [x] Issue #3 — Workout logging: activity dropdown
- [x] Issue #4 — Whole30 & nutrition tracker
- [x] Issue #5 — No-drink streak tracker
- [x] Issue #6 — Meal prep hub: recipes + shopping lists
- [x] Issue #7 — Weight & milestone tracking
- [x] Issue #8 — Weekly & monthly stats, heatmaps

---

## Milestone: v3 — Smart Recipe Hub (due April 12, 2026)

### ✅ Done
- [x] Issue #12 — Supabase: Recipe Database Migration
      → Recipes synced to Supabase, localStorage fallback intact,
        one-time migration on first load, anon key secured

### 🔄 Ready
- [ ] Issue #13 — Vercel: Spoonacular API Proxy
      → Serverless function to protect Spoonacular API key
      → Pro account secured, API key ready

### 📋 Up Next
- [ ] Issue #14 — Recipe Search & Auto-populate
- [ ] Issue #15 — Recipe Images
- [ ] Issue #16 — Whole30 Recipe Filtering
- [ ] Issue #17 — Cross-device Sync

---

## Workflow
- Branch: `feature/v3-recipe-hub` — never commit to main
- Commit message format: `feat: #N short description`
- Claude Code: always read CLAUDE.md first, propose plan, wait for approval
- After each issue: test in browser → commit → push → close on GitHub
- If push is rejected: `git stash` → `git pull --rebase` → `git stash pop` → push
- Final step: PR from `feature/v3-recipe-hub` → `main` when all 6 issues done

---

## Key Dates
- San Diego Trip: May 23, 2026
- v3 Milestone due: April 12, 2026

## Infra
- Supabase project: `dres-grind` (xmolnnnrmcyenntzrrig.supabase.co)
- Vercel: proxy for Spoonacular API (set up in #13)
- Spoonacular: Pro account, API key ready

## Claude Code Tips
- Always ask for the plan before building — no code until Dre approves
- Review in browser before committing (check console for errors)
- Commit after each issue: `feat: #N description`
- Use anon key only — never secret key in client-side code