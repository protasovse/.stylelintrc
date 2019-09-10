# [Stylelint](https://stylelint.io/)

Stylelint is a config that will lint styling in a project.

This repo consists of [my](https://jackdomleo.dev) preferred configuration for styling. Use https://stylelint.io/ to edit your config to how you wish.  

## Setup

- Copy the `.stylelintrc` file into your project
- In the command line, run `npm i stylelint stylelint-order stylelint-scss --save-dev` to install the packages used in the `.stylelintrc` file
- In your `package.json` file, under "scripts", add the following lines:
  - `"stylelint": "stylelint \"**/*.(scss|css)\""`
  - `"stylelint:fix": "stylelint \"**/*.(scss|css)\" --fix"`
- Edit the file types you want to lint. I.e.:
  - `*.css`
  - `*.scss`
  - `*.sass`
  - `*.less`
  - `*.vue`
  - `*.html`
- In the command line, run:
  - `npm run stylelint` to highlight styling errors
  - `npm run stylelint:fix` to autofix as many styling errors as it can and then highlight styling errors it was not able to autofix
  
---

## Stylelint plugins

- [stylelint-order](https://github.com/hudochenkov/stylelint-order)
- [stylelint-scss](https://github.com/kristerkari/stylelint-scss)
