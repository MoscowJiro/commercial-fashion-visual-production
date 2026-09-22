# CASE B — Composition / Canvas Extension

## Problem

The approved fabric macro is square and offers limited layout flexibility for portrait placements.

## Decision

Extend the canvas vertically to 4:5 while keeping the original central fold as the visual and material anchor. Only the added outer area may be synthesized.

## AI Operation

- Outpaint plausible continuous fabric above and below the original square field.
- Preserve the diagonal fold direction, warm cream/ivory color, fiber scale, soft grazing light, and depth of field.
- Prohibit seams, objects, labels, pattern repetition, and new folds.

## Manual / QC Decision

- Output aspect ratio: PASS, portrait 4:5
- Color continuity: PASS
- Fold direction and lighting continuity: PASS
- Fabric texture continuity: PASS
- Extension boundary visibility: PASS at normal viewing scale
- Human boundary: the generated extension is acceptable for layout use, but the source macro remains the authenticity anchor.

## Final Result

**PASS.** AFTER is approved as a composition-extension demonstration; use remains limited to textile-detail layouts.
