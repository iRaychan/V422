# KeySuite V4.22.10

- Corrects the V4.22.09 CHC C4 Product curve regression.
- C4 Product curves are routed to `selector-g1/product.html` before the model is posted.
- C6 remains on `selector/product.html`; End Suction remains on its dedicated selector.
- Shared Product Curve Back handling is retained for C4/C6/ES.
- Product-frame model-load failures are non-blocking and no longer create repeated alert loops that can freeze navigation.
- No Supabase database migration is required.
