# Tailwind CSS Procedure

## 1. How to setup Tailwind CSS

Step 1: Install Tailwind CSS

Install tailwindcss and @tailwindcss/cli via npm.

```
npm install tailwindcss @tailwindcss/cli
```
Step 2:
Import Tailwind in your CSS

Add the @import "tailwindcss"; import to your main CSS file.

```
@import "tailwindcss";
```

Step 3: Start the Tailwind CLI build process

Run the CLI tool to scan your source files for classes and build your CSS.

```
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```


Step 4: Start using Tailwind in your HTML

Add your compiled CSS file to the <head> and start using Tailwind’s utility classes to style your content.

```

<link href="./output.css" rel="stylesheet">
       
```

## 2. To automate the --watch process

Step 1: Create a 'build' script to package.json

```
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch"
  },
```

Step 2: Open terminal and run the following command:

```
npm build
```