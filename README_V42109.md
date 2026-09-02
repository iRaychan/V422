# KeySuite V4.21.09

## CHC generation naming normalization

- Internal generation mapping remains **G1 = C4** and **G2 = C6**.
- **Price Group and administrator pricing screens** display **CHC G1** and **CHC G2** consistently.
- **User-facing product/selection/brand-series screens** display **CHC C4** and **CHC C6** consistently.
- Removed mixed user-facing combinations such as `CHC C4 / CHC G2`.
- No database schema or Edge Function change is required for this naming-only patch.
