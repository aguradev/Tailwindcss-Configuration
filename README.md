<p>
<img src="https://raw.githubusercontent.com/tailwindlabs/tailwindcss/master/.github/logo-dark.svg" width="350px" height="50px">
</p>

## Documentation

Source : https://tailwindcss.com/docs/installation

## Requirement

- create folder project where ever you want
- make sure you already install [npm](https://www.npmjs.com/package/npm)
- use terminal like :
  - powershell
  - git bash

# How To Install And Configuration

## Configuration npm to folder

```
npm init
```

## Default Install Tailwindcss

```
npm i -D tailwindcss
```

## I prefer to use this to install tailwindcss

```
npm i -D tailwindcss postcss autoprefixer
```

## Create Configuration tailwind file

```
npx tailwindcss init
```

## Example configuration content file in tailwind.config.js

```JS
module.exports = {
  content: ["./index.html"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

## Create file type.css and add Tailwind Directives in your css

```css
/* reset to default style and use tailwind style */
@tailwind base;

/* Get Components Tailwind Like Container */
@tailwind components;

/* Get Utilities Tailwind Like Button,Color,Margin,Padding And More */
@tailwind utilities;
```

## Run npx to compile preprocessor css for create file.css and use it to your project

```
npx tailwindcss -i ./input.css -o ./new-file.css --watch
```
