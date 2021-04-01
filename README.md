# Files
## _document.tsx
- Renders the Main Document <Head> <body> <Main> <NextScript>
- Any JavaScript inside this will only be executed in the client side
## _app.tsx
- Responsible to render all the pages
- JS code inside this file will be executed both on client and server side

## CSS
### Styled-jsx 
- Its CSS in Javascript though its not recommended, we can have a style tag inside a component and that style will be applied only to that particular component
### Global CSS in _app.tsx
- Import a css file in _app.tsx .
- This css file will be applied to all the pages. 
- A css file cannot be imported to any other page or Component
### CSS only for a component or page
- To include a css file to a particualr component or a page.
- You should name the css file as filename.module.css . 
- And include that as `import style from fileName.module.css

# API Folder
- All files inside api folder should be js or ts files
- All files should export a function with (req,res) just like express
- To call a api function call `localhost:3000/api/file-name`
