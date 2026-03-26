# Vue Product Management App

<div align="center">

<img src="https://img.shields.io/badge/Vue.js_3-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" />
<img src="https://img.shields.io/badge/Pinia-FFD859?style=for-the-badge&logo=pinia&logoColor=black" />
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" />

**A full-featured product and task management application built with the Vue 3 ecosystem.**

[Live Demo](https://github.com/brandonperfetti/vue-product-management-app) · [Report Bug](https://github.com/brandonperfetti/vue-product-management-app/issues)

</div>

---

## Overview

This is a production-style **product management SaaS application** demonstrating a complete Vue 3 + TypeScript + Supabase stack. It features a fully relational data layer, role-based views, project and task management, and a component library built on Radix Vue and shadcn/vue.

Built to showcase real-world patterns for Vue 3 applications including composables, Pinia store architecture, typed database models, and accessible UI components.

---

## Features

- 📁 **Project Management** — Create, view, and organize projects with metadata and status tracking
- ✅ **Task Management** — Assign tasks to projects with priority, status, and due date fields
- 🔐 **Authentication** — Supabase Auth with protected routes via Vue Router navigation guards
- 📊 **Data Tables** — Powered by TanStack Table (Vue) with sorting, filtering, and pagination
- 🎨 **Component Library** — Accessible UI components from Radix Vue / shadcn/vue
- 🌙 **State Management** — Pinia stores for auth, projects, and tasks
- 🌱 **Database Seeding** — Faker.js-powered seed script for local development

---

## Tech Stack

| Technology | Purpose |
|---|---|
| [Vue 3](https://vuejs.org/) | Composition API-first frontend framework |
| [TypeScript](https://www.typescriptlang.org/) | Full type safety |
| [Vite](https://vitejs.dev/) | Fast dev server and build tooling |
| [Pinia](https://pinia.vuejs.org/) | State management |
| [Vue Router](https://router.vuejs.org/) | Client-side routing |
| [Supabase](https://supabase.com/) | Postgres database + Auth + real-time |
| [TanStack Table (Vue)](https://tanstack.com/table/latest) | Headless data tables |
| [Radix Vue](https://www.radix-vue.com/) | Unstyled, accessible component primitives |
| [Tailwind CSS](https://tailwindcss.com/) | Utility-first styling |
| [VueUse](https://vueuse.org/) | Composition utility library |
| [Faker.js](https://fakerjs.dev/) | Seed data generation |

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18+
- [npm](https://www.npmjs.com/)
- A [Supabase](https://supabase.com/) project (free tier works)

### Installation

```bash
git clone https://github.com/brandonperfetti/vue-product-management-app.git
cd vue-product-management-app
npm install
```

### Environment Variables

Create a `.env` file in the project root:

```env
VITE_SUPABASE_URL=https://your-project.supabase.co
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### Database Setup

Apply the database schema from `supabase/` to your Supabase project, then optionally seed local data:

```bash
node database/seed.js
```

### Development

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Production Build

```bash
npm run build
```

### Type Check

```bash
npm run type-check
```

### Lint

```bash
npm run lint
```

---

## Project Structure

```
vue-product-management-app/
├── src/
│   ├── components/       # Reusable UI components (shadcn/vue-based)
│   ├── pages/
│   │   ├── projects/     # Project list and detail views
│   │   └── tasks/        # Task list and management views
│   ├── stores/           # Pinia state stores
│   ├── router/           # Vue Router config with auth guards
│   ├── lib/              # Supabase client and utilities
│   └── utils/            # Shared helpers
├── database/
│   ├── seed.js           # Faker-powered seed data generator
│   └── types.ts          # Database type definitions
├── supabase/             # Supabase schema and migration files
└── public/               # Static assets
```

---

## Deployment

Deploy to Vercel or Netlify. Set your Supabase environment variables in the platform's project settings.

---

## License

MIT © [Brandon Perfetti](https://brandonperfetti.com)
