# KeySuite V4.21.08

PDC correction based on V4.21.07.

- Customer Edit keeps **Terms (days)** editable whether PDC is checked or not.
- Checkbox text is simply **PDC**.
- PDC no longer forces Terms to 90 and no longer disables the Terms field.
- Quotation payment terms use the entered Terms value and append `PDC` only when checked. Example: Terms `90` + PDC checked -> `90 days PDC`.
- Existing customer storage continues to use `payment_terms`; no schema migration is required.
- Browser/service-worker cache bumped to V4.21.08.

No Supabase database migration or Edge Function deployment is required.
