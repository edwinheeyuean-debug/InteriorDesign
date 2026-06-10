# InteriorDesign

Interior design project for HDB Blk 652 Senja Link, Unit 13-14 (Type B, Point Block-End).

## Rendering workflow (standing instruction)

Whenever the user asks for a render of a design and provides dimensions, always
produce **3 separate images** using the `banana` skill:

1. **Top view** — top-down plan render of the design with dimension lines and
   labels on all 4 sides (mm).
2. **Front view** — straight-on front elevation render of the design.
3. **Back view** — reverse-angle render of the design from the opposite side.

Encode every user-supplied dimension into the prompts both as absolute mm
values and as relative proportions (e.g., "the fridge stands exactly twice the
height of the washing machine") so scale reads correctly. Item dimensions are
only annotated on the top view when the user asks for them.

## Established kitchen design (current baseline)

- Kitchen: 3600mm x 3200mm, 2.6m ceiling (bottom-right of floorplan)
- WINDOWS: the kitchen's left wall has ONE window unit made of TWO casement
  panels side by side with NO gap between them (each quarter-circle arc on the
  plan = one panel). There is NO service yard. The windows must never be
  obstructed and must be rendered identically (two joined panels) in all views.
- Window wall: LOW base cabinets with worktop (900mm counter height, below the
  window sill), nothing above counter level so the windows stay clear.
- Main carpentry run along the 3.6m wall (left/window end to right): stainless
  sink, cooking hob with cooker hood above, washing machine under worktop,
  tall oven column, fridge in the corner furthest from the windows.
- Oven: 900W x 900H x 600D mm, built into a tall cabinet column
- Washing machine: 600W x 1000H x 700D mm, under-counter, front-loading
- Fridge: 900W x 1800H x 700D mm, at the end of the run away from the windows

## Kitchen logic rule (permanent)

Renders must always include functional essentials implied by the room type,
even if the user does not list them: a kitchen always has a sink, cooking
stove/hob, and cooker hood. Keep all views of a set consistent with each
other (same window count/position, same appliance arrangement).

## Finishes (from client's handwritten floorplan notes)

- Cabinets: HQE iron-grey scratch-resistant metallic laminate (43 HQE 耐刮金属-铁灰)
- Cabinet colour ref: 48 HQE 6214-03
- Wall tiles: 30x60cm G0712 "Bulgaria Silver"
- Floor tiles: 30x60cm QP 8324 GMB (dark graphite grey)
