# KeySuite V4.21.05 Upgrade

Upgrade target: V4.21.04.

Changes:
- CHC C4 / G1 Selection PDF and Product Curve PDF use the exact dimension drawings from `004 - CHC G1 260831 - V1.1.xlsx`.
- Drawing selection follows the G1 family/material mapping from the workbook (CHC versus CHCS/CHCN where separate drawings exist).
- Normal C4 Selection PDF now uses the same 409-model G1 numeric dimension table as the C4 Product engine instead of the stale G2 table.
- CHC C6 / G2 remains untouched.
- Browser/service-worker cache bumped to V4.21.05.

Deployment:
1. Replace/upload the files in this upgrade package.
2. No `supabase db push` is required.
3. No Edge Function deployment is required.
