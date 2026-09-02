# KeySuite V4.21 FULL CLEAN

Full-clean continuation built from the verified KeySuite V4.20.01 baseline.

## CHC impeller adjustment

- Custom reduced/small impeller counts now use the visible CHC suffix instead of `(Custom)`.
- Example: CHC 32-30 with 3 small/reduced impellers displays as `CHC 32-30-3`.
- Example: CHC 32-80 with 5 small/reduced impellers displays as `CHC 32-80-5`.
- Pricing remains tied to a valid catalog SKU. When the custom reduced count is beyond the catalog range, pricing uses the closest available reduced-impeller SKU for the same base model.
- Therefore CHC 32-30-3 prices from CHC 32-30-2, and CHC 32-80-5 prices from CHC 32-80-2.
- Existing exact catalog impeller models continue to use their exact model name and price.
- Existing physical `Reduce Impeller` stage-removal behavior remains unchanged.

## V4.20.01 pricing correction retained

- Fixed Price remains global/customer-independent.
- Fixed rows are resolved before customer Pricing Category currency filters.
- Fixed pricing does not require USD/RMB/MYR to be selected.
- Fixed pricing continues to bypass margin, rarity factors, transport, discounts, fuel charge, and RM10 rounding.

No SQL migration is required.
