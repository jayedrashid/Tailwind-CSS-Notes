

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
- [PostCSS](#postcss)
- [Environment Setup](#environment-setup)
- [Tailwind CSS Folder Structure](#tailwind-css-folder-structure)




---

## Tailwind CSS
Tailwind CSS is an open source CSS framework. The main feature of this library is that, unlike other CSS frameworks like Bootstrap, it does not provide a series of predefined classes for elements such as buttons or tables.


Since Tailwind is a PostCSS plugin, there's nothing stopping you from using it with Sass, Less, Stylus, or other preprocessors, just like you can with other PostCSS plugins like Autoprefixer.

Installing Tailwind CSS as a PostCSS plugin is the most seamless way to integrate it with build tools like webpack, Rollup, Vite, and Parcel.

---

## PostCSS
PostCSS is a software development tool that uses JavaScript-based plugins to automate routine CSS operations. It was designed by Andrey Sitnik with the idea taking its origin in his front-end work for Evil Martians.

PostCSS is a JavaScript tool that transforms your CSS code into an abstract syntax tree (AST) and then provides an API (application programming interface) for analyzing and modifying it using JavaScript plugins.

---

## Environment Setup

- Install VS Code
- Install `Tailwind CSS IntelliSence` (ext.) or `HTML CSS Support` (ext.)
- Setup VS Code `Emmet`
- Install Node

```sh
brew install node
```

- Set up a new or existing npm package

```sh
npm init-y
```

- Install Tailwind CSS

```sh
npm I tailwindcss
```

- Add Tailwind to your CSS src (eg: style.css) 

```sh
@tailwind base;
@tailwind components;
@tailwind utilities; 
```

- Edit JSon file as:

```sh
“scripts”: {
    “build:css”: “tailwind build src/style.css -o dist/style.css”
},
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

- Create CSS:

```sh
npm run create-css
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

