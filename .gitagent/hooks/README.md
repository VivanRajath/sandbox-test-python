# Hooks

Lifecycle points in a sandbox session.

- on-clone — scaffold this .gitagent spec and index the repo map.
- on-open — the knowledge-builder agent reads the repo and writes
  knowledge/overview.md, on its own API key so it never competes with chat.
- pre-edit — Guardrails check scope and protected paths before an edit is applied.
- post-edit — save the file and reload the live preview.
- on-stuck — if the app is slow to boot, the build doctor runs automatically.
