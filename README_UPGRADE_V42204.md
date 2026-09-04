# Upgrade to KeySuite V4.22.04

Base: V4.22.03

Copy the files in this patch over the existing V4.22.03 web root.

Fixes:
- CHC C6 Product curve preserves `CHC_G2` selling-series context.
- O.K.Pump C6 continues to display VMS / VMSS / VMSN on the curve page.
- Bottom-right Product Curve Back button returns to the model list reliably.
- CHC C4 model list preserves source order; reduced-impeller variants precede the full model at the same stage.

No Supabase migration is required.
