# TailwindCSS-init
How to Tailwind?

# Tailwind: PostCSS with Vite
## [In the Terminal]
npm init -y <br>
npm install -D tailwindcss postcss autoprefixer vite <br>
npx tailwindcss init -p <br>

## [In the package.json]
"scripts": { <br>
    <b>"start": "vite"</b> <br>
  }, <br>

## [In the style.css]
@tailwind base; <br>
@tailwind components; <br>
@tailwind utilities; <br>

## [In the Tailwind.config.js]
/** @type {import('tailwindcss').Config} */  <br>
module.exports = { <br>
  **content: ["\*"],**   &emsp;&emsp;&emsp; ///////////// &emsp; EDIT THIS ONLY <br>
  theme: {  <br>
    extend: {}, <br>
  }, <br>
  plugins: [], <br>
} <br>

## [In the Terminal] <br>
npm run start <br>

### ****To Config
[In the Terminal] <br>
npx tailwindcss init configDefault --full      	// npx tailwindcss init [NAME] --full <br>

### ****To Production 
[In the package.json] <br>
"scripts": { <br>
    "start": "vite", <br>
    **"build": "vite build"** <br>
  }, <br>

