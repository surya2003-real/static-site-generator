# Static Site Generator (SSG)
I recommend not downloading node_modules and resolving dependencies yourself.
## now after resolving dependencies or directly cloning repo use
    npm start
    npx serve dist
### Now run the website on your browser.
### You can edit index.md, page2.md and page3.md to change content of websites.

Here I have used `tailwindcss` for styling and `marked` for markdown to html conversion.

If you make any changes in index.md, page2.md or page3.md then you need to run `npm start` again to generate new html files.

Also you can add more pages by adding more .md files in `src` folder and then running `npm start` again.

## How it works
### 1. `npm start` runs `node index.js`
### 2. `index.js` reads all .md files in `src` folder and converts them to html files in `dist` folder.
### 3. `index.js` also copies all files in `src/static` folder to `dist` folder.

## How to use tailwindcss
>If you make any changes in css the you can use `npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch`  
>to watch for changes in css and automatically update `output.css` in `dist` folder.  
>Documentation for tailwindcss is [here](https://tailwindcss.com/docs/installation).

Even though I was able to make this SSG, I am not satisfied with the code. I will try to improve it in future.  
It doesn't contain RSS feed, sitemap, pagination, tags, categories, etc. This was due to time constraints and lack of knowledge.
I sincerely apologize for that. I will try to add these features in future.