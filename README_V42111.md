# KeySuite V4.21.11

Rebuild of V4.21.10.

- Preserves guided KeyBot model selection so scoped C4/C6 catalogue choices open directly.
- Preserves global navigation priority for Hi / New Request / Back.
- Preserves C4/C6 user-facing naming and G1/G2 Price Group naming.
- Cache/runtime token bumped to `42111` to force the rebuilt browser assets to refresh.
- Telegram webhook runtime version reports `V4.21.11`.

No database migration is required. Deploy the `telegram-webhook` Edge Function.
