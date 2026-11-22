# VC Bootcamp Tracker

Live progress tracker for the VC bootcamp, served via GitHub Pages.

The page reads its data directly from a public Google Sheet (tabs `config` and `milestones`) and refreshes every 30 seconds — no rebuild or redeploy is needed when the Sheet is updated.

- Sheet ID / tab gids are configured at the top of the `<script>` in `index.html` (`SPREADSHEET_ID`, `CONFIG_GID`, `MILESTONES_GID`).
- The Sheet must be shared as "Anyone with the link can view".
- Keyboard: `J` toggles Journey view, `F` toggles fullscreen. `#journey` in the URL opens Journey view directly.

## Translation

Sheet text is written once and auto-translated (Google Translate) when a viewer switches language. Some terms are kept as-is because they mistranslate (e.g. "VC" becomes "venture capital" / "CV", "trust registry" becomes a financial trust). Defaults: `VC Bootcamp`, `VC`, `VCs`, `trust registry`, `trust registries`.

To protect more terms, add a row to the `config` tab: field `keep_terms`, value pipe-separated, e.g. `BSSN|Dukcapil|Inji`. Matching is case-sensitive and whole-word.
