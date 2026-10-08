---
name: character-refinement-3d
description: Audit and refine 2D character concept sheets (AI-generated or hand-made) into consistent, 3D-modelling-ready turnarounds for a painterly, Monet-inspired side-scrolling 3D platformer. Use when a character is "close but off", reads as AI-made, has proportion or construction inconsistencies, or needs to be prepared as Blender reference.
---

# Character refinement for Blender (painterly 3D platformer)

## Goal
Turn a loose concept sheet into a **locked design** a modeller can build from:
one silhouette, one proportion system, one set of construction rules, and a
painterly look that comes from *deliberate* brushwork, not noise.

## Workflow

### 1. Audit (always first, always written down)
Review the sheet against the checklist below. Output a table:
`issue | where (view) | severity | fix`.

- **Proportions**: head:body ratio, leg length, hand/paw size, ear size and
  placement, tail thickness. Measure in head-units and keep the same across
  every view.
- **Cross-view consistency**: scar side, marking placement, scarf knot, strap
  path, weapon position. A mark on the character's left stays on the left;
  it must not appear on both sides in the side views.
- **Construction**: how the scarf wraps, where the strap crosses the chest,
  how the weapon is sheathed. Every prop must be physically plausible and
  readable at platformer scale.
- **Anatomy**: paw toes/pads, joint placement, how limbs attach in the action
  poses (running, all-fours).
- **"AI tells"**: noisy fuzzy edges with no brush logic, pixel/brick-like
  pattern marks, blobby hands, props that morph between views, decorative
  detail with no function.

### 2. Lock the design (decide, don't hedge)
Produce a short design brief:
- Silhouette: 3 shapes max (e.g. big round head, tapered body, plume tail).
- Proportion sheet: head-unit grid, side-by-side height chart.
- Prop spec: one weapon, one sheath, one strap path, drawn as simple
  orthographic views.
- Marking map: scar, cheek stripes, belly patch, drawn on a flat 2D UV-style
  layout.
- Palette: 5-7 painted colour families (see step 3).

### 3. Painterly style for 3D (Monet logic)
- Colour carries form: warm light, cool shadow, broken colour side by side.
  Avoid greying shadows; push them toward violet/blue.
- Edges: soft where forms turn away, crisp only at focal points (eyes, blade).
- Large readable brush shapes (stroke direction follows form) instead of
  uniform fur fuzz.
- In Blender: hand-painted albedo, no PBR gloss, subtle toon or stepped
  shading, painted-stroke normal/bump overlay, optional screen-space
  brush-texture pass. Keep the silhouette clean so it reads against
  busy impressionist backgrounds.

### 4. Platformer readability checks
- Reads at ~128 px tall. Squint test: silhouette still says "cat samurai".
- Side-on view is the hero angle; design the side view first.
- Distinct contrast against both light and dark backgrounds (scarf as the
  colour accent).

### 5. Deliverables (Blender-ready)
1. Orthographic turnaround: front, back, left, right, 3/4, aligned on shared
   horizontal guide lines (top of head, shoulder, hip, knee, ground).
2. Proportion/height sheet in head-units.
3. Prop and costume breakdown (weapon, sheath, strap, scarf).
4. Expression sheet (neutral, angry, sad) on one fixed head shape.
5. Key pose sheet (run, jump, attack, idle) with rig notes: joint locations,
   scarf/tail as secondary-motion chains.
6. Texture/palette reference with marking map.
7. Blender notes: base-mesh topology hints, rig/bone list, shader setup.

## Rules
- Fix the design in 2D before any modelling. Don't carry ambiguity into 3D.
- Change one thing at a time when regenerating; keep a change log.
- Prefer simple, consistent shapes over added detail.
- Never invent a new character; refine the one provided.
