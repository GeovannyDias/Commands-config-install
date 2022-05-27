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
## SSL

```
npm set strict-ssl false
npm set strict-ssl true
```

## ERROR: Failed to set up Chromium r782078! Set "PUPPETEER_SKIP_DOWNLOAD" env variable to skip download

[Solve Error:](https://stackoverflow.com/questions/63187371/puppeteer-not-able-to-install-error-failed-to-set-up-chromium-r782078-set-pu)


```
puppeteer not able to install: 

1. Go to project root.
2. Open a terminal and run the following command:

set PUPPETEER_SKIP_DOWNLOAD=true

3. Run: 

npm i
or
npm i --force
```

## Cmder Terminal
* **https://github.com/cmderdev/cmder/wiki#cmder-integration**
* **https://github.com/cmderdev/cmder/wiki/Seamless-VS-Code-Integration**
```
To run Cmder as the VS Code terminal, you may follow these steps:

1. Press Ctrl + , to access VSCode Settings
2. Search for settings.json
3. Click Edit in settings.json
4. Append or modify the following into your configuration file:

"terminal.integrated.profiles.windows": {
    "Cmder": {
         "path": "C:\\WINDOWS\\System32\\cmd.exe",
         "args": ["/K", "C:\\cmder\\vendor\\bin\\vscode_init.cmd"]
     }
}


Example:

"terminal.integrated.profiles.windows": {
        "PowerShell": {
            "source": "PowerShell",
            "icon": "terminal-powershell"
        },
        "Command Prompt": {
            "path": [
                "${env:windir}\\Sysnative\\cmd.exe",
                "${env:windir}\\System32\\cmd.exe"
            ],
            "args": [],
            "icon": "terminal-cmd"
        },
        "Git Bash": {
            "source": "Git Bash"
        },
        "Windows PowerShell": {
            "path": "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
        },
        "Cmder": {
            "path": "C:\\WINDOWS\\System32\\cmd.exe",
            "args": ["/K", "C:\\cmder\\vendor\\bin\\vscode_init.cmd"]
        }
},


Reboot VSC:

Press Ctrl + Shift + P to access VSCode Command Palette
>Termina: Select Default Profile
Select Cmder

```
SQL Server 2029 - SSMS (Connection String)
* **https://docs.microsoft.com/en-us/ef/core/cli/powershell**
```
Server=localhost;Database=master;Trusted_Connection=True;

Al instalar SSMS despliega la cadena de conexión.

Examples:

Scaffold-DbContext "Server=GEOLAP\SQLEXPRESS; Database=Pub; Trusted_Connection=True;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models

Scaffold-DbContext "Server=GEOLAP\SQLEXPRESS; Database=Pub; Trusted_Connection=True;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models -ContextDir


appsettings.json

"ConnectionStrings": {
    "DevConnection": "Server=(local)\\;Database=company_db_01;Trusted_Connection=True;MultipleActiveResultSets=True"
 }
 

DATA DATABASE:
Wide World Importers sample databases for Microsoft SQL

```
