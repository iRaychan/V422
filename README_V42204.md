# KeySuite V4.22.04

## Product CHC C6 selling-series context
- Product -> selling brand -> CHC C6 now preserves the `CHC_G2` product-group context when the curve opens.
- Selling Sub Series remains customer-facing on the C6 curve page (for example O.K.Pump `VMS`, `VMSS`, `VMSN`) instead of falling back to `CHC`, `CHCS`, `CHCN`.
- C4/G1 behavior remains independent and unchanged hydraulically.

## Product curve Back button
- The floating bottom-right Back button now closes the inline Product curve directly.
- It no longer hides itself before the curve has actually returned to the Product model list.

## CHC C4 model ordering
- C4 Product model lists preserve the source catalogue order instead of browser natural sorting.
- Reduced-impeller variants remain before the full-impeller model for the same stage.
- Example: `VMS 32-1`, `VMS 32-2-2`, `VMS 32-2`.

No Supabase database migration or Edge Function deployment is required.
