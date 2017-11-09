# coreui reactjs + create-react-app

This is just a boilerplate/sample,
how to integrate `coreui` in `create-react-app`.

**note**, that sass can't be compiled in `create-react-app` by default. So here i implement with `node-sass-chokidar`

mostly its just make compilation for sass to css, in `src/styles/css`, and react include css files, instead of sass

## Some Changes

1. it only implement `npm-run-all` and `node-sass-chokidar`, see `package.json`.
2. scss files located in `src/styles/scss`. And will be compiled to `src/styles/css`. almost no changes. 
3. for img directory in `src/styles/img`. It just an images used in css files. react really use that files. so better separation between images for css files, and images in public directory.
4. how i implement the css files. see `src/index.js` :-)
5. just compile as usual with `yarn` or `npm install`, then run on `yarn run start` or `npm run start`.
6. \*if build `start` not compile css files. Maybe it because of watch mode, try to edit something in `scss` files, to see if it will compile.

## Reference

- [coreui reactjs](https://github.com/mrholek/CoreUI-React)
- [Adding a CSS Preprocessor (Sass, Less etc.)](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-a-css-preprocessor-sass-less-etc)
