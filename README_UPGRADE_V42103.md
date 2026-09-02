# KeySuite V4.21.03 Upgrade

Upgrade target: V4.21.02.

Changes:
- Dashboard -> Brand / Series Settings no longer requires a customer.
- No customer selected: show User Assigned only.
- Customer selected: show User Assigned x Customer Brand / Series Price Preference only.
- Quick Selection execution uses the same rule, not only the visible settings panel.
- Runtime cache version updated so browsers load the patched Quick Selection logic immediately.

Deployment:
1. Replace/upload the files in this upgrade package.
2. No `supabase db push` is required.
3. No Edge Function deployment is required.
