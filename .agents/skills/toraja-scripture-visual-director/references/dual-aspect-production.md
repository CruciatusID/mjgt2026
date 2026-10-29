# 4:3 master → 16:9 extension specification

## Geometry
For identical heights H, 4:3 width W4=4H/3, 16:9 width W16=16H/9. Symmetric extension adds `(W16-W4)/2 = 2H/9` to **each** side. The 4:3 master occupies the **middle 75% of total 16:9 width** (since 4/3 divided by 16/9 = .75). Each expendable wing is 12.5% of final width. At 1152px high: master 1536×1152, final 2048×1152, +256px left and right.

## First image rules
- Compose master 4:3 as fully complete stand-alone frame, ideally leave title-negative-space *inside* 4:3. Title-safe area should be purpose-built (calm background, sufficient size/contrast), not empty white void by default.
- Make critical subject and gestures **interior to master** with margin; don't cut an essential face, object, or narrative gesture at master edge. Reserve default 5–8% inward safety from all edges for critical details (adjust explicitly if needed).
- Choose title on left/right/top based on scene, not automatically on left. Reserve enough negative space for the actual Indonesian title length. Do not put title in image itself.
- Ensure 4:3 alone still communicates theological thesis.

## Outpaint rules
- **Canvas expansion with locked master is mandatory**: Extend canvas horizontally to 16:9 while locking the original 4:3 master centrally (middle 75% width).
- Preserve exact master content, camera framing, lighting, brush texture, color temperature, perspective, and subject identities without alteration.
- Add only a physically continuous extension of horizon, clouds, foliage, wall, sky, farmland, vineyard, etc. **Do not add any meaningful person/object/symbol exclusive to wings**.
- Do not reframe, zoom, shift, or shrink the original 4:3 master.
- **Handling tool limitations & honesty**: If the generation tool does not support native pixel-locked canvas expansion/in-painting and performs partial or full resynthesis, perform a strict visual integrity QA comparison against the original 4:3 master. **NEVER claim pixel preservation if the central master was regenerated or re-sampled**. Report the exact technical behavior honestly.
- Expansion can be asymmetric only if precisely defined as a crop rectangle and both final deliverables have been validated.

## QA
- Crop centered 16:9 to 4:3 (middle 75% width) and compare with original. Confirm main content, title safe zone, emotion and visual meaning all survive. If any loss or distortion, fail.
- Audit for tool-induced artifacts: confirm no visible seam, repeated objects, inconsistent architectural geometry, painterly texture mismatch, changed horizon/perspective, new disconnected narrative elements, or scale discontinuities.
- Verify whether the master was genuinely pixel-locked or regenerated; state actual integrity test results clearly without false claims.
- File or pixel dimensions may need minor rounding for actual generators; use precise ratio and nearest supported sizes. Never stretch the original.
