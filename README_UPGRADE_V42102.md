# KeySuite V4.21.02 Upgrade

Upgrade target: V4.21.01.

Changes:
- CHC C4: Enhanced hidden/disabled and always false.
- CHC C4: visible naming cleaned up in app labels.
- KeyBot: CHC C4 now appears when allowed by User Brand/Series assignment and Customer Price Preference.
- KeyBot: C4 uses the G1 hydraulic/core database, G1 dimensions and IE2 motor data for curve/PDF/selection.
- C4 and G2/C6 stay hydraulically independent.

Deployment:
1. Replace/upload the upgrade files.
2. Redeploy the Telegram Edge Function:
   `npx.cmd supabase@latest functions deploy telegram-webhook --no-verify-jwt`
3. No `supabase db push` is required for this V4.21.02 patch.
