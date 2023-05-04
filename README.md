# NodeJs - NPM - NVM 🖥️
## Guía para la Instalación de los controles de paquetes y versiones de Node JS - Ubuntu 22.04.1 LTS WSL2
___
### Proyecto realizado con el curso de platzi: https://platzi.com/clases/3578-npm/
___
## npm-init
---
### Instalación de Paquetes y Requerimientos
- Instalación de Node 20.1.0, NPM 9.6.4 y NVM 0.39.0
~~~
- sudo apt-get install -y node.js
- curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash  (No es obligatorio, solo en caso de que node no este en su última versión)
- sudo apt-get update
- sudo apt-get upgrade
- node -v
- npm -v
- nvm -v
- nvm install 20.1.0 (Depende de la última versión)
~~~
### Iniciar npm
~~~
- npm init
- npm init -y (En caso de ser de un repositorio clonado o migrado)
~~~
### Instalar Dependencias ya Preasignados en el archivo: package.json
~~~
- npm install
~~~
### Visualizar Paquetes Instalados
~~~
- npm list 
- npm list -g
~~~
### Instalación de Dependencias (Ejemplos)
~~~
- npm install moment
- npm install eslint --save-dev
- npm install eslint -D
~~~
### Instalar React
~~~
- npm install react
(Opcionales)
- npm install react -S
- npm install react --save
~~~
### Instalar Paquetes Globales
~~~
    (Ejemplo)
- npm install -g cowsay
- cowsay Holis
~~~
### Instalación de Dependencias de Versiones Específicas
~~~
- npm install eslint -o
- npm install react-dom --dry-run
- npm install json-server@0.15.0
- npm install json-server@latest
- npm install react@latest
~~~
### Scripts en npm
~~~
- mkdir src
- cd src
- touch index.js (Agregar un console.log('Hola Mundo'); en index)
(Cambiar el "test" en package.json por "start":"node src/index.js")
- npm run start
- npm start
(Se pueden agregar los scripts que se requiera en la seccion de scripts del package.json)
~~~
---
## react-npm (Correr Servidor con React)
---
### npx
~~~
- npx create-react-app react-app
- cd react-app
- npm start
~~~
### Ver que paquetes pueden ser actualizados, reparados o remplazados
~~~
- npm outdate
- npm audit 
- npm audit fix
- npm audit fix --force
~~~
### Eliminar Dependencias
~~~
- npm uninstall ladependenciaadesinstalar
(También se pueden eliminar manualmente desde el package.json)
~~~
### Crear modulo para npm
- https://platzi.com/clases/3578-npm/52463-crear-un-paquete/