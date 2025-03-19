# 2025-03-19 Bug Report Qwik TailwindCSS Vite 4.0.8

This repository demonstrates an issue with @tailwindcss/vite 4.0.8 and higher.

The following was done to reproduce the issue

1. pnpm create qwik@latest
2. pnpm run qwik add tailwind
3. Modify package.json to pin @tailwindcss/vite to 4.0.8
4. Updated src/routes/index.tsx to use tailwindcss classes

To run this project

```bash
pnpm i 
pnpm run dev
```

Then connect to http://localhost:5173

If you change the @tailwindcss/vite version to 4.0.7 in the package.json, run a pnpm update and then
run the project the tailwindcss classes will work as expected.
