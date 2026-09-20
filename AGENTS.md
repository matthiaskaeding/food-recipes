# food-recipes

A personal cookbook of recipes saved as clean Markdown.

## Recipe workflow

When the user pastes a recipe URL, use the
[convert-recipe skill](.agents/skills/convert-recipe/SKILL.md). It contains the
extraction rules, recipe template, and metric conversion table.

1. Convert each recipe and save it as `<folder>/<slug>.md`.
2. Add each recipe to its section in `README.md`, alphabetically.
3. Commit as `Add <recipe name>` and push to `main`.

Proceed without asking for confirmation within the user's authorization and
available permissions. For several URLs, save one file per recipe and make one
commit for the batch.

For recipe conversions, report just the filename and a one-line note if the
source was ambiguous, such as an unclear quantity, missing time, or vague step.

## Folders and filenames

Recipes live in folders by type at the repository root, with no `recipes/`
wrapper folder.

- `mealprep/` contains general recipes and is the default.
- `baby/` contains baby and toddler food.

Choose the folder based on the recipe. Create a new folder if none fits.

Use kebab-case slugs without articles or source names, such as
`miso-glazed-aubergine.md`.

## Repository conventions

- Keep the recipe index in `README.md`.
- Commit directly to `main`. Do not create branches or pull requests.
