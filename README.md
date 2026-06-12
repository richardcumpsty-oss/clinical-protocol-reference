# Clinical Protocol Reference - Individual Protocol Pack v0.5

This pack is designed for a Lovable/GitHub PWA where each protocol is its own replaceable PDF.

## Key idea
- The app UI is driven by `data/protocol-index.json`.
- Each protocol card links to one PDF file under `docs/`.
- To update a protocol, replace only that PDF and update its index entry/version/date.

## Example: adding or replacing burns
Replace:
`docs/trauma/burns.pdf`

Or add a new file:
`docs/trauma/burns-rule-of-10s.pdf`

Then update `data/protocol-index.json` and `data/changelog.json`.

## Safety notice
Reference only. Use within training, authorisation and supervision. Does not replace clinical judgement, source protocols, reachback, local policy, command direction or evacuation.

## Recommended Lovable prompt
Build a mobile-first password-protected PWA called "Clinical Protocol Reference". Use `data/protocol-index.json` as the source of truth. Do not hard-code the protocol list. Generate category pages, search results and protocol cards from the JSON. Each card should show title, category, section, version, last updated, status, tags, and buttons to open/download the linked PDF. Do not rewrite or summarise clinical content. The app is a reference viewer only.
