# KeySuite V4.21.06

## CHCN PDF filename correction

- CHCN remains the material/model designation displayed inside KeySuite and inside the exported PDF.
- Saved/exported PDF filenames normalize the token `CHCN` to `CHC`.
- Example: a PDF whose displayed model is `CHCN 32-10` saves using `CHC 32-10` in the filename.
- Applied to Selection PDF, Product Curve PDF, quotation item datasheet export, CHC C4/G1 and CHC C6/G2.
- No database migration or Edge Function deployment is required.
