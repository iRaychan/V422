# KeySuite V4.22.03

## Product curve Selling Sub Series fix

- Product curve pages now keep the selected **Selling Sub Series** instead of falling back to the base hydraulic series.
- Example for O.K.Pump:
  - CHC -> VMS
  - CHCS -> VMSS
  - CHCN -> VMSN
- The base CHC / CHCS / CHCN identity remains internal for hydraulic, technical, dimension and pricing lookups.
- Product Brand Context is now routed to the Product selector iframe, not the normal Selection iframe.
- Explicit Product-frame presentation refresh is allowed while the iframe is hidden so the selling identity is applied before the first visible curve render.
- Existing first-open Selling Brand logo behavior from V4.22.02 is retained.

No Supabase database migration or Edge Function deployment is required for this release.
