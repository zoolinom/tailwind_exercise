# tailwind_exercise

Steps for installing tailwind in empty project:

1. Create package,json file with command:
    npm init -y

2. Instal tailwind, postcss and autoprefixer:
    npm install tailwindcss postcss-cli autoprefixer

3. Run command:
    npx tailwind init
    This command creates empty tailwind.config.js file
    If we need to customize tailwind we can do it in this file

4. Create new file postcss.config.js in root of project
    Inside this file we specify what postcss plugins we want to use

5. Create file css/tailwind.css and add:
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    Tailwind will replace base/components/utilities with all tailwind base styles

6. Go to package,json file and replace test script with build script:
    "build": "postcss css/tailwind.css -o public/build/tailwind.css"

7. Run:
    npm run build
    That will create public/build/tailwind.css file

8. Create index.htm in public folder

9. Add some html code

10. Link Tailwind like any other css with <link> tag

11. Add <h1> tag with some text, and add tailwind classes

12. Install live-server with command:
    npm install -g live-server

13. Run live server from public folder with command:
    live-server public