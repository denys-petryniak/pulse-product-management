# Product Management Dashboard

> Built while learning Vue 3 through [The Vue.js 3 Master Class](https://vueschool.io/the-vuejs-3-master-class) at Vue School, then extended with Supabase, FormKit, TanStack Table, and shadcn-vue.

## Stack

- **Frontend**: Vue 3 (Composition API), TypeScript, Vite, Pinia, Vue Router
- **Backend**: Supabase (Postgres + Auth)
- **Forms**: FormKit
- **Tables**: TanStack Vue Table
- **UI**: shadcn-vue (Radix Vue) + Tailwind CSS
- **Tooling**: Husky, Commitlint, ESLint, Prettier

## Setup

```sh
pnpm install
```

### Development

```sh
pnpm dev
```

Runs at [http://localhost:4000](http://localhost:4000).

### Supabase

```sh
pnpm supabase:link    # link the local project
pnpm supabase:types   # regenerate database/types.ts from the live schema
pnpm db:reset         # reset the linked database
pnpm db:seed          # run the seed script
```

### Build

```sh
pnpm build
pnpm preview
```
