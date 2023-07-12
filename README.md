- [TailwindCSS Crash Course](#tailwindcss-crash-course)
  - [Useful Information](#useful-information)
  - [VSCode Extension](#vscode-extension)
  - [Instalation \& Setup](#instalation--setup)

# TailwindCSS Crash Course

[The Net Ninja Course](https://www.youtube.com/watch?v=bxmDnn7lrnk&list=PL4cUxeGkcC9gpXORlEHjc5bgnIi5HEGhw)

- CSS Framework made up of utility classes
- Much lower-level than Bootstrap, Materialize, etc.

## Useful Information

[Official Documentation](https://tailwindcss.com/docs/installation)
[Cheatsheet](https://tailwindcomponents.com/cheatsheet/)

## VSCode Extension

[VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)

## Instalation & Setup

`* Node and npm require`

```zsh
npm install tailwindcss
```

On your `styles.css` file, import Tailwind

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Update the `package.json` scripts to build CSS

```json
{
  ...
  "scripts": {
    ...
    "build-css": "tailwindcss build src/styles.css -o public/styles.css"
              // "tailwindcss build <input CSS file> -o <output CSS file>"
  }
}
```
