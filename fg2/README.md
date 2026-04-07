# FG2 Inspection Packet

This folder packages the current Form Gallery sandbox Atrium/gallery pass for external inspection.

## Scope

This packet captures the recent sandbox work that:

- converts the Atrium homepage from a full inline gallery dump into summary gallery cards
- adds dedicated gallery routes under `museum/galleries/`
- moves full work grids to gallery pages
- refreshes route-shell asset tokens so the shared CSS/JS changes load consistently

## Included files

- [museum/shared/lobby.js](./museum/shared/lobby.js)
- [museum/shared/page.js](./museum/shared/page.js)
- [museum/shared/museum.css](./museum/shared/museum.css)
- [museum/index.html](./museum/index.html)
- [museum/tour/index.html](./museum/tour/index.html)
- [museum/galleries/](./museum/galleries/)
- [COMMITS.txt](./COMMITS.txt)
- [atrium-gallery-pass.patch](./atrium-gallery-pass.patch)

## Commit references from the sandbox branch

- `2ea1207` — `Add dedicated gallery pages to the atrium`
- `92c5ffa` — `Refresh museum route shells for shared asset changes`
- `57fb483` — `Add fg2 inspection handoff`

## Verification summary

- `/museum/` renders `13` summary gallery cards and `0` inline work cards in the latest sandbox pass.
- `/museum/galleries/egypt-mesopotamia/` renders `12` work cards on the dedicated gallery page.
- `node --check` passed for the copied `lobby.js` and `page.js`.

## Notes

- This is an inspection package only.
- It does not modify the production repo or live deployment.
- The authoritative working branch for this pass is `codex/thumbnail-grid-refinement` in the sandbox repository.
