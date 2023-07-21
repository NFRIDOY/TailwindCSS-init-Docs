# TailwindCSS-init: How to Tailwind?
# Tailwind: PostCSS with Vite
## 1.0 [In the Terminal]
~~~
npm init -y
~~~
~~~
npm install -D tailwindcss postcss autoprefixer vite
~~~
~~~
npx tailwindcss init -p
~~~

## 2.0 [In the package.json]
~~~
"scripts": {
    "start": "vite"
  },
~~~

## 3.0 [In the style.css]
~~~
@tailwind base;
@tailwind components;
@tailwind utilities;
~~~

## 4.0 [In the Tailwind.config.js]
/** @type {import('tailwindcss').Config} */  <br>
module.exports = { <br>
  content: ["\*"],   &emsp;&emsp;&emsp; /\* Add "\*" THIS ONLY */ <br>
  theme: {  <br>
    extend: {}, <br>
  }, <br>
  plugins: [], <br>
} <br>

....Or Copy and Replace The Full Code in the Tailwind.config.js
~~~
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
}
~~~


## 5.0 [In the index.html]
ADD into the <head> tag of index.html
~~~
<link rel="stylesheet" href="style.css">
~~~


## 6.0 [In the Terminal] <br>
~~~
npm run start
~~~

# ****To Config The Tailwind CSS 
## [In the Terminal] 
~~~
npx tailwindcss init configDefault --full
~~~
...Or Set [NAME] For as anything you want.
~~~
npx tailwindcss init [NAME] --full
~~~

# ****To Production 
[In the package.json] <br>
"scripts": { <br>
    "start": "vite", <br>
    **"build": "vite build"** &emsp;&emsp;&emsp; /\* ADD THIS */ <br>
  }, <br>
....Or Copy and Add This [In the package.json]
~~~
"build": "vite build"
~~~

