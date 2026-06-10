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
- Oven: 900W x 900H x 600D mm, built into a tall cabinet column
- Washing machine: 600W x 1000H x 700D mm, under-counter, front-loading
- Fridge: 900W x 1800H x 700D mm, on the far end wall

## Finishes (from client's handwritten floorplan notes)

- Cabinets: HQE iron-grey scratch-resistant metallic laminate (43 HQE 耐刮金属-铁灰)
- Cabinet colour ref: 48 HQE 6214-03
- Wall tiles: 30x60cm G0712 "Bulgaria Silver"
- Floor tiles: 30x60cm QP 8324 GMB (dark graphite grey)
