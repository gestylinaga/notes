---
layout: ../../layouts/MarkdownLayout.astro
title: Jest
---

# Jest
**Jest** is a JavaScript Testing Framework, made by Facebook,  with a focus on 
simplicity. It aims to work out of the box, config free, on most JavaScript 
projects.

**Jest** has support / docs for projects using:
  - [TypeScript](/on/typescript)
  - Babel
  - Node
  - React
  - Angular
  - Vue
  - and more

and is used extensively at these major companies:
  - Facebook
  - Twitter
  - The New York Times
  - Spotify
  - AirBnB
  - Instagram
  - and more

## Install
```bash
# installing to local npm directory
npm install --save-dev jest 

# installing globally on system
npm install jest --global
```

## Usage
A simple hypothetical function that adds two numbers called `sum.js`:
```javascript
// example function to be tested:
function sum(a, b) {
  return a + b;
}

module.exports = sum;
```
The test file, `sum.test.js`, that contains the actual tests:
```javascript
const sum = require('./sum');

test('adds 1 + 2 to equal 3', () => {
  expect(sum(1, 2)).toBe(3);
})
```
Add the following section to the local `package.json` file:
```json
{
  "scripts": {
    "test": "jest"
  }
}
```
Which allows you to run `npm test` or `yarn test` to output the message:
```
PASS  ./sum.test.js
✓ adds 1 + 2 to equal 3 (5ms)
```

### Generating a config file
**Jest** works fine without a config, but one can be generated to add 
functionality:
```bash
jest --init
```
This command will ask some questions based on your project, and generate a basic
configuration file with a short description for each option.

## More External Links
- [Official Site](https://jestjs.io/)
- [Official Docs](https://jestjs.io/docs/getting-started)
- [GitHub Repo](https://github.com/facebook/jest)
