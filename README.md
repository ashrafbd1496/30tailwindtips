# 30tailwindtips
30 Tailwind Tips
### 1. Steps to start-
npm install -D tailwindcss and npx tailwindcss init
### 2. paste the code into tailwind.config.js/** @type {import('tailwindcss').Config} */
    module.exports = {
    content: ["./src/**/*.{html,js}"],
    theme: {
        extend: {},
    },
    plugins: [],
    }

### 3. create a folder name src
### 5. create a file inside src folder named input.css
### 6. paste the code into input.css file
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
### 7. run the command 
    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
### 8. create a file named index.html and paste the cond into it
    <!doctype html>
    <html>
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="/dist/output.css" rel="stylesheet">
    </head>
    <body>
    <h1 class="text-3xl font-bold underline">
        Hello world!
    </h1>
    </body>
    </html>
### 9. Open the vite server or index.html file into browser