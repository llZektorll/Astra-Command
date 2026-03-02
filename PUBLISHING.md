# Publishing Guide

## Current Repository Model

This repository is a multi-variant theme collection. Each theme lives in its own standalone package:

- [`themes/Astra Command Blue`](./themes/Astra%20Command%20Blue)
- [`themes/Astra Command Green`](./themes/Astra%20Command%20Green)
- [`themes/Astra Command Titanium`](./themes/Astra%20Command%20Titanium)

Each package already contains the two essential files required for manual installation:

- `manifest.json`
- `theme.css`

## Community Theme Submission Requirements

Before submission, make sure the published repository for the selected variant includes:

1. `README.md` at the repository root.
2. A screenshot image at the repository root or a stable path in the repo.
3. `theme.css` at the repository root.
4. `manifest.json` at the repository root.
5. A license.

## Recommended Release Model

For Obsidian Community Themes, publish one variant per repository or one variant per release-ready root branch.

Recommended mapping:

- `Astra Command Blue` -> standalone repo or branch with Blue files at root
- `Astra Command Green` -> standalone repo or branch with Green files at root
- `Astra Command Titanium` -> standalone repo or branch with Titanium files at root

## Root Layout For Submission

When preparing one variant for release, the repository root should look like this:

```text
README.md
LICENSE
manifest.json
theme.css
screenshot.png
```

## Submission Checklist

1. Pick the variant to publish.
2. Copy `manifest.json` and `theme.css` from that variant folder to the repository root of the public release repo.
3. Use the matching preview image from [`assets/previews/`](./assets/previews) as the screenshot base, or replace it with a fresh in-app screenshot.
4. Confirm the `name`, `version`, `author`, and `authorUrl` in `manifest.json`.
5. Tag the release with the same version as the manifest.
6. Submit the theme entry to Obsidian's community theme list.

## Suggested Community Theme Entry

### Astra Command Blue

```json
{
  "name": "Astra Command Blue",
  "author": "llZektorll",
  "repo": "llZektorll/astral-command-blue",
  "screenshot": "screenshot-blue.png",
  "modes": ["dark", "light"],
  "branch": "main"
}
```

### Astra Command Green

```json
{
  "name": "Astra Command Green",
  "author": "llZektorll",
  "repo": "llZektorll/astral-command-green",
  "screenshot": "screenshot-green.png",
  "modes": ["dark", "light"],
  "branch": "main"
}
```

### Astra Command Titanium

```json
{
  "name": "Astra Command Titanium",
  "author": "llZektorll",
  "repo": "llZektorll/astral-command-titanium",
  "screenshot": "screenshot-titanium.png",
  "modes": ["dark", "light"],
  "branch": "main"
}
```

## Sources Used For This Packaging Guide

- Official sample theme template: https://github.com/obsidianmd/obsidian-sample-theme
- Official theme migration guide: https://obsidian.md/blog/1-0-theme-migration-guide/
- Community theme store submission guide: https://publish.obsidian.md/hub/04%20-%20Guides%2C%20Workflows%2C%20%26%20Courses/Guides/How%20to%20add%20your%20theme%20to%20the%20community%20theme%20store

