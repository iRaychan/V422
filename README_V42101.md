# KeySuite V4.21.01

## CHC G1 hydraulic curve
- Source: `004 - CHC G1 260831 - V1.1.xlsx`.
- 18 hydraulic families / 409 model configurations.
- CHC G1 curve/UI/PDF behavior follows the proven CHC G2 selector/product format.
- G1 uses its own hydraulic curves, efficiency, NPSHr, motor kW/HP, dimensions, connections and pressure data.
- G1 motor efficiency default is IE2.
- G1 is available in normal Selection and Quick Selection as an independent CHC generation; G1 and G2 results are kept separate.
- Customer Curve / Quick Selection preference can enable CHC G1 independently from CHC G2.
- Reduced-impeller curves are included for CHC 32/45/64/90/120/150; CHC 200 includes full/small/smallest impeller curves.
- Source-data correction confirmed by user: `CHC 32-11-2` and `CHC 32-11` are 11 stages.
- CHC G2 data and curve engine remain unchanged.

## CHC 200 visible model correction
The G1 specification now uses numeric impeller suffixes (for example `CHC 200-3-1-1` and `CHC 200-4-0-2`) instead of the prior synthetic A/B labels. A migration is included to rename existing G1 price-list records without changing their entered prices.

## CHC G1 price-model master V1.1
- Source: `010 - CHC G1 (Pricelist) - 260831 - V1.1.xlsx`.
- Price model master contains **373 models**.
- CHC 200 price models now use the same numeric impeller suffixes as the G1 hydraulic master.
- The obsolete separate `CHC 5-5 (60Hz)` price-list entry from the prior seed is removed.
- The normal `CHC 5-6` remains because it is explicitly present in the attached V1.1 workbook.
- Existing entered G1 prices are preserved during the CHC 200 rename; only model identifiers/source metadata are reconciled.
- `CHC_G1_PRICELIST_MODEL_MAP_V1.1.csv` is included as the exact V1.1 price-model audit map.

