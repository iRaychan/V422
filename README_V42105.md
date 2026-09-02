# KeySuite V4.21.05

- CHC C4 / G1 PDF Dimension page now uses the exact dimension drawings embedded in `004 - CHC G1 260831 - V1.1.xlsx` (CHC Dimension sheet).
- G1 drawing selection follows both hydraulic family and material variant: CHC cast-iron connection versus CHCS/CHCN stainless variants where the workbook provides separate drawings.
- Normal CHC C4 Selection PDF now also uses the 409-model G1 numeric dimension table; the stale copied G2 dimension table has been removed from the G1 selector export path.
- CHC C6 / G2 dimension drawings and values are untouched.
- PDF page layout, font, spacing and G2-style formatting remain unchanged.
- Browser/service-worker cache key bumped to V4.21.05.
- No Supabase database migration or Edge Function deployment is required for V4.21.05.
