# Rookie Legends — Shopify theme

Source for the live theme on rookielegends.com: Shopify's **Savor 3.4.0**, plus custom sections and GemPages templates. It was exported from the store on 30 Sep 2026 (`rookielegends-com-official-4-0`).

## Connect this repo to the store

1. In Shopify admin, go to **Online Store → Themes**.
2. Click **Add theme → Connect from GitHub**, then authorize the Shopify GitHub app for `matthewhammerx/Rookie-Legends`.
3. Pick this repository and the branch that holds the theme. The theme appears in your theme library.
4. **Preview** it and check it. Then click **Publish** when you want it live.

The sync works both ways:

- A commit pushed to the connected branch updates the theme in Shopify.
- A change made in the theme editor (**Customize**) is committed back to the branch by Shopify.

To test risky changes, connect a second branch as a separate, unpublished theme.

## Local development (optional)

```sh
npm install -g @shopify/cli
shopify theme dev --store <your-store>.myshopify.com # live preview with hot reload
shopify theme check                                      # lint Liquid/JSON
```

## Layout

| Folder | What's in it |
| --- | --- |
| `layout/` | Page shells (`theme.liquid`, password page, GemPages layouts) |
| `templates/` | JSON templates per page type, including the custom product/collection/page templates |
| `sections/`, `blocks/`, `snippets/` | Building blocks used by the templates |
| `assets/` | CSS, JS, images, fonts |
| `config/` | Theme settings schema and saved settings (`settings_data.json`) |
| `locales/` | Translations |
