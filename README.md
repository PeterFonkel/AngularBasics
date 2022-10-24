# AngularBasics

## 1.Instalación

Para usar Angular debe estar instalado NODE y NPM.

Comprobar instalacion de NODE y NPM:

`node -v`

`npm -v`

En caso de no estar instalado:

NODE

https://nodejs.org/es/download

NPM

`npm install npm@latest -g`

Comprobar instalación de typescript:

`tsc -v`

En caso de no estar instalado:

`npm install -g typescript`

Si da problemas:

`npm cache verify`

`npm cache clean`

Instalar Angular:

`npm install -g @angular/cli`

## 2.Crear un proyecto

`ng new <nombreApp>`

`ng serve -o`

Se abrirá un proyecto Angular por defecto en puerto 4200.

###Instalar Bootstrap, jquery y popper

`npm install bootstrap jquery @popperjs/core`

En el archivo angular.json:

```
"styles": [
  "node_modules/bootstrap/dist/css/bootstrap.min.css",
  "src/styles.scss"
],
"scripts": [
  "node_modules/jquery/dist/jquery.min.js",
  "node_modules/@popperjs/core/dist/umd/popper.min.js",
  "node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```
## 3.Estructura de modulos y componentes

Cada funcionalidad tendrá un módulo diferente:

`ng g m <nombre_modulo> --routing true`

Creamos un contendor de elementos iguales. Le pondremos el nombre en plural:

`ng g c <nombre_modulo>/<nombre_componente_plural>`

Creamos un componente singular:

`ng g c <nombre_modulo>/<nombre_componente_plural><nombre_componente_singular>`






