# learn-nextjs-dashboard-example

[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=fff&style=flat-square)](https://www.typescriptlang.org/)
[![Next.js](https://img.shields.io/badge/Next.js-000?logo=next.js&logoColor=fff&style=flat-square)](https://nextjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-38B2AC?logo=tailwindcss&logoColor=fff&style=flat-square)](https://tailwindcss.com/)

## Overview

A modern dashboard web application built with Next.js and TypeScript, featuring authentication, responsive UI, and structured data management. The app provides an interactive dashboard with overview, customers, and invoices sections, leveraging Tailwind CSS for styling and next-auth for secure user authentication. It demonstrates best practices in structuring scalable, typed, and maintainable React applications.

## Tech Stack

- **Languages:** TypeScript, JavaScript, CSS
- **Frameworks & Libraries:** 
  - [Next.js](https://nextjs.org/) (App Router)
  - [React](https://react.dev/)
  - [Tailwind CSS](https://tailwindcss.com/)
  - [NextAuth.js](https://next-auth.js.org/)
  - [Zod](https://zod.dev/)
  - [Bcrypt](https://www.npmjs.com/package/bcrypt)
  - [Postgres](https://www.postgresql.org/)
  - [Heroicons](https://heroicons.com/) (React)
  - [clsx](https://www.npmjs.com/package/clsx)
  - [use-debounce](https://www.npmjs.com/package/use-debounce)
- **Build Tools:** PostCSS, Autoprefixer
- **Linting & Type Safety:** ESLint, TypeScript

## Prerequisites

- **Node.js** (v16 or higher recommended)
- **Yarn** or **npm** (for dependency management)
- **PostgreSQL** (running instance for data storage)

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/ednandias/learn-nextjs-dashboard-example.git
cd learn-nextjs-dashboard-example
yarn install
# or
npm install
```

## Usage

### Development

Start the development server (with Turbopack):

```bash
yarn dev
# or
npm run dev
```

### Production

Build and start the production server:

```bash
yarn build
yarn start
# or
npm run build
npm start
```

### Linting

Check for linting issues:

```bash
yarn lint
# or
npm run lint
```

### Dashboard

- Access the dashboard at: `http://localhost:3000/dashboard`
- Login at: `http://localhost:3000/login`

## Project Structure

```
.
├── app/
│   ├── dashboard/
│   │   ├── (overview)/
│   │   ├── customers/
│   │   ├── invoices/
│   │   └── layout.tsx
│   ├── favicon.ico
│   ├── layout.tsx
│   ├── lib/
│   │   ├── actions.ts        # Server actions and business logic
│   │   ├── data.ts           # Data fetching utilities
│   │   ├── definitions.ts    # Type definitions and schema
│   │   ├── placeholder-data.ts
│   │   └── utils.ts          # Utility functions
│   ├── login/
│   │   └── page.tsx
│   ├── opengraph-image.png
│   ├── page.tsx
│   ├── query/
│   │   └── route.ts          # API endpoint: /query
│   ├── seed/
│   │   └── route.ts          # API endpoint: /seed
│   └── ui/
│       ├── acme-logo.tsx
│       ├── button.tsx
│       ├── customers/
│       ├── dashboard/
│       ├── fonts.ts
│       ├── global.css
│       ├── home.module.css
│       ├── invoices/
│       ├── login-form.tsx
│       ├── search.tsx
│       └── skeletons.tsx
├── public/
│   ├── customers/
│   ├── hero-desktop.png
│   └── hero-mobile.png
├── auth.config.ts
├── auth.ts
├── eslint.config.mjs
├── next.config.ts
├── package.json
├── postcss.config.js
├── proxy.ts
├── tailwind.config.ts
├── tsconfig.json
├── yarn.lock
└── .gitignore
```

## API Endpoints

| Method | Endpoint   | Description                |
|--------|------------|---------------------------|
| GET    | `/query`   | Fetch query data          |
| POST   | `/query`   | Submit query data         |
| GET    | `/seed`    | Fetch seed data           |
| POST   | `/seed`    | Create seed data          |

## Contributing

We welcome contributions! To contribute:

1. **Fork** the repository to your GitHub account.
2. **Create a new branch** for your feature or bugfix.
3. **Commit** your changes.
4. **Open a Pull Request** with a clear description of your changes.

## License

License not specified. Please contact the repository owner for licensing details.

---
[![README powered by ReadmeAI](https://img.shields.io/badge/README-powered%20by%20ReadmeAI-4c9be8?style=flat-square&logo=markdown)](https://www.readmeai.in)