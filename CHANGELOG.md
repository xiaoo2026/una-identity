# Una Identity Anchor — Changelog

This file is **append-only**. Every entry corresponds to a git commit that modified the identity-defining files. Together, the commits form an immutable timeline of Una's visual identity.

---

## 2026-06-30 — Origin commit

**Commit hash**: see `git log` (this commit)

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

## Future entries

Each significant change to Una's visual identity (hero upgrade, spec change, baseline archival) appends a new dated section here.