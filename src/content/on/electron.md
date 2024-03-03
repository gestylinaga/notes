---
title: Electron
category: JavaScript Framework
---

# Electron
**Electron** is a framework for building native *desktop* applications using 
languages typically used for web development:
- [JavaScript 🗒️](/on/javascript)
- [HTML 🗒️](/on/html)
- [CSS 🗒️](/on/css)

This allows developers the ability to maintain a **single** JavaScript codebase 
for creating cross-platform applications, that work on **Windows**, **MacOS**, 
and **Linux**. Electron accomplishes this by embedding 
[Chromium 🌐](https://www.chromium.org/) and [Node.js 🌐](https://nodejs.org/)
into its binary, which while considered inefficient or *'bloated'*, it makes 
desktop applications easy to develop/maintain for web developers.

In Electron, you build front-ends just like you would for a browser-based web 
app (optionally using front-end frameworks like: Vuejs, Svelte, Angular), while 
also having access to Node.js for low-level, back-end APIs.

Some popular apps created with Electron:
- [Discord 🌐](https://discord.com/)
- [Slack 🌐](https://slack.com/)
- [Visual Studio Code 🌐](https://code.visualstudio.com/)

## Install
1. In a terminal:
```bash
mkdir your-electron-app && cd your-electron-app # creates an empty directory
# NOTE: entry point should be set to `main.js` in next step:
npm init # creates an npm project in your new directory
npm install --save-dev electron # saves/installs electron as a dependency
touch main.js # creates a JavaScript file; the main entry point to your app
```
2. In the newly created `package.json` file, add this script option:
```json
{
  "scripts": {
    "start": "electron ."
  }
}
```
  - This allows you to run `npm start` in a terminal to run your app in 
  development mode

## Usage
*Boilerplate* example project from 
[ElectronJS Quick-Start 🌐](https://www.electronjs.org/docs/latest/tutorial/quick-start):

`main.js`:
```js
// Modules to control application life and create native browser window
const { app, BrowserWindow } = require('electron');
const path = require('node:path');

const createWindow = () => {
  // Create the browser window.
  const mainWindow = new BrowserWindow({
    width: 800,
    height: 600,
    webPreferences: {
      preload: path.join(__dirname, 'preload.js')
    }
  })

  // and load the index.html of the app.
  mainWindow.loadFile('index.html')

  // Open the DevTools.
  // mainWindow.webContents.openDevTools()
}

// This method will be called when Electron has finished
// initialization and is ready to create browser windows.
// Some APIs can only be used after this event occurs.
app.whenReady().then(() => {
  createWindow()

  app.on('activate', () => {
    // On macOS it's common to re-create a window in the app when the
    // dock icon is clicked and there are no other windows open.
    if (BrowserWindow.getAllWindows().length === 0) createWindow()
  })
})

// Quit when all windows are closed, except on macOS. There, it's common
// for applications and their menu bar to stay active until the user quits
// explicitly with Cmd + Q.
app.on('window-all-closed', () => {
  if (process.platform !== 'darwin') app.quit()
})

// In this file you can include the rest of your app's specific main process
// code. You can also put them in separate files and require them here.
```
`preload.js`
```js
// preload.js

// All the Node.js APIs are available in the preload process.
// It has the same sandbox as a Chrome extension.
window.addEventListener('DOMContentLoaded', () => {
  const replaceText = (selector, text) => {
    const element = document.getElementById(selector)
    if (element) element.innerText = text
  }

  for (const dependency of ['chrome', 'node', 'electron']) {
    replaceText(`${dependency}-version`, process.versions[dependency])
  }
})
```
`index.html`
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <!-- https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP -->
    <meta http-equiv="Content-Security-Policy" content="default-src 'self'; script-src 'self'">
    <title>Hello World!</title>
  </head>
  <body>
    <h1>Hello World!</h1>
    We are using Node.js <span id="node-version"></span>,
    Chromium <span id="chrome-version"></span>,
    and Electron <span id="electron-version"></span>.

    <!-- You can also require other files to run in this process -->
    <script src="./renderer.js"></script>
  </body>
</html>
```


## More External Links
- [Official Site 🌐](https://www.electronjs.org/)
- [Official Docs 🌐](https://www.electronjs.org/docs/latest/)
- [Official GitHub Repo 🌐](https://github.com/electron/electron)
