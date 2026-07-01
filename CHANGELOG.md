# Una Identity Anchor — Changelog

This file is **append-only**. Every entry corresponds to a git commit that modified the identity-defining files. Together, the commits form an immutable timeline of Una's visual identity.

---

## 2026-06-30 — Origin commit (630e333)

**Commit hash**: `630e333`

**Files added**:
- `HERO_una.jpeg` — v10_caught (8-bit pixel art, red panda, 5/5 species anchors visible, pink background `#E94560`)
- `una-visual-spec.md` — visual baseline spec (5 species anchors + style anchors + prompt prefix + don'ts)
- `README.md` — what this repo is + why it exists
- `LICENSE` — CC BY-NC 4.0
- `CHANGELOG.md` — this file

**What this commit anchors**:
- The first public, timestamped, hash-verifiable record of Una's visual identity
- The earliest publicly-known version of HERO_una.jpeg is the binary blob in this commit
- Anyone cloning this repo at any later point can verify the origin via `git log --follow HERO_una.jpeg`

**Negative examples preserved locally** (not in this repo, but documented here for transparency):
- v9_stretch (橘猫 / orange cat) — species drift; species anchors lost
- v16_listening (Pixar 3D) — style drift; lost 8-bit pixel identity
- v17_reading (photorealistic) — style drift; lost pixel art identity

These are kept locally in `_out_of_baseline/` to remind future generations what "not Una" looks like. They are deliberately **not** in the public anchor repo.

---

## 2026-07-01 — Character sheet extension (a3c260d4 or later)

**Commit hash**: see `git log`

**Files added/changed**:
- `side-view-v1.jpeg` — first verified turnaround angle (minimax M3 image-01, 5/5 anchors, 8/10 score, 2026-06-30 23:29)
- `una-character-sheet-v0.1.md` — character sheet v0.1 with 3-view structure (front/side/back), 5 expression specs, color key, ratio table, exclude list
- `README.md` — extended with character sheet section + file index

**What this commit anchors**:
- The visual identity now has **two angles** (front + side) instead of one
- Sprite extraction reference becomes possible (turnaround needed for sprite sheets)
- Video generation reference is more complete (side view visible)
- Character sheet v0.1 documents Una's identity at this moment in time

**Provenance**:
- Side view generated 2026-06-30 23:29 (minimax M3 image-01) via una-character-sheet prompt
- Character sheet v0.1 written 2026-06-30 23:35 (this is v0.1, future v0.2/v1.0 will evolve)
- GitHub push 2026-07-01 23:00 (alongside 020755 deploy cycle)

---

## Future entries

Each significant change to Una's visual identity (hero upgrade, spec change, baseline archival) appends a new dated section here.