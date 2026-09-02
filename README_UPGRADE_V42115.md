# KeySuite V4.21.15 Upgrade

## KeyBot End Suction Pole buttons

- Product -> B.G.Reich · End Suction now displays **2P** and **4P** as Telegram reply-keyboard buttons.
- The user no longer needs to type the pole during the normal guided Product flow.
- The ES hierarchy now reads Pole / ES Series / exact Model from the hydraulic ES selector database rather than relying on price-list rows for pole/rpm.
- Manual `2`, `2P`, `2 Pole`, `4`, `4P`, and `4 Pole` remain accepted as a fallback.
- Back and New Request remain available.

## Deployment

- No database migration is required.
- Redeploy `telegram-webhook` after uploading the V4.21.15 Upgrade files.
