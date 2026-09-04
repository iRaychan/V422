# KeySuite V4.22.02

## Fixes

- Customer-facing CHC model names now render from the assigned **Selling Sub Series** on the first render.
  - Example: O.K.Pump base/hydraulic `CHC 10-30` displays and prints as `VMS 10-30` when Selling Sub Series is `VMS`.
- Base/hydraulic CHC identity remains internal for curve, technical, dimension and pricing lookup.
- CHC C4 and CHC C6 selector pages, Product popup and normal Selection use the same selling-series presentation rule.
- Selling Brand logo is injected into the PDF report before the report HTML is written, preventing the first PDF from showing the previous/default B.G.Reich logo.
- Product popup clears stale Brand/PDF presentation state before each open and pins the new selling Brand/Sub Series before the iframe becomes visible.
- Existing V4.22.01 PDF filename material rule is preserved: CHC / CHCS / CHCN filenames continue to follow the selected CHC material variant.

No Supabase schema migration is required.
