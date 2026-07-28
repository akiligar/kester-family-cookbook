# Recipe Finalization Checklist

## 1. Duplicate check

Check `tools/recipe-index.csv`.

Decide one:

- New recipe
- Variation of existing recipe
- Update existing recipe
- Not worth saving

Do not create a new page for a minor variation.

## 2. Standard recipe

Confirm:

- Title
- Slug
- Description
- Servings
- Prep time
- Cook time
- Total time
- Ingredients
- Instructions

## 3. Recipe schema

Confirm JSON-LD Recipe schema includes:

- name
- description
- recipeYield
- prepTime
- cookTime
- totalTime
- recipeIngredient
- recipeInstructions

Use ISO 8601 durations:

- 10 minutes = PT10M
- 1 hour = PT1H
- 1 hour 15 minutes = PT1H15M

## 4. BLW fields

Confirm:

- Baby portion
- Set aside before
- Texture target
- Cut or shape guidance
- Allergen notes
- Choking-risk flags

## 5. Site updates

Update:

- `mkdocs.yml` nav
- `docs/recipes/index.md`
- `tools/recipe-index.csv`
