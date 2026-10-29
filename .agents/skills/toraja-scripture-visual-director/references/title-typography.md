# Indonesian title artwork — independent asset

## Intent
Title is NOT part of main illustration. It is generated/rendered after chosen concept and follows illustration palette, emotional tone, and available space. User will place manually over 4:3 and 16:9.

## Fidelity & Layout Adaptation
- Use **exact Indonesian theme title** verbatim from MD; do not translate, paraphrase or append scripture references. Toraja-language title is preserved in analysis but excluded unless requested.
- **Flexible line breaking, hierarchy, and canvas ratio**: Determine line breaks (1, 2, 3, or more lines), word hierarchy, and canvas aspect ratio based directly on title length, natural phrase rhythm, and the exact geometry of the available negative space in the master artwork. **Do not rigidly force a two-line layout**. Give visual prominence (scale/weight) to theological core words where appropriate.
- **Color & treatment derived from rendered master**: Typography color, luminance contrast, and surface treatment (e.g. warm ivory, burnished antique gold, soft parchment, or deep sepia) must be directly calibrated against the *approved and rendered master artwork*'s specific color palette, lighting temperature, and the backdrop of the negative-space zone.
- Choose one cinematic typography family for church identity, flex weight and accent by mood. Examples: elegant classic serif, restrained monumental serif, warm humanist serif; mention available real font choices only if verified on production machine. Use legal installed fonts.
- 3D/painterly treatment is **subtle**: handcrafted letterpress-like matte finish, delicate painted edge, light bevel only when beneficial; avoid illegible distress, extreme gradients, bulky extrusions, superfluous flourishes, religious clipart or exaggerated magical glow.

## Extraction options
1. **Prioritized: Transparent PNG / SVG**: Vector or real-font typography exported as a clean 32-bit PNG with alpha channel (transparent background) is the primary deliverable whenever tooling/workflows permit. This guarantees 100% exact orthography and effortless compositing across slides.
2. **Solid Pure Black (#000000) or Pure White (#FFFFFF)**: Maintained for AI text/diffusion generation models or rapid blending overlays (e.g. Screen/Multiply). The background must be 100% flat and uniform with no gradients, no texture, no shadows, and no decorative halos outside glyphs that complicate isolation.
3. Keep shadow/glow minimal and tight to glyphs, never contaminate uniform background in a way that makes removal difficult.

## Prompt template variables
TITLE_EXACT; LINE_BREAKS; DERIVED_COLOR_PALETTE; TYPOGRAPHIC_CLASS; MOOD; BACKGROUND (TRANSPARENT_ALPHA / #000000 / #FFFFFF); TYPE_TREATMENT; TEXT_ORIENTATION (horizontal); WIDTH_RELATIVE_TO_MASTER_SAFE_ZONE.

## QA
Verify every Indonesian letter, capitalization, spacing, punctuation, word sequence, line breaks, clipping and readability; text image models may fail exact orthography. If failure, switch to font/vector typography rather than repeated uncontrolled regeneration. Test compositing over BOTH 4:3 and 16:9 at realistic slide viewing size. Logo and watermark absent.
