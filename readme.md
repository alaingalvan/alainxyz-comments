![Cover Art](https://alain.xyz/assets/brand/website-screenshot.jpg)

# 🔮 Alain.xyz Blog Comments

[![License][license-img]][license-url]

All comments on the [Alain.xyz](https://alain.xyz/blog) are powered by [Uterances](https://utteranc.es/), a tool that uses Github issues as threads for blog post comments.

## How it Works

The site is comprised of 3 primary modules:

```bash
├─ daemon/    # Server Daemon
├─ backend/   # Express HTTP Server
├─ frontend/  # React Frontend Application
└─ portfolio/ # Personal Portfolio
```

### Backend

The **Backend** is a basic Express HTTP server, with the added functionality of being able to prerender React components to help reduce the time to interaction.

- [Node](https://nodejs.org/en/) - JavaScript based web server.

- [Express](https://expressjs.com/) - Middleware based web server framework.

- [MongoDB](https://mongodb.org/) - Basic non-relational database.

### Frontend

The **Frontend** is a React/Redux/Webpack application with that takes lots of artistic license.

- [React](https://facebook.github.io/react/) - Front-end framework view framework.

- [Redux](http://http://redux.js.org) - Unified Application State system.

### Daemon

The **Daemon** is responsible for keeping the server in sync with this Github repo (so **Continuous Integration**), and uses [Github's Repository Webhooks](https://developer.github.com/v3/repos/hooks/) to do so. Alternatives such as using a git remote are also possible, but this has the added benefit of supporting pull requests from here 😁.

- [Rust](https://rustlang.org) - easy to use systems language used for a continuous integration daemon.

- [Iron](http://ironframework.io/) - An Express like extendable web framework for Rust.

### Build

- [TypeScript](http://www.typescriptlang.org/) - Typed JavaScript.

- [Lerna](https://lernajs.io/) - Tool for managing multiple projects in one repo.

- [Webpack](https://webpack.js.org) - Compilation tool for JavaScript.

- [SystemJS](https://github.com/systemjs/systemjs) - an `import()` polyfill.

- [PostCSS](https://github.com/postcss/postcss) - CSS with postprocessing functions applied to its AST.

---

Check out the [blog post where I detail design decisions here](https://alain.xyz/blog/the-making-of-alain-xyz).

A few of the projects that influenced the design of this app were:

- [Wordpress Calypso](https://github.com/Automattic/wp-calypso)

- [TypeScript Samples](https://github.com/Microsoft/TypeScriptSamples/tree/master/imageboard)

- [ReactJS Essentials by Artemij Fedosejev](https://github.com/fedosejev/react-essentials)

- [GatsbyJS](https://www.gatsbyjs.org/)

## License

*All source code* is available with an **MIT license**, feel free to take bits and pieces and use them in your own projects. I would love to hear how you found things useful, feel free to contact me on Twitter [@alainxyz](https://twitter.com/alainxyz).

*All written articles and art* such as blog posts and artwork, etc. are **Copyright Alain Galvan, All Rights Reserved** unless stated otherwise. If you would like to feature them in a research paper however, feel free to use the following bibtex:

```tex
% If you're using a different blog post, replace the title, month, and year appropriately.
@misc{galvan2020,
  title={A Comparison of Modern Graphics APIs},
  url={https://www.alain.xyz/blog/comparison-of-modern-graphics-apis},
  journal={Alain.xyz},
  author={Alain Galvan},
  year={2020}
}
```

[license-img]: https://img.shields.io/:license-mit-blue.svg?style=flat-square
[license-url]: https://opensource.org/licenses/MIT
