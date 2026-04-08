# Dre's Grind — Project Context

## What this is
A personal fitness and lifestyle accountability dashboard. Single HTML file,
vanilla JS, Chart.js for charts, localStorage for data persistence.

## v2 (Complete)
- Sage design system — premium wellness app aesthetic
- Whole30 nutrition tracking with daily compliance logging
- No-drink streak tracker
- Meal prep hub with recipes, meal planner, and shopping lists
- San Diego countdown (May 23, 2026)
- Workout activity dropdown (10 activities)
- Weight tracking toward goal weight with pace line
- Weekly and monthly stats with dual heatmaps and charts
- Deployed to: dretheprophet-pixel.github.io/dres-grind

## v3 Goals — Smart Recipe Hub
Milestone #2, due April 12, 2026. Branch: `feature/v3-recipe-hub`

Issues in order:
- #12 Supabase: Recipe Database Migration — move recipes from localStorage to Supabase for cross-device persistence
- #13 Vercel: Spoonacular API Proxy — secure Spoonacular API key behind a Vercel serverless function
- #14 Recipe Search & Auto-populate — search Spoonacular and auto-fill recipe form (ingredients, instructions, image)
- #15 Recipe Images — display recipe images from Spoonacular or manual URL in recipe cards
- #16 Whole30 Recipe Filtering — filter Spoonacular search results to Whole30-compliant recipes only
- #17 Cross-device Sync — sync all app data (not just recipes) to Supabase

## Current recipe object shape (localStorage)
```js
{
  id: Date.now(),       // number
  name: string,
  tags: string[],       // e.g. ['Whole30']
  ingredients: [{ item: string, qty: string }],
  instructions: string,
  createdAt: string     // 'YYYY-MM-DD'
}
```

## Code Preferences
- Single HTML file (no build process, no frameworks)
- Explain what you're building before writing it — no code until Dre reviews the plan
- Keep changes focused — one issue at a time
- Commit after each issue is complete and working

## Infra
- Supabase: recipe storage and eventual full sync
- Vercel: serverless proxy for Spoonacular API key protection

## Branch
Always work on `feature/v3-recipe-hub` — never commit directly to main