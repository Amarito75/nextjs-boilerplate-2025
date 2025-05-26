# 🚀 NextJS Boilerplate 2025

A modern, feature-rich starter template for building web applications with Next.js 15, Prisma, shadcn/ui, and better-auth.

## ✨ Features

- 🔥 [Next.js 15](https://nextjs.org/) with App Router and Turbopack
- 💾 [Prisma](https://www.prisma.io/) with PostgreSQL (Supabase) integration
- 🎨 [shadcn/ui](https://ui.shadcn.com/) for beautiful, accessible components
- 🔐 [better-auth](https://github.com/better-auth/better-auth) for authentication
- 🌙 Dark mode support with [next-themes](https://github.com/pacocoursey/next-themes)
- 📱 Fully responsive design with [Tailwind CSS](https://tailwindcss.com/)
- 🪄 TypeScript for type safety
- 🔔 Toast notifications with [sonner](https://sonner.emilkowal.ski/)

## 🚦 Getting Started

### Prerequisites

- Node.js 18+ and pnpm (recommended)
- PostgreSQL database (or use the provided Supabase connection)

### Setup

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/boilerplate-2025.git
cd boilerplate-2025
```

2. **Install dependencies**

```bash
pnpm install
```

3. **Environment Setup**

Copy the example environment file and modify as needed:

```bash
cp .env.example .env
```

Update the following variables in your `.env` file:

- `DATABASE_URL`: Your PostgreSQL connection string (with pooling)
- `DIRECT_URL`: Direct database connection (for migrations)
- `NEXT_PUBLIC_BETTER_AUTH_SECRET`: Secret key for authentication
- `NEXT_PUBLIC_BETTER_AUTH_URL`: Your application URL

4. **Set up the database**

```bash
pnpm prisma db push
```

5. **Start the development server**

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) to see your application.

## 🏗️ Project Structure

```
boilerplate-2025/
├── app/             # Next.js app router pages and layouts
├── components/      # UI components (including shadcn components)
├── lib/             # Utility functions and shared code
├── prisma/          # Prisma schema and migrations
├── public/          # Static assets
└── ...
```

## 💻 Development Workflow

- Modify `app/page.tsx` to change the homepage
- Run `pnpm prisma studio` to view and edit your database
- Add new components to the `components/` directory
- Add new pages in the `app/` directory
- Update the Prisma schema in `prisma/schema.prisma` for database changes

## 🧩 Adding shadcn/ui Components

To add new shadcn/ui components, use the CLI:

```bash
pnpm dlx shadcn-ui@latest add button
```

## 🔐 Authentication with better-auth

This boilerplate uses better-auth for authentication. Available features:

- Email/password login and registration
- OAuth providers support
- Session management
- User profiles

## 📚 Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Prisma Documentation](https://www.prisma.io/docs)
- [shadcn/ui Documentation](https://ui.shadcn.com)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)

## 📄 License

MIT
