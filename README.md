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


```
