
Iniciando en el mundo de los polyfills
================

> **Note**. En este proyecto inicio en el mundo de los polyfills (siento la mezcla de idiomas)

## ¿Cómo utilizarlo?
Lo primero que hice fue:

> **Note**. Recuerda instalar Node y npm

```bash
npm install -g bower
bower init
```

Después cree el index.html

### Install polyfills

```bash
npm install @webcomponents/webcomponentsjs
npm init
npm i
```
You can also load the code from a CDN such as unpkg: https://unpkg.com/@webcomponents/webcomponentsjs@^2/

### Using `webcomponents-bundle.js`

The `webcomponents-bundle.js` contains all of the web components polyfills and is
suitable for use on any supported browser. All of the polyfill code will be loaded
but each polyfill will only be used based on feature detection.
The bundle includes Custom Elements, Shady DOM/CSS and generic platform polyfills
(such as ES6 Promise, Constructable events, etc.) (needed by Internet Explorer 11),
and Template (needed by IE 11 and Edge).

The `webcomponents-bundle.js` is very simple to use but it does load code
that is not needed on most modern browsers, slowing page load. For best performance,
use the `webcomponents-loader.js`.

Here's an example:

```html
<!-- load webcomponents bundle, which includes all the necessary polyfills -->
<script src="node_modules/@webcomponents/webcomponentsjs/webcomponents-bundle.js"></script>

<!-- load the element -->
<script type="module" src="my-element.js"></script>

<!-- use the element -->
<my-element></my-element>
```

### Levantar localhost

```bash
sudo npm i -g http-server
```

y para arrancar en localhost

```bash
http-server
```