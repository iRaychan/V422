# KeySuite V4.21.02

## CHC C4 / KeyBot correction
- CHC C4 is the customer-facing name for the internal G1 hydraulic generation.
- CHC C4 no longer exposes or enables Enhanced mode. C4 remains standard 50 Hz and uses its IE2 motor data.
- Quick Selection only shows the Enhanced checkbox beside CHC G2/C6; C4 requests always force Enhanced = false.
- KeyBot now exposes CHC C4 under the B.G.Reich master CHC assignment, subject to the same User Brand/Series and Customer Price Preference gates as the app.
- KeyBot CHC C4 sizing, exact-model curve, curve PDF and price flow use the C4/G1 hydraulic database instead of falling back to G2.
- CHC C4 Telegram curve PDFs use the C4/G1 dimension table and IE2 motor class while retaining the CHC G2 PDF layout/format.

## Deployment
- No new database migration is required for V4.21.02.
- The `telegram-webhook` Edge Function must be redeployed because KeyBot routing/curve logic changed.
- The upgrade package includes the complete `supabase/functions` tree needed for deployment.
