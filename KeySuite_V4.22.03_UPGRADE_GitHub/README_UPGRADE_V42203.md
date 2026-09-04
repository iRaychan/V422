# Upgrade to KeySuite V4.22.03

Base version: **V4.22.02**

Copy the files in this patch over the existing V4.22.02 deployment, preserving the same folder structure.

## Fixes

- O.K.Pump Product curve now stays VMS / VMSS / VMSN instead of reverting to CHC / CHCS / CHCN.
- Product CHC/ES Brand Context now targets the correct Product selector iframe.
- Selling Brand/Sub Series presentation is applied while the Product iframe is still hidden, before first display.

No Supabase DB migration and no Edge Function deployment are required.
