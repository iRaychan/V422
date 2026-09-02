# KeySuite V4.21.03

## Dashboard Brand / Series Settings
- When no Dashboard customer is selected, Brand / Series Settings shows only the signed-in user's Role Brand Assigned scope.
- A customer is no longer required just to use Quick Selection.
- When a customer is selected, the eligible list becomes the intersection of User Assigned and the customer's Brand / Series Price Preference.
- Saved Quick Selection preferences are filtered against the currently authorized User Assigned list, so previously saved unassigned entries cannot reappear.
- The Dashboard hint/status identifies whether the current list is `User Assigned` or `User + Customer`.
- Owner remains unrestricted by Role Brand Assigned and therefore sees the active eligible Brand / Series list when no customer is selected.

## Deployment
- No database migration is required for V4.21.03.
- No Supabase Edge Function deployment is required for V4.21.03.
- Replace/upload the web files only.
