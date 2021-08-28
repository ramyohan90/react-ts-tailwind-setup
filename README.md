##### React setup with typescript and tailwind css

# Step 1: 
#       create-react-app <project-name> --template=typescript
# Step 2: 
#       npm i tailwindcss@^2.0.2 postcss-cli@^8.3.1 postcss@^8.2.1 autoprefixer@^10.1.0 @fullhuman/postcss-purgecss@4.0.0
# Step 3:
#       npx tailwindcss init tailwindcss-config.js --full
# Step 4:
#       Create styles.css and tailwind.css. tailwind.css should hold custom / tailwind components
# Step 5: 
#       In package.json script property, configure tailwind script to output extracted css to the destination
#       "build:css": "postcss src/styles/tailwind.css -o src/styles/styles.css",
#       "build:watch": "postcss src/styles/tailwind.css -o src/styles/styles.css --watch"
# Step 6:
#       create postcss.config.js in root folder and import tailwind and autoproefixer packages. This will benecessary to create or extract css
# Step 7:
#       npm run build:css to extract css
# Step 8: 
#       import styles.css (as per your naming css convention) in app.ts
# Step 9:
#       npm start and check if tailwind is working
# Step 10: 
#        Extra: Install Tailwind intellisense to autocomplete