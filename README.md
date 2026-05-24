# ToyBox3d

Shopify Horizon theme for The Toy Box 3D.

## Deploying to Shopify

The Shopify deploy app can fail with errors like:

```text
(assets/base.css) this file is not part of your theme
(templates/index.json) this file is not part of your theme
```

That means the deploy app is trying to update an existing Shopify theme record that does not already contain this full Horizon theme file set. This repository is a complete Shopify theme, so Shopify must be seeded with the full theme once before incremental deploys will work.

Recommended path:

1. In Shopify Admin, go to `Online Store > Themes`.
2. Choose `Add theme > Upload zip file`.
3. Upload `toybox3d-child-friendly-refresh.zip`.
4. Preview the uploaded theme and publish it when ready.
5. After that full theme exists in Shopify, use the deploy app/GitHub sync only for later incremental edits.

The theme source lives at the repository root in the standard Shopify folders: `assets`, `blocks`, `config`, `layout`, `locales`, `sections`, `snippets`, and `templates`.