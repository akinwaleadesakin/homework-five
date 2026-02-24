# about

Simple "About" static page project (SCSS → CSS).

## Prerequisites
- Node.js and npm installed

## Install dependencies
From the project root run:
```sh
npm install
```
Or install dev tools directly:
```sh
npm install --save-dev sass gh-pages live-server
```

## Useful npm scripts
Add these to package.json scripts if not present:
```json
{
  "scripts": {
    "serve": "live-server",
    "compile:sass": "sass scss/styles.scss css/styles.css -w",
    "build:sass": "sass scss/styles.scss css/styles.css",
    "predeploy": "npm run build:sass",
    "deploy": "gh-pages -d ."
  }
}
```

## Common commands
- Build CSS once: npm run build:sass
- Watch SCSS: npm run compile:sass
- Serve locally: npm run serve
- Deploy to GitHub Pages (requires repo pushed / repository set in package.json): npm run deploy

## Files to edit
- index.html
- scss/styles.scss (entry)
- scss/variable.scss, scss/structure.scss, scss/components.scss
- css/styles.css (generated)
