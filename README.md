__NOTICE:__
Just like with the boilerplate project, we are working on rewriting this with TypeScript.  We'd still love for you to use this and submit PRs, so have at it!

# React Library Starter
This project can be used to create your next React Component library.  It's configured to give you a starting place for publishing react components to NPM.

## Getting Started
1. `yarn` or `npm install` if you're old fashioned
2. Develop components within the `src` directory.  Make sure to export the ones you want in your library from `src/index.js`
3. Set your libraries name within the root level webpack configuration file's output object and in the package.json.

```
  output: {
    path: path.resolve(__dirname, 'dist'),
    filename: 'index.js',
    library: 'react-library-starter', // your library's name goes here
    libraryTarget: 'umd',
    umdNamedDefine: true,
  },
```
4. Increment the version of your package with `npm version x.x.x`
5. Run `npm publish` with your code checked into to git and watch as your npm library is born!

## Example App
It's often the case that you want to test your components out with an example app before publishing.

Included in this setup is a setup to do just that.

### Getting Started
1. `cd example/app && yarn`
2.  Within the example/app directory, you will find a setup that you can use to test your app.  Import your components from `components` and use them within the App.js file.
3. Run `npm run start` and navigate to `http://localhost:3000 to see your app`

## Example usage
- [Grommet CMS Content Blocks](https://github.com/grommet/grommet-cms-content-blocks)
- [Grommet Forms](https://github.com/RyanCCollins/grommet-forms)
