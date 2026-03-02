# Contributing

## Scope

This repository contains three Obsidian theme variants:

- `Astra Command Blue`
- `Astra Command Green`
- `Astra Command Titanium`

Keep each variant visually distinct and internally consistent.

## Workflow

1. Work inside the relevant folder under [`themes/`](./themes).
2. Update `theme.css` and `manifest.json` together when versioning a variant.
3. Refresh the matching preview in [`assets/previews/`](./assets/previews).
4. Document the change in [`CHANGELOG.md`](./CHANGELOG.md).

## Style Rules

- Use ASCII unless a file already requires otherwise.
- Preserve the theme identity of each variant.
- Do not collapse the three variants into minor color swaps.
- Keep `theme.css` and `manifest.json` installable as a standalone Obsidian theme package.

## Release Rule

Each variant should be releasable on its own. If a change only affects one variant, only bump that variant's version.

