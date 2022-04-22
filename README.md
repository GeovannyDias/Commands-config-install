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

Command prompt run as administrator.
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

OR:

Create a .env file at the root of the project:

PORT=4200

npx create-react-app my-app --template typescript

npm run start
npm build

SASS:
npm install sass


```

## Variables de entornos en ReactJS
* **https://blogs.encamina.com/piensa-en-software-desarrolla-en-colores/como-gestionar-las-variables-de-entornos-en-reactjs/**
* **https://blog.santiagoporras.com/react-variables-entorno/**
* **https://www.youtube.com/watch?v=_17erZzdDTk**
```
Variables empezar con:

REACT_APP

Ejemplo:

REACT_APP_API_URL=MY_ENV_APIURL

.env
.env.development
.env.production
.env.local
```

## RegExp or RegEx - ES5
* **https://regex101.com/**

```
const patternValue = /^([0-9])*$/; // Integer
const patternValue = /^[0-9]+(.[0-9]{1,2})?$/; // Decimal con coma y con punto
const patternValue = /^[0-9]+([.][0-9]{1,2})?$/; // Decimal solo con punto

const cadena = "hello world!";
const result = /^hello/.test(cadena);
console.log(result); // true

```

## Tutoriales React
* **https://www.youtube.com/watch?v=U_jlqtLX4nE**
* 

## Generate TypeScript Interface from JSON
* **http://json2ts.com/**

```
json2ts
Generate TypeScript Interface from JSON
```

## Angular

```
Instalar Angular CLI :

npm i -g @angular/cli

Actualizar Angular CLI de manera global:

npm uninstall -g @angular/cli
npm cache clean --force
npm i -g @angular/cli
ng --version

CLI:

ng g module components/pages/home -m=app --route home
Crea el módulo, routing y componente (-m=app --route home → Crea la ruta "home" en app-routing.ts)

ng g c components/posts/new-post -m=app
ng g module components/posts/new-post -m=app => Solo crear un "módulo". (Sin rutas)
ng g module components/posts/list-posts -m=app --route posts
ng g c components/posts/post
ng g m app-material -m=app --flat

Create project modules (home, about and contact):

ng g m modules/home --routing → (Crea el módulo y fichero home-routing.ts)
ng g m modules/about --routing
ng g m modules/contact --routing

ng g c modules/home/componente01 --skipTests
ng g c shared/Page404 --skip-tests

ng g m app-material -m=app --flat

ng g m pipes/pipes -m=app --flat
ng g pipe pipes/filter

ng g guard shared/guards/auth

LAZY LOAD:
https://fjmduran.com/blog/lazy_load_angular

HttpInterceptors:
https://dev.to/ricardochl/como-usar-httpinterceptors-en-angular-2o84
```

## Package NPM

```
npm install -g @briebug/jest-schematic
npm install -g yarn
npm install -g typescript

npm install --global yarn

```
