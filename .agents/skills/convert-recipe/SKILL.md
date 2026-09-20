---
name: convert-recipe
description: Convert recipe URLs into clean Markdown recipes with metric cup conversions. Use when the user supplies one or more recipe links to save in this cookbook or asks to convert a recipe into its format.
---

# Convert a recipe

Fetch each supplied recipe page and extract its ingredients, method, servings,
and times. Follow the repository's AGENTS.md for file locations, slugs, the
recipe index, and Git conventions. Save one file per recipe.

## Extract the recipe

Use the recipe card for quantities and read the surrounding text for useful
technique details, substitutions, and storage instructions. Retain quantities,
temperatures, times, pan sizes, and details that affect the outcome.

Remove personal stories, travel anecdotes, promotional claims, advertisements,
newsletter pitches, affiliate copy, SEO padding, photo captions, unnecessary
equipment lists, and reader comments.

Rewrite the method in your own words. Preserve the source's quantities and times,
apart from the unit conversions below. Do not invent missing quantities or times.
Distinguish preparation time from extra chilling, resting, or advance cooking
when the source gives those separately. If the source is ambiguous, mention it
briefly when reporting the saved filename.

## Recipe format

```markdown
# Recipe Name

Source: <url>
Serves 4 · 25 min

## Ingredients

- 120 g (1 cup) flour
- 2 tbsp olive oil

## Method

1. First step.
2. Second step.

## Notes

Include only useful substitutions, preparation or storage windows, and technique
notes that help the reader avoid a mistake.
```

- Always include the source URL.
- Keep servings and time on one line. Omit either if the source does not give it.
- List ingredients in the order used. Use level-three subheadings only for
  distinct components, such as a dressing or dough.
- Number method steps, with related actions together and no more than three
  sentences per step.
- Omit the Notes section when there is nothing useful to add.

## Metric conversions

Convert every cup measurement to grams for dry ingredients and produce, or
millilitres for liquids. Keep the original cup amount in parentheses, such as
`120 g (1 cup) flour` or `240 ml (1 cup) milk`. Leave tsp and tbsp unchanged.

Use metric quantities supplied by the source when available. Otherwise use the
table below, scaling it for the stated cup amount. Match the ingredient's state,
such as dry, cooked, chopped, or packed. For an ingredient not covered here,
check an ingredient-specific conversion instead of using a liquid volume as a
weight.

The table uses 240 ml per cup. Weights are approximate because density and how
an ingredient is chopped or packed can vary.

### Liquids (by volume)

| Cup     | ml  |
| ------- | --- |
| 1 cup   | 240 |
| ¾ cup   | 180 |
| ⅔ cup   | 160 |
| ½ cup   | 120 |
| ⅓ cup   | 80  |
| ¼ cup   | 60  |
| ⅛ cup   | 30  |

### Baking staples

| Ingredient        | 1 cup |
| ----------------- | ----- |
| Flour (all-purpose) | 120 g |
| Sugar (granulated)  | 200 g |
| Butter              | 227 g |

### Dry grains and legumes

| Ingredient          | 1 cup |
| ------------------- | ----- |
| Quinoa (dry)         | 170 g |
| Lentils (dry)        | 200 g |
| Orzo pasta (dry)     | 200 g |
| Pearl couscous (dry) | 115 g |

### Produce and other

| Ingredient                     | 1 cup |
| ------------------------------- | ----- |
| Chopped tomato                  | 180 g |
| Diced onion                     | 160 g |
| Diced cucumber                  | 120 g |
| Cherry tomatoes, halved         | 150 g |
| Chickpeas, cooked               | 165 g |
| Olives, pitted                  | 150 g |
| Feta cheese, crumbled           | 150 g |
| Baby spinach, loosely packed    | 30 g  |
| Kale, chopped and packed        | 65 g  |
| Cilantro, packed                | 15 g  |
| Fresh herbs, chopped (loose)    | 30 g  |
| Nuts, chopped                   | 120 g |
| Raisins                         | 165 g |
| Pepitas                         | 140 g |
| Brussels sprouts, halved        | 88 g  |
