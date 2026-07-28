# {{RECIPE_TITLE}}

<p class="recipe-description">{{DESCRIPTION}}</p>

<div class="recipe-meta">
  <div class="meta-item"><span class="meta-label">Servings</span><span class="meta-value">{{SERVINGS_VISIBLE}}</span></div>
  <div class="meta-item"><span class="meta-label">Prep time</span><span class="meta-value">{{PREP_TIME_VISIBLE}}</span></div>
  <div class="meta-item"><span class="meta-label">Cook time</span><span class="meta-value">{{COOK_TIME_VISIBLE}}</span></div>
  <div class="meta-item"><span class="meta-label">Total time</span><span class="meta-value">{{TOTAL_TIME_VISIBLE}}</span></div>
</div>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Recipe",
  "name": "{{RECIPE_TITLE}}",
  "description": "{{DESCRIPTION}}",
  "recipeYield": "{{SERVINGS_SCHEMA}}",
  "prepTime": "{{PREP_TIME_ISO}}",
  "cookTime": "{{COOK_TIME_ISO}}",
  "totalTime": "{{TOTAL_TIME_ISO}}",
  "recipeCategory": "{{CATEGORY}}",
  "recipeCuisine": "{{CUISINE}}",
  "recipeIngredient": [
    "{{INGREDIENT_1}}",
    "{{INGREDIENT_2}}"
  ],
  "recipeInstructions": [
    {"@type": "HowToStep", "text": "{{INSTRUCTION_1}}"},
    {"@type": "HowToStep", "text": "{{INSTRUCTION_2}}"}
  ]
}
</script>

<div class="callout import-note">
<strong>Browser-extension import:</strong> The standard recipe is represented in the page's Recipe schema. Open this page in a browser and use the recipe import extension. Keep the BLW notes here as the family-specific reference.
</div>

## Ingredients

- {{INGREDIENT_1}}
- {{INGREDIENT_2}}

## Instructions

1. {{INSTRUCTION_1}}
2. {{INSTRUCTION_2}}

## Baby-Led Weaning Adaptation

### Baby portion

{{BABY_PORTION}}

### Set aside before

- {{SET_ASIDE_BEFORE_1}}

### Texture target

{{TEXTURE_TARGET}}

### Cut or shape guidance

- {{CUT_GUIDANCE_1}}

### Allergen notes

{{ALLERGEN_NOTES}}

### Choking-risk flags

- {{CHOKING_RISK_FLAG_1}}

## Family Notes

- {{FAMILY_NOTE_1}}

## Revision History

| Date | Change |
|---|---|
| {{DATE}} | {{REVISION_NOTE}} |
