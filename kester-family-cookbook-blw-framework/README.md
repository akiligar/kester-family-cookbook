# Kester Family Cookbook BLW Framework

This repository publishes a simple `/cookbook/` section for family recipes.

## Project boundary

This is the complete family recipe record.

AnyList is still useful for shopping, meal planning, and kitchen execution, but the website holds the family context that does not fit cleanly into a standard recipe app.

## What this framework includes

- Static HTML only
- One page per recipe
- Standard recipe content
- Baby-led weaning adaptation fields
- JSON-LD Recipe schema for browser-extension import
- A thin recipe index
- A repeatable finalization checklist

## What this framework excludes

- Photos
- Build system
- Database
- Search
- Comments
- Ratings
- Nutrition calculator
- Meal planner
- Recipe app synchronization
- Custom import automation

## Folder structure

```text
cookbook/
  README.md
  CNAME
  index.html
  styles.css
  recipes/
    example-family-chicken/
      index.html
  templates/
    recipe-template.html
  tools/
    blw-field-guide.md
    recipe-checklist.md
    recipe-index.csv
    finalization-prompt.md
```

## Recipe page model

Each recipe page has two layers.

### 1. Standard recipe

This is the part intended for clean browser-extension import.

It includes:

- title
- description
- servings
- prep time
- cook time
- total time
- ingredients
- instructions
- JSON-LD Recipe schema

### 2. Family and BLW notes

This is the part that makes the recipe useful for the family.

It includes:

- baby-led weaning adaptation
- what to set aside before salt, sugar, or adult seasoning
- texture target
- cut or shape guidance
- allergen notes
- choking-risk flags
- adult finishing steps
- family notes
- revision history

## Maintenance rule

Do not add a feature unless it helps one of these jobs:

1. Preserve the complete family recipe.
2. Support BLW adaptations.
3. Reduce duplicate recipe creation.
4. Make browser-extension import cleaner.
5. Make future recipe revision easier.

If it does not serve one of those jobs, leave it out.

## New recipe workflow

1. Check `tools/recipe-index.csv`.
2. Decide whether the meal is new, a duplicate, or a variation.
3. If it is a keeper, create a new folder under `recipes/`.
4. Copy `templates/recipe-template.html`.
5. Fill in the standard recipe.
6. Fill in the BLW adaptation.
7. Update `index.html`.
8. Update `tools/recipe-index.csv`.
9. Open the published page and test browser-extension import.
10. If the imported recipe is messy, fix the page template before adding more recipes.

## Safety note

BLW notes in this framework are family planning notes, not medical advice. Keep using current pediatric guidance and your clinician's advice for choking hazards, allergens, readiness, and food safety.
