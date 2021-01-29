# [Boilerplate Code](https://appseed.us/boilerplate-code) 11ty

> Eleventy (11ty) seed project - Features:

- UI Kit: **Pixel Lite** (Free Version) by **Themesberg**
- Render Engine: Nunjunks
- CSS Pipeline (Sass, CleanCSS)
- JS Bundling (Webpack)
- SVG Icon Sprite Generation
- Critical CSS, HTML Minification
- Support via **Github** and [Discord](https://discord.gg/fZC6hup).

<br />

**Credits**

- Initially forked from [Eleventastic](http://github.com/maxboeck/eleventastic) / [Max Böck](https://github.com/maxboeck)
- More **11ty** inspiration from: [EleventyOne](https://github.com/philhawksworth/eleventyone), [Supermaya](https://github.com/MadeByMike/supermaya) 

<br />

> Links

- [Jinja Pixel Lite](https://appseed.us/jinja-template/jinja-template-pixel-uikit) - Product page
- [Jinja Pixel Lite Demo](https://jinja-pixel-lite.appseed-srv1.com/) - LIVE Demo

<br />

![Eleventy Starter - Template project provided by AppSeed.](https://raw.githubusercontent.com/app-generator/boilerplate-code-11ty/master/media/boilerplate-code-11ty-screen.png)

<br />

## Build from sources

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/boilerplate-code-11ty.gti
$ cd jinja-boilerplate-code-11ty
$
$ # Install modules
$ npm install # OR `yarn`
$
$ # Start for development
$ npm start # OR `yarn start`
$
$ # Access the project in browser:
$ # http://127.0.0.1:8080/ 
$
$ # Production Build
$ npm build # OR `yarn build`
```

<br />

## Codebase structure

The project has a simple structure, represented as bellow:

```bash
< PROJECT ROOT >
   |
   |-- src/
   |    |-- data/
   |    |    |-- meta.json            # Provides META information 
   |    |    |-- app.json             # Provides APP information
   |    |
   |    |-- includes/                 # Page chunks, components
   |    |    |-- navigation.html      # Top bar
   |    |    |-- sidebar.html         # Left sidebar
   |    |    |-- scripts.html         # JS scripts common to all pages
   |    |    |-- footer.html          # The common footer
   |    |
   |    |-- layouts/                  # App Layouts (the master pages)
   |    |    |-- base.html            # Used by common pages like index, UI
   |    |    |-- base-fullscreen.html # Used by auth pages (login, register)
   |    |   
   |    |-- index.html                # The default page
   |    |-- *.html                    # All other pages provided by the UI Kit
   |
   |-- utils/                         # JS Helpers
   |
   |-- run.py
   |
   |-- ************************************************************************
```

<br />

## Deploy a fork of this template to Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/app-generator/boilerplate-code-11ty)

## CSS

Styling works with Sass. The main index file is in `src/static/assets/styles/main.scss`. Import any SCSS code you want in there; it will be processed and optimized. The output is in `dist/static/assets/styles/main.css`

## JS

Javascript can be written in ES6 syntax. The main index file is in `src/static/assets/scripts/main.js`. It will be transpiled to ES5 with babel, bundled together with webpack, and minified in production. The output is in `dist/static/assets/scripts/main.js`

## SVG Icons

All SVG files added to `src/static/assets/icons` will be bundled into a `symbol` sprite file. The SVG filename will then be used as the symbol identifier and the icon can be used as a shortcode.

For example, if you have a `github.svg` file in that folder, you can display it anywhere by using `{% icon "github" %}` in your templates.

## Critical CSS

Currently, critical CSS will only be inlined in the head of the homepage. This is done by using the [critical](https://github.com/addyosmani/critical) package in an automatic transform.

<br />

---
[Boilerplate Code](https://appseed.us/boilerplate-code) 11ty - Provided by **AppSeed** [App Generator](https://appseed.us/app-generator).
