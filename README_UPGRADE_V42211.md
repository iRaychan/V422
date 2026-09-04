# Upgrade to KeySuite V4.22.11

Apply over V4.22.10.

This release updates the CHC C4/G1 Price List model master to `010 - CHC G1 (Pricelist) - 260903 - V1.2.xlsx` and cleans up the remaining customer-facing C4/G1 labels.

Supabase migration is required. From the upgraded project run `npx supabase db push` so these migrations are applied:
- `V42211_CHC_G1_PRICELIST_V12.sql`
- `V42211_VERIFY_CHC_G1_PRICELIST_V12.sql`

The migration does not overwrite existing user-entered C4/G1 prices.
