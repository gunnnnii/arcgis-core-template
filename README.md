# ArcGIS API for JavaScript template

## Prerequisites

* Node.js 16.0+

## Run project locally

To start:

```
npm install
npm run dev
```

Then open your browser at http://localhost:3002/

## Create productive build

```
npm run build
```

The `dist` folder then contains all the files for the web app which can either be copied to a web server or pushed to the `gh-pages` branch to be served at `https://arnofiva.github.io/arcgis-core-template`.

In order to use the `gh-pages` approach, you have to do the following once. Remove `dist` folder if it has been created from a previous build.

```
git worktree add dist gh-pages
```

After that it's the following to create and deploy a new build:

```
npm run build
cd dist
git add .
git commit -am '🎉'
git push origin gh-pages
```
