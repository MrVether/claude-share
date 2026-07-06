# claude-share

Ephemeral image share for Claude. Batches live under `img/<YYYYMMDD-HHMM>/` and are
served via `raw.githubusercontent.com`. Each batch has a `manifest.json` + `CREDITS.md`.

All images are downloaded from **Wikimedia Commons** and remain under their original
licenses (see each batch's `CREDITS.md` for author + license). Batches older than
6 hours are auto-removed by `clean.sh` (systemd timer, every 15 min).
