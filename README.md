# Scoped Preflight with Tailwind CSS 3
### Add Tailwind to an existing project without breaking existing styles and still benefit from preflight defaults.

![project preview](https://user-images.githubusercontent.com/6473382/152337143-11d9e308-c0d1-403c-bd6e-57ff678c7a11.png)


# Getting Started

### **Step 1**
The custom prefix is appended using [stylus](https://github.com/stylus/stylus) which can be installed using npm.

The scoped-preflight.stylus file restricts the scopes of preflight. Set the desired prefix at top ( default is *tw-cst-pf* ) and run: 
```bash
stylus scoped-preflight.stylus -o scoped-preflight.css
```
### **Step 2**

Copy the contents of scoped-preflight.css under base layer in input.css.

### **Step 3**
That's it :) Start the tailwind cli: 
```bash
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```