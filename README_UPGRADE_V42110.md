# V4.21.10 Upgrade

Replace the supplied files and deploy the Telegram webhook:

```powershell
npx.cmd supabase@latest functions deploy telegram-webhook --no-verify-jwt
```

No `supabase db push` is required for V4.21.10.
