# V4.21.11 Upgrade

Rebuilt from V4.21.10. Replace the supplied files, then deploy KeyBot:

```powershell
npx.cmd supabase@latest functions deploy telegram-webhook --no-verify-jwt
```

No `supabase db push` is required for V4.21.11.
