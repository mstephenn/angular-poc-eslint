# PocAngular

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.26.

## For adding to the existing project

Install these dependencies

```
$ npm install --save-dev eslint eslint-plugin-import @typescript-eslint/eslint-plugin prettier eslint-plugin-prettier @typescript-eslint/parser husky lint-staged

```

Copy the following files

- .eslintrc.json
- .prettierrc.js

Add the following command to the scripts.
```
"lint": "eslint '*/**/*.{js,ts,tsx}' --quiet --fix"
```

Add the following code to the `package.json` file.

```
"husky": {
  "hooks": {
    "pre-commit": "lint-staged"
  }
},
"lint-staged": {
  "*.{js,ts,tsx}": [
    "eslint --fix"
  ]
}
  ```
Finally copy the code from `.vscode > settings.json` vscode settings for auto format on save. And add the following extenstions to the vs code.

```
dbaeumer.vscode-eslint
esbenp.prettier-vscode
```

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
