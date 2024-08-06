# tailwind-css

step 1: npm init -y
2. create a folder: public and create a file index.html inside the public folder
3. npm install -D tailwindcss
& npx tailwindcss init

4. "./src/**/*.{html,js}  copy this from tailwind css docs file and paste it on tailwind.config.js file of content
    content: ["./public/*.html"],

5. create new folder: src and create file input.css
6. copy the following code from docs and paste it inside the input.css file 
@tailwind base;
@tailwind components;
@tailwind utilities;

7. npx tailwindcss -i ./src/input.css -o ./public/style.css --watch 
 this command run tailwindcss in background

 8. change the script: 
 package.json
  "test": "echo \"Error: no test specified\" && exit 1" to  "build": "npx tailwindcss -i ./src/input.css -o ./public/style.css --watch"

9. now connect style.css file in the index.html page