# Commands, Configuration, Install


## Node and NPM
```
npm cache clean --force
npm cache verify


npm install -g npm


Optional (PowerShell Administrator):

Set-ExecutionPolicy Unrestricted -Scope CurrentUser -Force
npm install -g npm-windows-upgrade
npm-windows-upgrade

NPM NOTICE:
New minor version of npm available! 8.1.2 -> 8.4.0
Changelog: https://github.com/npm/cli/releases/tag/v8.4.0
Run npm install -g npm@8.4.0 to update!

npm install -g npm@8.4.0

```

## NVM | Node version Manager
* **https://github.com/coreybutler/nvm-windows**
```
nvm-setup.zip

nvm
nvm list available
nvm list 

nvm install
nvm install 16.13.2

nvm use 16.13.2

```

## React.js

```
Change PORT, Windows: "set PORT=4200 && react-scripts start", Linux, IOS: "PORT=4200 react-scripts start"

package.json

"scripts": {
    "start": "set PORT=4200 && react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },



npx create-react-app my-app --template typescript

npm run start
npm build

SASS:
npm install sass

```

## RegExp or RegEx - ES5
* **https://regex101.com/**

```
const patternValue = /^([0-9])*$/; // Integer
const patternValue = /^[0-9]+(.[0-9]{1,2})?$/; // Decimal con coma y con punto
const patternValue = /^[0-9]+([.][0-9]{1,2})?$/; // Decimal solo con punto

```

## Tutoriales React
* **https://www.youtube.com/watch?v=U_jlqtLX4nE**
* 
