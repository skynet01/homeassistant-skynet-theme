# Skynet Dark Theme for Home Assistant

A dark Home Assistant theme using the Skynet palette with updated support for current Home Assistant UI tokens, including modern toggles, input fields, chips, pills, entity lists, tables, and semantic color variables.

## HACS installation

1. Open HACS in Home Assistant.
2. Go to the three-dot menu and select **Custom repositories**.
3. Add this repository URL:

   ```text
   https://github.com/skynet01/homeassistant-skynet-theme
   ```

4. Select **Theme** as the category.
5. Install the theme.
6. Reload themes or restart Home Assistant.

You can also use this shortcut:

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=skynet01&repository=homeassistant-skynet-theme&category=theme)

## Home Assistant setup

Make sure themes are enabled in your Home Assistant `configuration.yaml`:

```yaml
frontend:
  themes: !include_dir_merge_named themes
```

After installation, select `skynet_dark_v2` from your Home Assistant profile theme menu.

## Manual installation

Copy `themes/skynet_dark_v2.yaml` into your Home Assistant `themes/` directory, then reload themes or restart Home Assistant.

## Notes

This theme includes optional `card-mod` styling for fan icon animation. The theme still works without `card-mod`, but those custom animations require it.

## Versioning

Releases use semantic version tags. Commits pushed to `main` run HACS validation, bump the patch version in `VERSION`, and publish a matching GitHub release.
