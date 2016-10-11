This repo is to demonstrate [Yarn](https://yarnpkg.com) issue [#616](https://github.com/yarnpkg/yarn/issues/616) affecting [v0.15.1](https://github.com/yarnpkg/yarn/tree/v0.15.1) that I have experienced running Node v6.2.0 on Mac OSX 10.11.5. When using `yarn` to install dependencies into an uncreated node_modules folder, the bower_components folder is emptied out.

### Steps to Reproduce
- clone this repo to your machine
- `bower install` - the `bower_components` folder should be created with a single `bourbon` folder
- `yarn` - the `node_modules` folder should be created with a single `wrappy` folder, but the `bower_components` folder will now be empty
