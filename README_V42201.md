# KeySuite V4.22.01 Full Clean

Built from V4.21.15 Full Clean.

## Changes
- Role Brand / Series Assigned exposes CHC C4 and CHC C6 as independent assignment scopes.
- Owner can manage all user assignments, while the Owner account also follows its own Brand / Series assignment for Product and Quick Selection.
- Quick Selection without a customer uses User Assigned only.
- Quick Selection with a customer uses User Assigned ∩ Customer Brand / Series Price Preference.
- Legacy `Brand|CHC` remains backward-compatible until that user assignment is resaved. New CHC saves use `CHC_G1` and `CHC_G2` independently.
- CHC-family PDF filenames preserve the selected variant: CHC → CHC, CHCS → CHCS, CHCN → CHCN.
