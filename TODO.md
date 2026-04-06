# Dre's Grind — v2 Redesign TODO

## Current State
Single HTML file (`index.html`) on branch `redesign/v2`.
Live at: https://dretheprophet-pixel.github.io/dres-grind
Repo: https://github.com/dretheprophet-pixel/dres-grind

Design system complete — light mode, sage green accent, Chart.js 
updated, all old dark palette removed.

---

## Milestone: v2 — Full Redesign (due May 16, 2026)

### ✅ Done
- [x] Issue #1 — Design system: light mode + sage accent

### 🔄 In Progress
- [ ] Issue #2 — Today page: San Diego countdown, Whole30 counter, 
      no-drink streak, daily check-in summary
      → Next step: prompt Claude Code to build it (button approach 
      for Whole30 + no-drink start dates)

### 📋 Up Next
- [ ] Issue #3 — Workout logging: activity dropdown replacing checkboxes
- [ ] Issue #4 — Whole30 & nutrition tracker (full page)
- [ ] Issue #5 — No-drink streak tracker (dedicated section)
- [ ] Issue #6 — Meal prep hub: recipes + shopping lists
- [ ] Issue #7 — Weight & milestone tracking update
- [ ] Issue #8 — Weekly & monthly stats refresh

---

## Workflow
- Branch: `redesign/v2` — never commit to main during redesign
- Commit message format: `Issue #N — short description`
- After each issue: close it on GitHub Project board
- Final step: PR from `redesign/v2` → `main` when all 8 issues done

---

## Key Dates
- San Diego Wedding: May 23, 2026
- Milestone due: May 16, 2026

## Data Model (current)
```json
data.workouts[]     // existing
data.weights[]      // existing
data.whole30Start   // NEW — added in Issue #2
data.nodrinkStart   // NEW — added in Issue #2
data.meals[]        // NEW — added in Issue #2
```

## Claude Code Tips
- Always ask for the plan before building
- Review in browser before committing
- Commit after each issue with message: Issue #N — description