# Project Vault updates

This repo holds the signed update files for Project Vault, a tool for Ableton Live producers and DJs
(finds lost samples, swaps missing plugins while keeping settings, diagnoses crashes).

- `latest.json`: the newest version, where its zip is, and its SHA-256, signed with the publisher's key
- `releases/project_vault-X.Y.Z.zip`: each version

Project Vault checks `latest.json` at most once a day and installs with `python -m project_vault update`.
It only accepts files signed with the key built into the app, so files changed by anyone else are refused.
