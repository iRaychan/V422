# KeySuite V4.21.12

## KeyBot CHC C4 Page 3 dimension drawing

- Fixes the Telegram / KeyBot PDF Page 3 dimension picture for CHC C4 (G1).
- C4/G1 now uses the same 13 G1 dimension drawing assets already used by the web C4 selector.
- G1 numeric dimension values continue to come from the G1 dimension table.
- G1 drawing selection follows the existing web resolver:
  - CHC 1/2/3/4/5: CHC drawing vs CHCS/CHCN drawing
  - CHC 8/10: CHC drawing vs CHCS/CHCN drawing
  - CHC 12: supplied G1 drawing
  - CHC 15/16/20: CHC drawing vs CHCS/CHCN drawing
  - CHC 32/45/64/90/120/150/200: supplied G1 family drawing
- C6/G2 continues using the existing G2 dimension drawing map.
- No Supabase database migration is required.
- Redeploy `telegram-webhook`.
