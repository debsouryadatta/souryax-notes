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

## Steps Of Development
1. Create a new project using `npx create-next-app@latest --ts` -> all default options(tailwind, eslint, src folder, app sir)
2. npx shadcn-ui@latest init -> For initialising shadcn-ui, npx shadcn-ui@latest add button

### Clerk
3. Initializing Clerk - creating a project in the clerk dashboard, npm install @clerk/nextjs, saving the secret keys in the .env file
4. Setting up middleware.ts following the clerk docs
5. Building the sign-up & sign-in pages using the clerk components and aligning them


### Landing Page
6. Creating the Landing Page, creating the TypewriterTitle.tsx component
7. Changing the globals.css to add the slight green effect in the landing page
8. npm i typewriter-effect -> For the typing effect, npm i lucide-react for icons


### Dashboard Page
9. Creating the dashboard page, npx shadcn-ui@latest add separator

### Neon & Drizzle
10. Setting up the neonDb in the website, copying the DATABASE_URL to .env file
11. npm i drizzle-orm, npm i @neondatabase/serverless(To connect neon db to our drizzle orm)
12. Creating the index.ts & schema.ts in the lib/db directory
13. Writing the db-config in the index.ts and the schema in the schema.ts
14. npm i drizzle-kit -> To sync the db with the schema, also provides a studio to view the db
15. Creating the drizzle.config.ts file for configuration of the drizzle kit, npm i dotenv(since nextjs can not read the .env file outside the src directory)
16. Changing the target from es5 to es6 in the tsconfig.json file 