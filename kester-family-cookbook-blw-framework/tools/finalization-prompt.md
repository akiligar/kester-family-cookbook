# Finalization Prompt

Use this prompt in ChatGPT when a recipe is ready to become permanent.

```text
Finalize this meal as a Kester Family Cookbook recipe page.

Constraints:
- The cookbook page is the complete family recipe record.
- Include Baby-Led Weaning adaptation fields.
- Include a clean standard recipe suitable for browser-extension import.
- Include JSON-LD Recipe schema.
- Do not include photos.
- Do not add automation, sync, search, database, ratings, nutrition, or extra architecture.
- Check whether this is new, a duplicate, or a variation before creating the page.

Output:
1. Duplicate/variation assessment.
2. Recipe slug.
3. Full `index.html` file for the recipe folder.
4. Updated line for `tools/recipe-index.csv`.
5. Updated `<li>` line for the main `index.html`.
```
