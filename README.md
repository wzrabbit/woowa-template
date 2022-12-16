# woowa-template  
## npm-install
```
npm install
npm install eslint --save-dev
npx eslint --init
npm install prettier --save-dev
npm install eslint-config-prettier --save-dev
npm install eslint-plugin-prettier --save-dev
```
## eslintrc.js
```JavaScript
module.exports = {
  env: {
    browser: true,
    commonjs: true,
    es2021: true,
  },
  extends: ['airbnb-base', 'plugin:prettier/recommended'],
  overrides: [],
  parserOptions: {
    ecmaVersion: 'latest',
  },
  rules: {
    'max-depth': ['error', 2],
    'max-lines-per-function': ['error', 12],
    'lines-between-class-members': ['error', 'always', { exceptAfterSingleLine: true }],
  },
};
```
## prettierrc  
```JavaScript
{
  "trailingComma": "es5",
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true,
  "printWidth": 100
}
