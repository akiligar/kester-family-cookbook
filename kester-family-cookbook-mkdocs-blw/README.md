# Kester Family Cookbook — MkDocs BLW Framework

This repository publishes the Kester Family Cookbook as a small MkDocs site.

## Project boundary

The cookbook site is the complete family recipe record, including Baby-Led Weaning details that do not fit cleanly in a standard recipe app.

AnyList can still be used for shopping, meal planning, and kitchen execution. The recipe pages include JSON-LD Recipe schema so the standard recipe can be imported through a browser recipe extension.

## Do not add by default

- Photos
- Database
- CMS
- Search
- Comments
- Ratings
- Nutrition calculator
- Meal-planning app
- Custom import automation
- Recipe sync

## Cloudflare Pages settings

Use these settings for Cloudflare Pages:

```text
Framework preset: MkDocs
Build command: pip install -r requirements.txt && mkdocs build
Build output directory: site
Root directory: blank
Production branch: main
```

If Cloudflare already installs dependencies for your project, `mkdocs build` may work. The explicit command above is more reliable.

## Local preview

```bash
pip install -r requirements.txt
mkdocs serve
```

Open the local URL shown by MkDocs.

## Adding a recipe

1. Check `tools/recipe-index.csv`.
2. Decide whether the meal is new, duplicate, variation, or not worth saving.
3. Copy `docs/templates/recipe-template.md` into a new folder under `docs/recipes/`.
4. Fill in the standard recipe and BLW notes.
5. Add the page to `mkdocs.yml` navigation.
6. Add/update the row in `tools/recipe-index.csv`.
7. Deploy and test browser-extension import.

## Maintenance rule

Only add features that clearly help one of these jobs:

1. Preserve the complete family recipe.
2. Support Baby-Led Weaning adaptations.
3. Reduce duplicate recipe creation.
4. Improve browser-extension import quality.
5. Make future recipe revision easier.
