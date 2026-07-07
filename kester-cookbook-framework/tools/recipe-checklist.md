# Recipe Finalization Checklist

Use this when turning a meal into an AnyList-importable recipe page.

## Before creating a page

1. Check `recipe-index.csv` for the recipe name, main ingredients, and tags.
2. Decide whether the recipe is:
   - already in AnyList,
   - a variation of an existing AnyList recipe,
   - or a new recipe.
3. If it is a duplicate or minor variation, do not create a new page. Update the AnyList recipe instead.
4. If it is new, create a new recipe folder and page.

## New recipe page requirements

Each page must include:

- Title
- Short description
- Servings
- Prep time
- Cook time
- Total time, if useful
- Ingredients
- Instructions
- Optional family notes
- JSON-LD Recipe schema

Do not include photos. AnyList handles photos after import.

## File naming

Use lowercase slugs with hyphens.

Example:

```text
lemon-garlic-chicken-thighs
```

Folder path:

```text
recipes/lemon-garlic-chicken-thighs/index.html
```

## After creating a page

1. Add the recipe link to the root `index.html`.
2. Add or update the row in `recipe-index.csv`.
3. Publish the site.
4. Open the recipe page.
5. Use the AnyList browser extension to import it.
6. Confirm AnyList imported:
   - title,
   - servings,
   - ingredients,
   - instructions.
7. Once imported, AnyList is authoritative.
