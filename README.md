# Angular2-starter project

This project is a starter app for using Angular 2.0 with Webpack and the packager.

#### To start:

1. Clone the repo
2. Install Node/NPM. (Node version 6.7.0+)
3. Install Yarn `npm install -g yarn`
4. Install angular-cli `npm install -g angular-cli`
5. run `yarn`
6. replace all instances on OpaqueToken in node_modules with InjectionToken (if it requires a type use <object>)
7. run `yarn add @angular/{animations,common,compiler,compiler-cli,core,forms,http,platform-browser,platform-browser-dynamic,platform-server,router}@'^5.2.0' typescript@2.4.2 rxjs@'^5.5.2'`
8. run `yarn start` to start the dev server
9. in webpack.common.js, replace line 100-106 with:
 `    new webpack.ContextReplacementPlugin(
        /angular(\\|\/)core(\\|\/)/,
        helpers.root("src") // location of your src
 )`

#### To build:

1. run `yarn build`
2. the build artefacts will be found in the /angular/dist directory.

#### To lint:

1. run `yarn lint`

#### To run tests:

TESTING WITH KARMA NOT CURRENTLY WORKING

## Third party frameworks and libraries

This is a list of the third party frameworks and libraries that the development team 
will monitor via development mailing lists for vulnerabilities.  Vulnerabilities which 
are found will be addressed in a Pull Request to indicate that the version was changed 
to address the vulnerability.

| Framework/ Library | Version  | License
| ------------------ | -------- | -------
| Angular            | 4.2.x    | MIT
| Bootstrap          | 4.0.x    | MIT
| ngrx/store         | 2.2.x    | MIT
| Jasmine            | 2.4.x    | MIT
| Karma              | 1.4.x    | MIT
| PhantomJS          | 2.1.x    | Apache 2.0
| RxJs               | 5.4.x    | Apache 2.0
| TypeScript         | 2.4.x    | Apache 2.0
| Webpack            | 2.2.x    | MIT
