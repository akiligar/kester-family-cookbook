# Recipe Finalization Checklist

Use this checklist when turning a meal into a permanent family cookbook page.

## 1. Duplicate check

Check `recipe-index.csv`.

Decide one:

```text
New recipe
Variation of existing recipe
Update existing recipe
Not worth saving
```

Do not create a new recipe page for a minor variation.

## 2. Standard recipe

Confirm the standard recipe has:

```text
Title
Slug
Description
Servings
Prep time
Cook time
Total time
Ingredients
Instructions
```

## 3. Browser-extension import fields

Confirm JSON-LD Recipe schema includes:

```text
name
description
recipeYield
prepTime
cookTime
totalTime
recipeIngredient
recipeInstructions
```

Use ISO 8601 durations in schema:

```text
10 minutes = PT10M
1 hour = PT1H
1 hour 15 minutes = PT1H15M
```

## 4. BLW fields

Confirm the recipe has:

```text
Baby portion
Set aside before
Texture target
Cut or shape guidance
Allergen notes
Choking-risk flags
```

## 5. Family notes

Add only useful notes:

```text
What worked
What failed
What to change next time
Work-night suitability
Baby acceptance
Timing problems
```

## 6. Revision history

Add one concise row:

```text
YYYY-MM-DD — Created from weekly meal plan.
```

## 7. Index update

Add or update the row in `recipe-index.csv`.

## 8. Test import

After publishing:

1. Open the recipe page.
2. Use the browser recipe extension.
3. Confirm title, ingredients, and instructions imported cleanly.
4. If the import is messy, fix the page before creating more recipes.
