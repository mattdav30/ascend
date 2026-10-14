# ASCEND | Phase 2 character production

Approved character specification: original stylised action-RPG hunter, close likeness to owner reference photos, permanent rounded glasses, evolving physique, seven visual ranks (0–6), four existing classes (berserker/ranger/paladin/monk).

## Production gates

1. Base appearance: approved likeness, detailed mesh sculpt, hairstyle and glasses, layered dark hunter clothing. Production asset in GLB/glTF format.
2. Rig and skinning: articulated humanoid skeleton, smooth deformation, coat and hair secondary motion.
3. Appearance progression: existing rank index 0–6 controls seven distinct outfits and evolving physique. Rank data must come from the existing heroCfg() hook, not a new progression system.
4. Equipment: modular class-specific gear from the four approved concept designs.
5. Animation: idle, breathing, inspect, celebrate, level-up, power-up.
6. Browser acceptance: model loads in Ascend, rotations and class and rank changes respond, fallback on loading failures, performance reviewed on desktop and mobile.

## Strict scope and integration contract

Only character 3D assets and the Hero3D renderer section inside index.html may change. Do not touch workouts, quests, levelling formulas, rank thresholds, nutrition, persistence, accounts, tab navigation or non-character UI. Preserve Hero3D.init(), .set(), .active(), .celebrate() and avatar customisation fields. Build as a draft PR, do not merge until visually tested.

## Current status

First mesh construction pass produced a separately downloadable GLB proof-of-work, not yet uploaded into the repository. It is not yet rigged, skin-weighted, animated or production quality. No main-branch application logic has been changed.
