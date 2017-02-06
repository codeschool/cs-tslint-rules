# cs-tslint-rules

This repo contains the TSLint rule configuration for Code School projects that
use TypeScript as well as TypeScript + Angular 2.

## Installation

The instructions differ for plain TypeScript projects and for Angular 2 +
TypeScript projects, so follow the instructions that apply to your
project type.

### Basic Installation

Install TSLint and TypeScript for your project.

```
npm i --save-dev typescript tslint
```

Install the cs-tslint-rules module.

```
npm i --save-dev git+https://github.com/codeschool/cs-tslint-rules.git
```

Create a `tslint.json` file in the root folder of your project and add
the following:

``` json
{
  "exclude": [
    "node_modules/"
  ],
  "extends": "cs-tslint-rules/tslint-base"
}
```

### Angular 2 Installation

Install TSLint, Codelyzer and TypeScript for your project.

```
npm i --save-dev typescript tslint codelyzer
```

Install the cs-tslint-rules module.

```
npm i --save-dev git+https://github.com/codeschool/cs-tslint-rules.git
```

Create a `tslint.json` file in the root folder of your project and add
the following:

``` json
{
  "exclude": [
    "node_modules/"
  ],
  "rulesDirectory": [
    "node_modules/codelyzer"
  ],
  "extends": "cs-tslint-rules/tslint-ng2"
}
```

## Usage

Add a script to the `scripts` section of your `package.json`, making sure to
set the correct pattern for your source files (the example uses `src/**/*.ts`):

``` json
{
  "scripts": {
    "lint": "./node_modules/.bin/tslint --type-check --project tsconfig.json --config tslint.json src/**/*.ts"
  }
}
```

If you have a build script then you should modify it so that the linting is
done before the project can be successfully built. For example, you could
prepend the linting command to your build command to make sure the linting
is run first.

```
npm run lint
```
