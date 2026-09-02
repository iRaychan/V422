# KeySuite V4.21.14

## CHC C4 / G1 pricing handoff

- Normal CHC C4 Selection now explicitly sends `generation_code = G1`.
- It also sends `keysuite_generation_code = G1`, `keysuite_product_group_code = CHC_G1`, and `keysuite_price_group_code = CHC_G1`.
- KeySuite normalizes CHC generation before Assembly/Quotation pricing, so an older cached C4 selector cannot silently fall back to C6/G2.
- C6/G2 selector payloads are also explicit for symmetry.

## KeyBot PDF motor efficiency

- CHC C4/G1 KeyBot PDF motor row now displays `IE2` instead of the previously hard-coded `IE3`.
- The actual IE2 motor lookup remains unchanged (for example `2BM3-2`).
- CHC C6/G2 continues to display `IE3`.

## KeyPLC SQL correction

- Corrects the V4.21.13 3kW / 37kW seed SQL to supply the required text `id` using the existing `KEYPLC-xxxx` convention.
- Existing KeyPLC rows and prices are preserved.

## Deployment

1. Upload the web files from this build.
2. Redeploy `telegram-webhook` for the KeyBot PDF IE2 label correction.
3. No new V4.21.14 database migration is required if the 3kW and 37kW KeyPLC rows are already present. The corrected V4.21.13 SQL is included for fresh/unapplied installs.
