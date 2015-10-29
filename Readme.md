#OpenOrder

##-Primer Hito-
###Integrantes del proyecto conjunto
- Jose Ignacio Recuerda Cambil
- **Antonio Miguel Pozo Cámara**
- Ignacio Romero Cabrerizo

###Descripción
Proyecto para la gestión de pedidos de pequeña a mediana empresa mediante una aplicación cliente-servidor. El servidor hará de intermediario entre 2 clientes (comercio y usuario) con notificaciones push. El usuario podrá realizar un pedido directamente a través de la aplicación y el comercio será notificado, agilizando el proceso de comunicación entre ambas partes. Se cuenta también con un sistema de gestión de estadísticas para informar a los locales que lo soliciten.

###Descripción del repositorio
Este repositorio alojará todo lo relativo a la parte de estadísticas de pedidos. Localización de clientes, locales y pedidos. Pevisionamiento de carga para los locales que lo soliciten. Información en tiempo real sobre los locales más demandados e información sobre tiempo de entrega de pedido. 
Se utilizará una licencia de Microsoft Azure proporcionada por el profesor de la asignatura.

###Documentación
Enlace para encontrar la descripción e información del proyecto (en construcción).

###Introducción a la aplicación
El proyecto se encuentra en un punto inicial, con forme vaya avanzando su desarrollo se dará la necesidad de utilizar distintas herramientas, las cuales se citarán **aquí**.
No obstante, ya se están utilizando las herramientas que proporciona la plataforma de informática en la nube Microsoft Azure. El servicio tendrá una base de datos interna (MySQL) en la que almacenar los datos obtenidos y una interfaz web a la que tendrán acceso los usuarios que lo soliciten.

###Participación en el certamen de proyectos de libres de la UGR
Este proyecto se ha inscrito en el certamen de proyectos libres de la UGR.



##	-Segundo Hito-
###Integración contínua
Para la integración contínua he utilizado las herramientas que nos ofrece Microsot Azure para ello. A continuación una captura del sistema de integración contínua funcionando:

![integración contínua](http://s2.subirimagenes.com/imagen/previo/thump_9485832imementacioncontinua.png)


###Sistema de pruebas

Instalamos mocha con: npm install -g mocha. Creamos un directorio en el que vamos a alojar los tests, y dentro de este, el fichero test.js que tiene el siguiente contenido:

```
var assert = require("assert");
miweb = require(__dirname+"/../app.js");

describe('Miweb', function(){
    describe('Comentar', function(){
        it('Debe cargar el programa', function(){
            assert(miweb, "Cargado");
        });
    });
});
```

Ejecutamos mocha:
![haciendo test](http://s2.subirimagenes.com/imagen/previo/thump_9485866test.png)
Nota: en los [ejercicios del tema 2](https://github.com/AntonioPozo/IV-2015-16/blob/master/ejercicios/AntonioPozo/Tema2.md) se detalla el proceso de instalación de nvm. 