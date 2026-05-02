# Bulat Firefox Themes

A small collection of Firefox themes built from simple WebExtension manifests and custom theme artwork.

## Themes

| Theme | Source folder | Notes |
| --- | --- | --- |
| Dark Forest Rain Bulat Theme | `dark_forest_rain_bulat_theme_v040/` | Animated SVG header, dark forest rain palette, no scripts. |
| Southern Cross Night Bulat Theme | `southern_cross_night_bulat_theme_v010/` | Animated SVG southern night sky with a bright Southern Cross, soft rain, and forest horizon. |
| Surreal Time Desert Bulat Theme | `surreal_time_desert_bulat_theme_v010/` | Animated SVG night desert with melting clock shapes, floating stars, and warm dream shadows. |
| Impressionist Water Garden Bulat Theme | `impressionist_water_garden_bulat_theme_v010/` | Animated SVG water garden with soft dawn light, lily pads, and shimmering brushstroke reflections. |
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

This repository is licensed under the Creative Commons Attribution 4.0 International License.

You may share and adapt the theme source files and artwork, including commercially, as long as you give appropriate credit and link to the license.

See [LICENSE](LICENSE) or <https://creativecommons.org/licenses/by/4.0/>.
