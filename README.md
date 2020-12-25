
<img  align="left" width="150" style="float: left;" src="https://www.upm.es/sfs/Rectorado/Gabinete%20del%20Rector/Logos/UPM/CEI/LOGOTIPO%20leyenda%20color%20JPG%20p.png">
<img  align="right" width="60" style="float: right;" src="http://www.dit.upm.es/figures/logos/ditupm-big.gif">

<br/><br/><br/>

# nosql_pouchdb_bdfi
## Antes de empezar: Consejos
1. Instalar Couchdb en WINDOWS directamente instalando el programa descargando el "apache-couchdb-3.1.1.msi"
(Intentando hacerlo funcionar en docker me llevó 1 hora y no lo conseguí, de esta forma se tardan 2 minutos)
2. Entrando en la interfaz web de couchdb creamos desde ahí la base de datos "todos_remote"
3. Activar el CORS: en configuración cambiar en Main config > "enable_cors = true" y marcar en CORS > All domains ( * )
4. En los permisos de la base de datos "todos_remote" acceder a sus permisos y quitar todos los usuarios que haya en members y admins, tanto en users como roles

Siguiendo estos pasos corriendo el autocorector debería pasar todos los prechecks

## Pasos a seguir

1. añadir 
```
<script src="//cdn.jsdelivr.net/npm/pouchdb@7.1.1/dist/pouchdb.min.js"></script>
```
a index.html

## Objetivos
 * Objetivo 1
 * Objetivo 2
## Descripción de la práctica

A completar por el profesor


## Descargar el código del proyecto

El proyecto debe clonarse en el ordenador desde el que se está trabajando:

```
$ git clone https://github.com/ebarra/nosql_pouchdb_bdfi
```
A continuación se debe acceder al directorio de trabajo y abrir el fichero index.html con el editor de la elección del alumno.

```
$ cd nosql_pouchdb_bdfi
```
## Prueba de la práctica 

Para ayudar al desarrollo, se provee una herramienta de autocorrección que prueba las distintas funcionalidades que se piden en el enunciado. Para utilizar esta herramienta debes tener node.js (y npm) ([https://nodejs.org/es/](https://nodejs.org/es/)) y Git instalados. 

Para instalar y hacer uso de la [herramienta de autocorrección](https://www.npmjs.com/package/autocorector) en el ordenador local, ejecuta los siguientes comandos en el directorio del proyecto:


```
$ npm install -g autocorector     ## Instala el programa de test
$ autocorector                    ## Pasa los tests al fichero a entregar
............................      ## en el directorio de trabajo
... (resultado de los tests)
```
También se puede instalar como paquete local, en el caso de que no se dispongas de permisos en el ordenador desde el que estás trabajando:
```
$ npm install autocorector     ## Instala el programa de test
$ npx autocorector             ## Pasa los tests al fichero a entregar
............................   ## en el directorio de trabajo
... (resultado de los tests)
```

Se puede pasar la herramienta de autocorrección tantas veces como se desee sin ninguna repercusión en la calificación.

## Instrucciones para la Entrega y Evaluación.

Una vez satisfecho con su calificación, el alumno puede subir su entrega a Moodle con el siguiente comando:
```
$ autocorector --upload
```
o, si se ha instalado como paquete local:
```
$ npx autocorector --upload
```

La herramienta de autocorrección preguntará por el correo del alumno y el token de Moodle. En el enlace [https://www.npmjs.com/package/autocorector](https://www.npmjs.com/package/autocorector) se proveen instrucciones para encontrar dicho token.

