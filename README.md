# JSON

**JavaScript Object Notation (JSON)** es un formato basado en texto estándar para representar datos estructurados en la sintaxis de objetos de JavaScript. Es comúnmente utilizado para transmitir datos en aplicaciones web (por ejemplo: enviar algunos datos desde el servidor al cliente, así estos datos pueden ser mostrados en páginas web, o vice versa).

Un objeto JSON puede ser almacenado en su propio archivo, que es básicamente sólo un archivo de texto con una extensión ***.json.***

Por otro lado cuando enviamos datos de un sistema a otro, por lo general se envía la información de lo que se esta enviando, a esto se le llama los mime type, y cuando se crea el archivo normalmente se le da el nombre de application/json

¿Para qué se usa JSON?

JSON es un lenguaje para representar datos, con la sintaxis propia de los literales de objetos Javascript. Sus usos son varios, pero principalmente serían los siguientes:

- Compartir y transferir información entre distintos sistemas de software.

  -- Las aplicaciones frontend requieren datos para representar al usuario.

  -- Mediante Javascript realizan solicitudes HTTP a un endpoint (URL) en el backend. Estas solicitudes se realizan de manera asíncrona mediante Ajax.

  -- El backend recibe la solicitud sobre el dato que se requiere desde el frontend, o la operación que se desea realizar (ediciones, inserciones, etc.)

  -- El backend realiza la operación, enviando el resultado al frontend en formato JSON.

  -- El frontend recibe el JSON y generalmente construye mediante Javascript el HTML necesario para representar esa información convenientemente al usuario.

- Almacenar información en sistemas de persistencia.

## Reglas de JSON

  - Pares clave / valor.

    -- Cuando nosotros tenemos datos, los podemos representar poniendo un nombre a la variable (key), y una propiedad a esta (value). ->   name: "Jhoswe" profesion: "Programador" edad: 32 casado: true

    -- JSON requiere usar comillas dobles para las cadenas y los nombres de propiedades. Las comillas simples no son válidas.

    -- Toda variable siempre debe tener un valor; debemos tener en cuenta que es diferente un string vacío a que una key no tenga un valor.

    -- Poner todos los pares de clave - valor entre llaves ya que de esta manera decimos que todos los datos que están dentro pertenecen a una entidad.

    -- Una coma o dos puntos mal ubicados pueden producir que un archivo JSON no funcione. Se debe ser cuidadoso para validar cualquier dato que se quiera utilizar, a la vez el ultimo valor de una variable ya no debe llevar comas.
  
  - JSON es sólo un formato de datos — contiene sólo propiedades, no métodos.

  - JSON no admite comentarios

## Tipos de datos de JSON

 - Un valor primitivo, que pueden ser de tipos diversos de Javascript, numérico, cadena de caracteres, y boleanos (true / false).

 -  Arrays, es decir, una secuencia de valores separados por comas. En los arrays utilizamos los corchetes para delimitar el principio y fin de los valores que contienen.

 - Objetos, es decir, otros elementos JSON con pares clave / valor.

 - Además, también es válido el valor null.

## Métodos

 - JSON.stringify(obj, props, spaces) -> Este método nos ayuda a convertir un objeto Javascript a JSON también se puede realizar fácilmente haciendo uso del método JSON.stringify().
Este método dificil de pronunciar viene a ser algo así  como «convertir a texto», y lo podemos utilizar para transformar un objeto de Javascript a JSON rápidamente.

- JSON.parse(str) -> Este método es una acción que analiza un string que contiene un JSON válido y devuelve un objeto Javascript con dicha información correctamente estructurada, en pocas palabras nos ayuda a convertir una cadena en formato JSON a objeto Javascript, y a esta acción se le suele denominar parsear.
Para ello, utilizaremos el mencionado método JSON.parse()

<br>
<br>
<br>

# Ajax

AJAX significa JavaScript asíncrono y XML (Asynchronous JavaScript and XML). Es un conjunto de técnicas de desarrollo web que permiten que las aplicaciones web funcionen de forma asíncrona, procesando cualquier solicitud al servidor en segundo plano, En palabras, Ajax permite acceder a datos existentes en el servidor sin necesidad de recargar la página completamente, estas consultas contra el servidor se realizan por medio de Javascript y los datos se procesan mediante éste mismo lenguaje, permitiendo actualizar el contenido de la página justamente donde sea preciso.

## XML

XML es un lenguaje de marcado similar a HTML. Significa Extensible Markup Language (Lenguaje de Marcado Extensible) y es una especificación de W3C como lenguaje de marcado de propósito general. Esto significa que, a diferencia de otros lenguajes de marcado, XML no está predefinido, por lo que debes definir tus propias etiquetas. El propósito principal del lenguaje es compartir datos a través de diferentes sistemas, como Internet.

## Asíncrono

Asíncrono es todo proceso que tarda un tiempo en realizarse y que, durante ese tiempo, el motor de Javascript puede estar desocupado o realizando otras tareas. Cuando el proceso termina, entonces el motor de Javascript recibe una señal de recuperación y posiblemente un dato como respuesta, pudiendo seguir con la ejecución de código, así como realizar el tratamiento que corresponda sobre el dato recibido como respuesta.

## ¿Cómo funciona AJAX?

Ten en cuenta que AJAX no es una sola tecnología, ni es un lenguaje de programación. Como se dijo antes, AJAX es un conjunto de técnicas de desarrollo web. El sistema generalmente comprende.

- HTML/XHTML para el lenguaje principal y CSS para la presentación.

- El Modelo de objetos del documento (DOM) para datos de visualización dinámicos y su interacción.

- XML para el intercambio de datos y XSLT para su manipulación. Muchos desarrolladores han comenzado a reemplazarlo por JSON porque es más similar a JavaScript en su forma.

- El objeto XMLHttpRequest para la comunicación asíncrona.

- Finalmente, el lenguaje de programación JavaScript para unir todas estas tecnologías.

### Modelo convencional 

1. Se envía una solicitud HTTP desde el navegador web al servidor.

2. El servidor recibe y, posteriormente, recupera los datos.

3. El servidor envía los datos solicitados al navegador web.

4. El navegador web recibe los datos y vuelve a cargar la página para que aparezcan los datos.

Durante este proceso, los usuarios no tienen más remedio que esperar hasta que se complete todo el proceso. No solo consume mucho tiempo, sino que también supone una carga innecesaria en el servidor.

### Modelo AJAX

1. El navegador crea una llamada de JavaScript que luego activará XMLHttpRequest.

2. En segundo plano, el navegador web crea una solicitud HTTP al servidor.

3. El servidor recibe, recupera y envía los datos al navegador web.

4. El navegador web recibe los datos solicitados que aparecerán directamente en la página. No se necesita recargar.

## HTTP

El http (del inglés HyperText Transfer Protocol o Protocolo de Transferencia de Hiper Textos) es el protocolo de transmisión de información de la World Wide Web, es decir, el código que se establece para que el computador solicitante y el que contiene la información solicitada puedan “hablar” un mismo idioma a la hora de transmitir información por la red.
