# VC Bootcamp Tracker

Live progress tracker for the VC bootcamp, served via GitHub Pages.

The page reads its data directly from a public Google Sheet (tabs `config` and `milestones`) and refreshes every 30 seconds — no rebuild or redeploy is needed when the Sheet is updated.

- Sheet ID / tab gids are configured at the top of the `<script>` in `index.html` (`SPREADSHEET_ID`, `CONFIG_GID`, `MILESTONES_GID`).
- The Sheet must be shared as "Anyone with the link can view".
- Keyboard: `J` toggles Journey view, `F` toggles fullscreen. `#journey` in the URL opens Journey view directly.
