# KeySuite V4.21.01 Upgrade

Base: KeySuite V4.21 FULL CLEAN.

## CHC G1 hydraulic / curve
- Adds CHC G1 as its own hydraulic generation using `004 - CHC G1 260831 - V1.1.xlsx`.
- CHC G1 Selection, Quick Selection, Product Curve and PDF follow the CHC G2 format/engine.
- G1 technical master: 18 hydraulic families / 409 models.
- `CHC 32-11-2` and `CHC 32-11` are fixed at 11 stages.
- CHC 200 uses numeric impeller suffix naming.

## CHC G1 price-model master
- Source: `010 - CHC G1 (Pricelist) - 260831 - V1.1.xlsx`.
- Exact price model master: 373 models.
- CHC 200 price models are reconciled to the numeric hydraulic names without overwriting entered prices.
- The old separate `CHC 5-5 (60Hz)` price row is removed. The normal `CHC 5-6` remains, matching the V1.1 attachment.

## Supabase
Run the included migration after copying the patch:

`supabase/migrations/V42101_CHC_G1_HYDRAULIC_MODEL_NAMES.sql`

The migration is safe to rerun and preserves existing G1 price values while renaming/synchronizing the model identifiers.

No Edge Function deployment is required for this update.
