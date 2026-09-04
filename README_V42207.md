# KeySuite V4.22.07

Focused fix for Product > CHC/VMS C4 curve Back navigation.

- Captures the C4 Product state before opening the inline curve.
- Bottom-right Back explicitly restores Product > CHC C4 / VMS C4 and the previous model-series list.
- Restores the selected brand, CHC_G1 product group, search/filter state and scroll position.
- Does not change the working CHC C6 or End Suction Back paths.
- No Supabase database migration is required.
