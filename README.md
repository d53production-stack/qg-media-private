# QG Media (private)

The images the QuantGeeks tools use: thumbnails, stills, reference images, device frames and logos. They were copied out of each claude.ai tool so the tools can get lighter and nothing lives only inside a tool. Videos are not here; they stay in the QG Media Repo and on the Mac.

[`manifest.json`](manifest.json) lists every file: where it is here, its fingerprint (sha256), its size, and the tool and link it came from. QG Full Records (`qg-records`) reads this list, so each record knows where its picture lives.

| Folder | What it holds |
|---|---|
| `publishing_desk/thumbs/` | Thumbnails the desk publishes with its page. |
| `publishing_desk/thumbs-uploaded/` | Thumbnails uploaded to the desk (A/B title and thumb variants). |
| `publishing_desk/logos/` | The logo the desk uses. |
| `copy_studio/stills/` | Stills and thumbnails uploaded to Copy Studio. |
| `black_friday_lab/refs/` | The reference board images. |
| `black_friday_lab/logos/` | The QG mark and wordmark, black and white. |
| `promo_studio/` | Device frames, logo and app screenshots that were built into the page. |
| `template_studio/` | The sample still built into the page. |

Files keep the tool's own id as their name, so a record's id leads straight to its file. The same picture can appear under two tools (Copy Studio and Black Friday Lab share some); Git stores it once.

The official logos are the ones in `qg-command` (brand reference). The copies here are what each tool was using, kept for the record.

## Rules

- Private: these include unreleased promo images.
- Add images, don't overwrite them. A new version gets a new name.
- After adding files, update `manifest.json` so Records can find them.
- No secrets, no videos.
