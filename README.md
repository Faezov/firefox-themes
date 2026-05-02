# Bulat Firefox Themes

A small collection of Firefox static themes built from simple WebExtension manifests and custom theme artwork.

## Themes

| Theme | Source folder | Notes |
| --- | --- | --- |
| Dark Forest Rain Bulat Theme | `dark_forest_rain_bulat_theme_v040/` | Animated SVG header, dark forest rain palette, no scripts. |
| Neon Tide | `neon-tide-theme/` | Static PNG header with neon cyan waves and bundled theme icons. |
| Neon Pixel Tide | `neon-pixel-tide/neon-pixel-tide-theme/` | Animated SVG pixel-art tide with neon particles. |
| Deep Blue | `deep-blue-theme/` | Lightweight color-only dark blue theme. |

## Privacy

These themes do not include JavaScript, permissions, remote assets, or tracking. Each public manifest declares no required data collection for AMO submissions.

## Local Install

1. Open `about:debugging#/runtime/this-firefox` in Firefox.
2. Click **Load Temporary Add-on**.
3. Select the theme folder's `manifest.json`.

## Packaging

Package from inside a theme source folder so `manifest.json` is at the root of the ZIP:

```sh
zip -r ../theme-name.zip manifest.json README.md images icons
```

For color-only themes such as Deep Blue, omit folders that do not exist.

Generated `.zip` and `.xpi` files are ignored by Git. Use GitHub Releases for published packages.

## Workbench

Experimental themes and test packages live in `.training_ground/` and are intentionally ignored for a cleaner public repository.

## License

No open-source license has been selected yet. Treat the theme artwork and source files as all rights reserved until a license is added.
