# KeySuite V4.21.07

Built from V4.21.06.

## Changes
- PDF item export: the PDF document title/metadata is locked to the exact requested Item filename, preventing a stale item number (for example Item 08 inside an Item 04 PDF).
- Quick Selection: Recommended and Alternative models now wait for the final selector frame and use an explicit open-model acknowledgement/retry, so the curve opens on the first click for CHC C4, CHC C6 and ES.
- Dashboard customer clear (X): resets the pump PDF Item counter. Reselecting the same customer starts again at Item 01; previously saved records are not deleted.
- Customer Edit: PDC checkbox added beside Terms (days). When checked, Terms is fixed at 90 and customer/quotation payment terms present as `90 Days PDC`. The value is stored in the existing customer `payment_terms` field, so no database schema migration is required.
- Browser/service-worker cache key bumped to V4.21.07.

No Supabase database migration or Edge Function deployment is required for V4.21.07.
