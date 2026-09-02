# KeySuite V4.21.10

KeyBot Telegram state fix.

- Guided Product drill-down owns its own model buttons. A scoped model such as B.G.Reich > CHC C4 > CHC 8 > CHC 8-10 opens directly and is not re-routed through global Fast Search.
- Global navigation (Hi/Menu, New Request, Back) is processed before pending Brand / Model disambiguation.
- Back from an older/stale Fast Search model-choice state restores the previous guided catalogue when that context exists; otherwise it returns to the selected customer or main menu.
- True unscoped CHC ambiguity now labels B.G.Reich generations distinctly as CHC C4 / CHC C6 instead of two identical B.G.Reich - CHC model buttons.

No database migration is required. Deploy the telegram-webhook Edge Function.
