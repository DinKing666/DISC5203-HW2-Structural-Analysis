# HW2 project guidance

- Treat `assignment/`, `assets/`, and everything under `../HW1_reference/` as immutable source/reference material.
- Reuse `../HW1_reference/config/plan1_geometry.json`; do not re-derive the HW1 outline, openings, columns, walls, or vertical-element tributary areas.
- Read slab load across to the 24 finite beam segments using nearest-edge distance. Equal distance to perpendicular edges is the required 45-degree bisector.
- Store the exact dead/live line-load profiles in `output/results/hw2_beam_profiles.json`. Label tabulated UDLs as equivalent by total load only.
- Use kN, m, kN/m and kN/m2. Enter E in kN/m2 and I in m4 in OpenSees.
- Freeze load profiles before running the four models. Do not tune loads to force agreement with HW1.
- Run `python scripts/verify_hw2_outputs.py` before committing or uploading.
