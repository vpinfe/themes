# VPinFE themes

The list of frontend themes VPinFE 3.0 offers. `themes.json` is what its Themes page reads
by default.

This is the 3.0 list. VPinFE 2.x reads a different list, `superhac/vpinfe-themes`, which
stays as it is.

## An entry

```json
"revolution": {
  "url": "https://github.com/vpinfe/theme-revolution",
  "name": "Revolution",
  "default_install": true
}
```

- The key is the theme's folder name on disk and its identity. It does not change once
  listed.
- `url` is the theme's repository. VPinFE reads `manifest.json` from its default branch.
- `name` is what the Themes page shows, and nothing else. Without one, the `name` in the
  theme's `manifest.json` is used.
- `ref` pins a branch, tag or commit to read instead of the default branch.
- `default_install` is honored only in this list. It installs the theme when VPinFE starts
  and keeps it from being deleted.

A theme's version comes from its own `manifest.json`, so a new release is a commit in the
theme's repository and nothing here changes.

## Getting listed

Open a pull request adding an entry. The theme needs a `manifest.json` with `name`,
`version`, `author` and `min_vpinfe`, and a `preview_image` under about 300 KB. How a theme
is built is in the VPinFE documentation, `docs/theme-publishing.md`.
