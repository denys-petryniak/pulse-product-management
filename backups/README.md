# Database backups

This is an educational project on the Supabase **free plan**, which has no scheduled backups
and pauses the project after 7 days of inactivity. These snapshots exist so the demo can be
rebuilt if the project is ever paused for too long or deleted.

Each dated folder holds a data-only export of the `public` tables, taken through the REST API
with the service role key. All rows are seed data from `database/seed.js` (Faker).

## Restore

1. Create a new Supabase project and apply the schema from `supabase/migrations/`.
2. Sign up the users again (auth users are not backed up here, since they hold personal data).
3. Insert the rows in dependency order: `profiles` → `projects` → `tasks`.
   Each `profiles.id` must match the new `auth.users` id.
