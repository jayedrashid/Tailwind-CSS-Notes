

# `Tailwind CSS`

`Tailwind CSS - Notes`

<p align="center">
 <img width="750px" src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20220831183000/Tailwind-CSS-Tutorial1.png" align="center" alt="GitHub Readme Stats" />
 <h2 align="center">Tailwind CSS Beginners Guide</h2>
</p>

To Learn officially go to.. [Tailwind CSS](https://tailwindcss.com/docs/installation)

---

## Quick Links

- [Tailwind CSS](#tailwindcss)
- [Production Build for Purging](#production-build-for-purging)
- [PostCSS](#postcss)
- [Tailwind CSS Installation](#tailwind-css-installation)
- [Environment Setup](#environment-setup)
- [Component Extraction](#component-extraction)
- [Tailwind CSS Folder Structure](#tailwind-css-folder-structure)
- [Breakpoints](#breakpoints)



---

## Tailwind CSS
Tailwind CSS is an open source CSS framework. The main feature of this library is that, unlike other CSS frameworks like Bootstrap, it does not provide a series of predefined classes for elements such as buttons or tables.


Since Tailwind is a PostCSS plugin, there's nothing stopping you from using it with Sass, Less, Stylus, or other preprocessors, just like you can with other PostCSS plugins like Autoprefixer.

Installing Tailwind CSS as a PostCSS plugin is the most seamless way to integrate it with build tools like webpack, Rollup, Vite, and Parcel.

---

## Production Build for Purging

Tailwind CSS is incredibly performance focused and aims to produce the smallest CSS file possible by only generating the CSS you are actually using in your project. Combined with minification and network compression, this usually leads to CSS files that are less than 10kB, even for large projects.

Tailwind CSS v2.1 introduces a new just-in-time (JIT) compiler for Tailwind CSS that generates your styles on-demand as you author your templates instead of generating everything in advance at initial build time.

---

## PostCSS
PostCSS is a software development tool that uses JavaScript-based plugins to automate routine CSS operations. It was designed by Andrey Sitnik with the idea taking its origin in his front-end work for Evil Martians.

PostCSS is a JavaScript tool that transforms your CSS code into an abstract syntax tree (AST) and then provides an API (application programming interface) for analyzing and modifying it using JavaScript plugins.

---

## Tailwind CSS Installation

- Install from CDN (non-customizable)
- Install as PostCSS Plugin ()
- Install Tailwind CLI (using terminal commands)

---

## Environment Setup

- Install VS Code
- Install `Tailwind CSS IntelliSence` (ext.) or `HTML CSS Support` (ext.)
- Setup VS Code `Emmet`
- Install Node

```sh
brew install node
```

- Set up a new npm package

```sh
npm init -y
```

- Install Tailwind CSS

```sh
npm I -D tailwindcss
```

- Install tailwind config file:

```sh
npx tailwindcss init
```

- Edit tailwind.config.js file as:

```sh
module.exports = {
  content: [“*”],
  theme: {
  },
  plugins: {
  }
}
```

- Add Tailwind to your CSS src (eg: style.css) 

```sh
@tailwind base;
@tailwind components;
@tailwind utilities; 
```

- Edit package.json file as:

```sh
“scripts”: {
    “build”: “tailwindcss -i ./src/style.css -o ./output/style.css -w”
},
```


- Add CSS file to HTML as:

rel="stylesheet" href="./output/style.css"

- Run Build as:

```sh
npm run build
```

- css run:

```sh
npm run create-css
```

---

## Component Extraction

Add Custom CSS to your CSS src (eg: style.css) file to avoid repeatation. Use the created utility class (eg: btn-purple) in your html file.

```sh
.btn-purple {
     @apply px-4 py-1 border-purple-200 rounded-full focus:outline-none
}
```

---

## Tailwind CSS Folder Structure

[Structuring Tailwind CSS Projects](https://aviyel.com/post/1180/setting-up-tailwindcss-inside-vanilla-html-project)

`Tailwind CSS` Folder Structure

```
root
├── css
│   └── tailwind.css
├── node_modules
├── public/build
│   └── tailwind.css
├── package-lock.json
├── package.json
├── postcss.config.js
└── tailwind.config.js

```

[Structuring Tailwind CSS in React Projects](hhttps://dev.to/hasibrashid/tailwindcss-with-reactjs-3ih9)

`Tailwind CSS in React` Folder Structure

```
root
├── node_modules
├── public
├── src
│   ├── styles
│   │   ├── global.css
│   │   └── tailwind.css
│   ├── App.css
│   ├── App.js
│   ├── App.test.js
│   ├── index.css
│   ├── index.js
│   ├── logo.svg
│   ├── reportWebVitals.js
│   └── setupTests.js
├── .gitignore
├── package-lock.json
├── package.json
└── readme.md

```

---

## Breakpoints

sm		640px		@media (min-width: 640px) { ... }	Mobile
md		768px		@media (min-width: 768px) { ... }	Fablet
lg		1024px		@media (min-width: 1024px) { ... }	Tablet
xl		1280px		@media (min-width: 1280px) { ... }	Laptop
2xl		1536px		@media (min-width: 1536px) { ... }	Desktop

---

## Notes

1. No class order in Tailwind CSS
2. Tailwind CSS coding is mobile first. You need to add additional codes for md and lg devices
3. Tailwind size / 4 = rem
4. Tailwind size x 16 = px
5. Installing CDN is great for html templates 
6. Responsive variants: see Breakpoints list
7. Stacking (Order) of variants 
eg: lg:dark:hover:bg-white
8. Dark mode variant 
darkMode: media (system preference) and
darkMode: class (manual preference)
8. Specificity counts eg: ‘text-black’ loses specificity after adding ‘dark:text-white’ while darkMode: class selected in config.js

---

## Contributing

1. Fork it
2. Create your feature branch with specs (`git checkout -b my-cute-feature`).
3. Commit your changes (`git commit -m 'Added my cute feature'`).
4. Push to the branch (`git push origin my-cute-feature`).
5. Create your new pull request.

---

## Contributors

<table>
  <tr>
    <td align="center"><a href="https://jayedrashid.com/"><img src="https://avatars.githubusercontent.com/u/68325519?s=400&u=c3380d6ce56295f87d4f877de9ca04b7adf28d55&v=4" width="100px;" style="border-radius:50%; border:2px solid white;" alt=""/><br /><sub><b>Jayed Rashid</b></sub></a><br />   
  </tr>
</table>

---

## Let's Connect

Feel free to Contact me on [Twitter](https://mobile.twitter.com/jayedrashid), send an email to jayed@jayedrashid.com

<img height="20" src="https://www.bollywoodmdb.com/images/uparrow.gif"> [back to top](#quick-links)<br>

