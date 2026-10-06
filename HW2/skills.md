# Reusable HW2 procedures

## Transfer slab load to beams

1. Load the accepted HW1 slab polygon and openings from `../HW1_reference/`.
2. Define finite beam segments between adjacent structural grid points.
3. Assign each loaded slab cell to its nearest beam segment. Parallel edges divide at mid-lines; perpendicular edges divide on 45-degree bisectors.
4. Bin assigned area along each beam to retain triangular, trapezoidal, cantilever-uniform, and superposed profiles.
5. Store dead and live profiles separately. Compute an equivalent UDL only as total load divided by beam length.
6. Confirm that all beam tributary areas and loads close to the reused HW1 slab totals.

## Build and check an OpenSees model pair

1. Preserve a plain-language structural briefing before generating code.
2. Establish qL2/8 and qL2/12 moment scales and a qualitative curvature sketch before solving.
3. Model the standalone beam with continuous nodes, vertical support restraints, and free rotations.
4. Replace point supports by 3 m fixed-base elastic columns for the one-floor subframe.
5. Apply the same frozen local-negative-y load profile to both models.
6. Require reaction/load closure, sagging-positive and hogging-negative regions, and peak moments inside the pre-solve envelope.
7. Compare subframe column-top axial forces with the unchanged HW1 one-floor estimates and explain model-scope differences without tuning either result.
