# Semana1

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 18.2.6.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.


## Como funciona el Pipe personalizado

Importamos las dependencias necesarias y proseguimos a poner la logica del pipe.

Vamos a tomar el valor inicial (que es un string) para poder separarlo en un array (lo separamos por espaciado)

"Hola como estas" -> ["Hola", "como", "estas"]

Despues le pasamos 2 funciones map, una para pasar a minusculas todas las letras de cada palabara

["Hola", "como", "estas"] -> ["hola", "como", "estas"]

La otra es para poner la primera letra de cada palabra en mayuscula

["hola", "como", "estas"] -> ["Hola", "Como", "Estas"]

De ahi, le pasamos un reduce para unir todas las palabras en un string

["Hola", "Como", "Estas"] -> "HolaComoEstas"

Por ultimo en la variable camelCase hacemos que la primera letra del string sea minuscula y que nos la devuelva junto con todas las demas letras.

"HolaComoEstas" -> "holaComoEstas"