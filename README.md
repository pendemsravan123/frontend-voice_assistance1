# Voice Assistance — Frontend (React + Vite)

Project description
-------------------
A Single-Page Application (SPA) voice assistance client built with React and Vite.

Local setup
-----------
1. Install dependencies
```bash
npm install
```
2. Start development server
```bash
npm run dev
```
3. Build for production
```bash
npm run build
```

Environment variables
---------------------
- `VITE_API_URL` — Base URL of the backend API (e.g. https://api.example.com)

Vercel deployment
-----------------
1. Push this repo to GitHub.
2. In Vercel, create a new Project → Import Git Repository.
3. Build Command: `npm run build`
4. Output Directory: `dist`
5. Add Environment Variable `VITE_API_URL` in Vercel dashboard (Project Settings → Environment Variables).
6. Deploy. Vercel will serve the `dist` SPA; the `vercel.json` rewrite prevents 404s on page refresh.

Notes
-----
- Ensure `VITE_API_URL` starts with `https://` for production.
- Use Vercel's preview/staging environments for testing before production.

Git commands (Frontend)
-----------------------
# Run these from the Frontend project directory (replace placeholders)
```bash
# Remove existing local git if present (cleanup first)
git init -b main
git add .
git commit -m "Initial commit — frontend"
git remote add origin https://github.com/<GITHUB_USERNAME>/<FRONTEND_REPO>.git
git push -f origin main
```
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some Oxlint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the Oxlint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and Oxlint's TypeScript related rules in your project.
