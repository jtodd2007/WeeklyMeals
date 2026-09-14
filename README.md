# Weekly Meal & Grocery Planner

A self-contained meal-planning app (single `index.html`, no build step) for
picking breakfasts, lunches, dinners, and snacks from the current sale ad,
building a priced grocery list, and staying under a weekly budget.

## Features
- Adjustable household size (adults/kids) and weekly budget ($25–$500)
- Breakfast / Lunch / Dinner tabs, with Lunch+Dinner sharing one combined
  meal-count slider and Breakfast on its own
- Cuisine filters (Mexican, American, Italian, Mediterranean, Asian)
- Snack categories (Fruit, Veggie, Dairy, Salty & Crunchy, Sweet)
- "Quick meals" target (1–3 meals under 20 minutes) with a ⚡ filter
- ★ Favorites for meals and snacks, saved on-device
- Live grocery list generated from selected meals/snacks, with adjustable
  quantities for anything already on hand
- "Update prices" panel — paste a price block or edit items individually;
  meal/snack costs recalculate automatically

## Updating prices each week
1. Open the app, tap **Update prices**
2. Paste a `key:price` block (ask Claude to read the new ad and generate
   one) into the paste box, tap **Import**, then **Save prices**
   — or edit individual item prices by hand
3. Prices persist on your device until reset

## Hosting
This repo is set up for GitHub Pages: Settings → Pages → Deploy from branch
→ `main` / `(root)`. The site will be live at
`https://<username>.github.io/<repo-name>/`.

## Local editing
All data (ingredient catalog, meals, snacks) lives in the `<script>` block
at the bottom of `index.html`. No dependencies, no build tools — edit and
reload.
