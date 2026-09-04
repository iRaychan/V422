# KeySuite V4.22.06

Focused fix: CHC / VMS C4 Product Curve bottom-right Back button.

- One press now force-closes the inline Product curve and restores the Product model list.
- The close action no longer depends on a possibly stale `inlineOpen` runtime flag.
- All inline-curve DOM markers are cleared before the Back button is hidden.
- The Back button works again after opening another C4 curve.
- No Supabase database migration or Edge Function deployment is required.
