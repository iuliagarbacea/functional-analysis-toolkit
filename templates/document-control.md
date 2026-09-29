# Document control: [project]

> Purpose: at any moment, anyone can answer "which version is current, and what changed since the one I read".

## Conventions

- **File naming:** `[Project]_[Document]_v[N].[ext]`. Version increments on every issued change. Drafts between issues use `v[N]-draft`.
- **Current versions** live in the working folder. **Superseded versions** move to `_archive/[YYYY-MM-DD superseded]/` the day they are replaced. Nothing is deleted.
- **Inside the document:** version, date, author, status (Draft / Issued / Superseded) on the first page, and a change table at the end.
- **Cross-references** cite document + version. A reference without a version is a defect in the citing document.

## Current document set

| Document | Current version | Issued | Owner | Depends on | Referenced by |
|---|---|---|---|---|---|
| Requirements | v4 | YYYY-MM-DD | | Decision register rev. 9 | Test plan v3, RTM v2 |
| Test plan | v3 | YYYY-MM-DD | | Requirements v4 | |
| Decision register | rev. 9 | YYYY-MM-DD | | — | all |

## Change table (kept inside each document)

| Version | Date | Author | Change | Triggered by |
|---|---|---|---|---|
| v4 | YYYY-MM-DD | | §3.2 rewritten for new payment flow | D-017 |

## When a document changes

1. Bump version, update first page and change table.
2. Move the previous version to `_archive/`.
3. Update the *Current document set* table above.
4. Check every document listed under *Referenced by*. If it cites a section or number that changed, it changes too, or the drift is logged in the [coherence audit](coherence-audit.md).
