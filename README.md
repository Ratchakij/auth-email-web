# React + Vite
react-swc

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript and enable type-aware lint rules. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

# Setup Project
npm create vite@latest auth-email-web -- --template react-swc
npm install tailwindcss @tailwindcss/vite

## Install Tailwind CSS
1. Add the @tailwindcss/vite plugin to vite.config.js
    import tailwindcss from '@tailwindcss/vite'
    export default defineConfig({
      plugins: [
        tailwindcss(),
      ],
    })

2. Add an @import to your CSS file that imports Tailwind CSS.
    @import "tailwindcss";

3. Config settings.json for Tailwind CSS IntelliSense
   "tailwindCSS.includeLanguages": {
      "html": "html",
      "javascript": "javascript",
      "css": "css"
   },
   "editor.quickSuggestions": {
      "strings": true
   }