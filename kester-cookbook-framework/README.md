# Kester Family Cookbook Import Bridge

This repository publishes simple recipe web pages for importing recipes into AnyList with the browser extension.

## Project boundaries

- AnyList is the master recipe archive.
- This site is only an import bridge.
- Recipe pages exist to make AnyList import cleaner and reduce manual recipe pasting.
- Do not add features unless they directly improve recipe import or reduce recipe-entry friction.

## Basic workflow

1. Finalize a recipe in ChatGPT.
2. Check `tools/recipe-index.csv` for duplicates or similar recipes.
3. If the recipe is new, create a new folder under `recipes/`.
4. Copy `templates/recipe-template.html` into that folder as `index.html`.
5. Fill in the visible recipe and the JSON-LD Recipe schema.
6. Add the recipe to `index.html`.
7. Add or update the row in `tools/recipe-index.csv`.
8. Publish the site.
9. Open the recipe page and import it into AnyList with the browser extension.
10. After import, AnyList is authoritative.

## Folder structure

```text
cookbook/
  README.md
  CNAME
  index.html
  styles.css
  recipes/
    example-recipe/
      index.html
  templates/
    recipe-template.html
  tools/
    recipe-checklist.md
    recipe-index.csv
```

## Custom domain

Edit `CNAME` if this repository is served directly by GitHub Pages using a custom domain.

If this folder is being added under an existing website as `/cookbook/`, you may not need `CNAME`.

## Recipe page standard

Each recipe page should include:

- Recipe title
- Short description
- Servings
- Prep time
- Cook time
- Total time, if useful
- Ingredients
- Instructions
- Optional family notes
- JSON-LD using `@type: Recipe`

Do not include photos in this bridge. Add photos in AnyList after import.
