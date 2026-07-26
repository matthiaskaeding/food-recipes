# food-recipes

A personal cookbook of recipes saved as clean markdown, stripped of everything
that makes recipe websites unpleasant to read.

## The workflow

When I paste a recipe URL, do all of this without asking for confirmation:

1. Fetch the page.
2. Extract the recipe, discarding the fluff (see below).
3. Decide which folder it belongs in (see Folders below) and write
   `<folder>/<slug>.md` using the template below.
4. Add a line for it to the index in `README.md`, alphabetically.
5. Commit as `Add <recipe name>` and push to `main`.

Report back with just the filename and a one-line note if anything about the
source was ambiguous (unclear quantities, missing times, vague step). Don't
summarize what you did.

If I paste several URLs at once, one file per recipe, one commit for the batch.

## Folders

Recipes are organized into folders by type, at the repo root (no `recipes/`
wrapper folder):

- `mealprep/` — general recipes, the default for most things.
- `baby/` — baby and toddler food.

Decide which folder a new recipe belongs in based on what it actually is.
If none of the existing folders fit, create a new one rather than forcing it
into the wrong place.

## Slugs

Kebab-case, no articles, no source name: `miso-glazed-aubergine.md`,
not `the-best-ever-miso-aubergine-from-food-blog.md`.

## File template

```markdown
# Recipe Name

Source: <url>
Serves 4 · 25 min

## Ingredients

- 400 g flour
- 2 tbsp olive oil

## Method

1. First step.
2. Second step.

## Notes

Only if the source has something genuinely useful: a substitution that matters,
a make-ahead window, a step that's easy to get wrong.
```

Rules for the template:

- `Serves` and time on one line. Omit either if the source doesn't say — don't guess.
- Ingredients in the order they're used, grouped under `###` subheadings only if
  the recipe has real components (a sauce, a dough, a topping).
- Method steps are numbered, one action-cluster each. No step longer than three
  sentences.
- Always convert cup measurements to metric: grams for dry ingredients, millilitres
  for liquids. Keep the original cup amount in brackets, e.g. `250 g (1 cup) flour`,
  `240 ml (1 cup) milk`. Leave spoon measures (tsp, tbsp) alone.
- `Source:` line is never omitted.

## What counts as fluff

Cut: the author's childhood, the trip to Italy, why this recipe is the best on
the internet, "jump to recipe", ad copy, newsletter pitches, affiliate blurbs,
comment-section anecdotes, SEO padding, photo captions, equipment nobody needs.

Keep: quantities, temperatures, times, pan sizes, and any technique detail that
changes the outcome.

Write the method steps in your own words rather than copying the author's prose.
Quantities and times are facts and come over as-is.

## Repo conventions

- Recipes live in per-type folders at the repo root (see Folders above), not
  in a single `recipes/` directory.
- `README.md` holds the index and nothing else.
- Commit straight to `main`. No branches, no PRs.
