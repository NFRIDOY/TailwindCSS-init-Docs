# TailwindCSS-init
How to Tailwind?

# Tailwind: PostCSS with Vite
## [In the Terminal]
~~~
npm init -y
npm install -D tailwindcss postcss autoprefixer vite
npx tailwindcss init -p
~~~

## [In the package.json]
~~~
"scripts": { 
    <b>"start": "vite"
  },
~~~

## [In the style.css]
~~~
@tailwind base;
@tailwind components;
@tailwind utilities;
~~~

## [In the Tailwind.config.js]
/** @type {import('tailwindcss').Config} */  <br>
module.exports = { <br>
  content: ["\*"],   &emsp;&emsp;&emsp; /\* EDIT THIS ONLY */ <br>
  theme: {  <br>
    extend: {}, <br>
  }, <br>
  plugins: [], <br>
} <br>

## [In the index.html]
ADD <br>
~~~
<link rel="stylesheet" href="style.css">
~~~


## [In the Terminal] <br>
~~~
npm run start 
~~~

### ****To Config
[In the Terminal] <br>
npx tailwindcss init configDefault --full      	// npx tailwindcss init [NAME] --full <br>

### ****To Production 
[In the package.json] <br>
"scripts": { <br>
    "start": "vite", <br>
    **"build": "vite build"** <br>
  }, <br>

