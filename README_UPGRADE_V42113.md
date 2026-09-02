# V4.21.13 Upgrade

## KeyBot C4 dimension asset deployment fix

- Removes the 2 MB embedded `chc-g1-dimension-assets.ts` module from the Telegram Edge Function bundle.
- The 13 CHC C4/G1 dimension drawings are now normal static PNG files under `assets/chc-g1-dimensions/`.
- KeyBot fetches only the required C4 drawing when generating PDF Page 3.
- C4/G1 still uses its own G1 numeric dimensions and CHC vs CHCS/CHCN drawing resolver.
- C6/G2 remains on the existing G2 dimension map.
- The Telegram function package is reduced back below the V4.21.12 size that triggered Supabase HTTP 413.

## KeyPLC Price List

- Adds the missing `3kW` KeyPLC price-list model.
- Adds the missing `37kW` KeyPLC price-list model.
- Both rows contain 1–6 Pump variants and start with blank USD / RMB / MYR values so prices can be entered normally.
- KeyPLC Price List rows are displayed in motor-kW order.

## Deployment

1. Upload the web/upgrade files, including `assets/chc-g1-dimensions/`.
2. Run the included KeyPLC SQL migration (or paste `V42113_KEYPLC_3KW_37KW_SQL_EDITOR.sql` into Supabase SQL Editor).
3. Redeploy the `telegram-webhook` Edge Function.

