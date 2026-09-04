# KeySuite V4.22.11

- Updates CHC C4/G1 Price List model master from `010 - CHC G1 (Pricelist) - 260903 - V1.2.xlsx`.
- Price master now contains 412 models.
- Adds 22 CHC 10 price models and 17 CHC 15 price models compared with the prior V1.1 price map.
- Preserves all existing user-entered C4/G1 prices; the attached workbook's zero values are stored only as source/audit values.
- Keeps technical/hydraulic C4 data unchanged. The four V1.2 price-only rows `CHC 32-15-2`, `CHC 32-15`, `CHC 32-16-2`, and `CHC 32-16` are not promoted into the curve catalogue because the pricelist contains no C4 technical/dimension data for them.
- Product display cleanup removes internal `G1` from customer-facing C4 labels.
- O.K.Pump example now shows `Product · VMS C4`, `VMS C4 Series`, and `C4 models`; the helper text follows the selling Brand Series instead of leaking CHC/G1 naming.
- V4.22.10 generation-aware C4 curve routing/stability fixes are retained.

Supabase migration required:
- `V42211_CHC_G1_PRICELIST_V12.sql`
- `V42211_VERIFY_CHC_G1_PRICELIST_V12.sql`
