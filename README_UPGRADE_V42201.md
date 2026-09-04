# KeySuite V4.22.01 Upgrade

Upgrade base: **KeySuite V4.21.15**

## Included fixes

### Role Brand / Series Assigned + Quick Selection
- B.G.Reich CHC C4 and CHC C6 are independently assignable per user.
- Owner can manage all user assignments, but the Owner account's own Product / Quick Selection visibility now also follows its saved Role Brand / Series Assigned scope.
- No customer selected: visible products = User Assigned only.
- Customer selected: visible products = User Assigned intersect Customer Brand / Series Price Preference.
- Existing legacy `CHC` role-scope entries remain backward-compatible until the Owner resaves the user scope.

### CHC PDF saved filename
- CHC exports as `CHC ...pdf`.
- CHCS exports as `CHCS ...pdf`.
- CHCN exports as `CHCN ...pdf`.
- Applied to CHC C4 and CHC C6 selector export paths.

## Deployment
- No database migration is required.
- Upload/copy the patch files over the existing V4.21.15 deployment, preserving the folder paths.
- Refresh/redeploy the static site so the V4.22.01 service-worker/cache version is active.
