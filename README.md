# supabase-next-test

A test repo for experimenting with:

- Supabase
- Next.js v14 App Router

## Steps taken for project setup

1. Install Next.js app pre-configured with Cookie-based Auth, TypeScript, and Tailwind CSS:

   `npx create-next-app -e with-supabase`

2. Move application code to the `src` directory:

   i. Update import module alias path in `tsconfig.json` to:

   ```
   "compilerOptions": {
      "paths": {
         "@/*": ["./src/*"]
      }
   }
   ```

   ii. Add the `/src` prefix to the `tailwind.config.js` file in the `content` section like so:

   ```
   content: [
      "./src/app/**/*.{js,ts,jsx,tsx,mdx}",
      "./src/components/**/*.{js,ts,jsx,tsx,mdx}"
   ]
   ```
