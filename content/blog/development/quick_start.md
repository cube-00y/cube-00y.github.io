---
title: 'Quick Start'
date: 2020-07-05 17:21:13
category: 'κ°λ°λΈνΈ'
draft: false
---

# Getting Started π

## 1. Create a Gatsby site.

```sh
# create a new Gatsby site using the blog starter
$ npx gatsby new my-blog-starter https://github.com/JaeYeopHan/gatsby-starter-bee
```

> If you are not using `npx`, following [Gatsby Getting Started](https://www.gatsbyjs.org/docs/quick-start)

```sh
$ npm install -g gatsby-cli
$ gatsby new my-blog-starter https://github.com/JaeYeopHan/gatsby-starter-bee
```

## 2. Start developing.

```sh
$ cd my-blog-starter/
$ npm start
# open localhost:8000
```

## 3. Add your content

You can write...

- contents to blog in `content/blog` directory.
- resume `content/__about` directory.

> With markdown syntax and some meta data

### Support script for creating new post

![](./images/cli-tool-example.gif)

```sh
$ npm run post
```

## 4. Fix meta data

You can fix meta data of blog in `/gatsby-meta-config.js` file.

## 5. Publish with [netlify](https://netlify.com)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/JaeYeopHab/gatsby-starter-bee)

:bulb: if you want to deploy github pages, add following script to package.json

```json
"scripts": {
    "deploy": "gatsby build && gh-pages -d public -b master -r 'git@github.com:${your github id}/${github page name}.github.io.git'"
}
```

# :memo: Write a post!

```
content
βββ __about
βββ blog
```

- You can register your resume on the web. (in `__about` directory)
- You can register your post. (in `blog` directory)

# π§ Customize!

## Gatsby config

```
/root
βββ gatsby-browser.js // font, polyfill, onClientRender ...
βββ gatsby-config.js // Gatsby config
βββ gatsby-meta-config.js // Template meta config
βββ gatsby-node.js // Gatsby Node config
```

## Structure

```
src
βββ components // Just component with styling
βββ layout // home, post layout
βββ pages // routing except post: /(home), /about
βββ styles
β   βββ code.scss
β   βββ dark-theme.scss
β   βββ light-theme.scss
β   βββ variables.scss
βββ templates
    βββ blog-post.js
    βββ home.js
```

## Style

You can customize color in `src/styles` directory.

```
src/styles
βββ code.scss
βββ dark-theme.scss
βββ light-theme.scss
βββ variables.scss
```

> Welcome to gatsby-starter-bee!
> Happy blogging! π»
