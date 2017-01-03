# notebook

A simple boilerplate app to demonstrate how to use [ES6] and [React] with
[Electron]. It uses [Babel] to automatically transpile ES6 and JSX code,
without depending on any package manager besides `npm`.

## How?

The main entry point is `boostrapper.js`, which registers Babel and loads the
real entry point `main.js`. This is necessary to allow `main.js` to make use of
Babel's features.

The renderer entry point `index.html` does basically the same, but loads the
`scripts/main.js` file, which renders the `components/main.jsx` component into the `body`.

## Installation

```bash
git clone https://github.com/jochen-oko/notebook.git
cd notebook
npm install
npm start
```

[ES6]: http://exploringjs.com/
[React]: https://facebook.github.io/react/
[Electron]: http://electron.atom.io/
[Babel]: http://babeljs.io
