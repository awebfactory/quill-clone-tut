# Quill Clone Tutorial Step by Step

- Based on [You Tube Josh tried coding 2023-09-28 Build a Complete SaaS Platform with Next.js 13, React, Prisma, tRPC, Tailwind | Full Course 2023](https://www.youtube.com/watch?v=ucX2zXAZ1I0)

## Project creation from scratch

```bash
victor@victorpc:dev$ npx create-next-app@latest
✔ What is your project named? … quill-clone-tut
✔ Would you like to use TypeScript? … No / Yes
✔ Would you like to use ESLint? … No / Yes
✔ Would you like to use Tailwind CSS? … No / Yes
✔ Would you like to use `src/` directory? … No / Yes
✔ Would you like to use App Router? (recommended) … No / Yes
✔ Would you like to customize the default import alias? … No / Yes
Creating a new Next.js app in /home/victor/Work/Learn/NextJS/NextJS-2023/JoshTriedCoding/dev/quill-clone-tut.

Using npm.

Initializing project with template: app-tw


Installing dependencies:
- react
- react-dom
- next

Installing devDependencies:
- typescript
- @types/react
- @types/node
- @types/react-dom
- autoprefixer
- postcss
- tailwindcss
- eslint
- eslint-config-next


added 331 packages, and audited 332 packages in 25s

117 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
Initialized a git repository.

Success! Created quill-clone-tut at [workstation dir](~/Work/Learn/NextJS/NextJS-2023/JoshTriedCoding/dev/quill-clone-tut)
```

## Create Landing Page

### Phase Planning

- 08:22
  > SaaS dev build workflow: Landing Page & Navigation ➡️ Auth ️➡ Functionality (➡ Payment & Launch)

## Adding Radix UI based shadcn/ui to the project

```bash
victor@victorpc:quill-clone-tut$ npx shadcn-ui@latest init
Need to install the following packages:
  shadcn-ui@0.4.0
Ok to proceed? (y) y
✔ Would you like to use TypeScript (recommended)? … no / yes
✔ Which style would you like to use? › Default
✔ Which color would you like to use as base color? › Zinc
✔ Where is your global CSS file? … src/app/globals.css
✔ Would you like to use CSS variables for colors? … no / yes
✔ Where is your tailwind.config.js located? … tailwind.config.ts
✔ Configure the import alias for components: … @/components
✔ Configure the import alias for utils: … @/lib/utils
✔ Are you using React Server Components? … no / yes
✔ Write configuration to components.json. Proceed? … yes

✔ Writing components.json...
✔ Initializing project...
✔ Installing dependencies...

Success! Project initialization completed.
```

- Now we can choose any of the [shadcn/ui components](https://ui.shadcn.com/docs/components/accordion) and install them via `npx` (CLI method)
- So, button for our home page, for example:

```bash
victor@victorpc:quill-clone-tut$ npx shadcn-ui@latest add shadcn-ui@latest add button
✔ Done.

victor@victorpc:quill-clone-tut$ tree src/components
src/components
├── MaxWidthWrapper.tsx
└── ui
    └── button.tsx

1 directory, 2 files
```

---

## Original Next.js README

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
