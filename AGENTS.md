# Bring Recipe Publisher

This repository is a flat, phone-friendly GitHub Pages recipe site.

## When adding a recipe

1. Read every supplied recipe image carefully.
2. Extract the title, source, yield, ingredients, directions, and useful notes.
3. Never invent missing or unreadable text.
4. Paraphrase cookbook directions while preserving quantities, temperatures,
   timings, ordering, and techniques.
5. Do not publish the photographed page itself.
6. Create one lowercase, hyphenated HTML filename at the repository root:
   `recipe-name.html`.
7. Copy the existing recipe page structure.
8. Include valid Schema.org Recipe JSON-LD with:
   - name
   - description
   - author
   - recipeYield
   - recipeIngredient
   - recipeInstructions using HowToStep objects
9. Include:
   `<script async="async" src="https://platform.getbring.com/widgets/import.js"></script>`
   and:
   `<div data-bring-import="" style="display:none"></div>`
10. Do not edit `index.html`; it discovers root-level recipe HTML files automatically.
11. Reuse `styles.css`; do not create another stylesheet.
12. Validate that every visible ingredient and instruction matches the JSON-LD.
13. Commit and push the completed change.

## Final response

Report:
- the recipe page filename
- any uncertain transcription
- the public GitHub Pages URL
- whether the commit and push succeeded
