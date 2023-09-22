# Explorando los Fundamentos del Desarrollo Web en Entornos de Cliente

## Modelos de Arquitectura web

Antes de hablar de los diferentes Modelos de Arquitectura Web, vamos a definir qué es la Arquitectura Web. Según una entrada escrita por Ivan de Souza en RockContent:

> ***La arquitectura web es la planificación y el diseño de los componentes técnicos, funcionales y visuales de un sitio web,** antes de que sea diseñado, desarrollado e implementado.*

Hay diversos tipos de arquitectura web, de los cuales vamos a destacar algunos de ellos:

* **Arquitectura de una Sola Página (SPA)**: La aplicación se basa en una única página que, una vez cargada, no necesita navegar a otra página web. Es capaz de satisfacer los requisitos de los usuarios dentro de la propia aplicación. Algunos ejemplos son *Aman*, *The Berkeley*, *Bare Flyt*, entre muchos otros.
* **Arquitectura de Aplicaciones Web Progresivas (PWA)**: Están basadas en las SPA pero con capacidades offline, pudiéndose instalar en los dispositivos de los usuarios. Estas aplicaciones ofrecen compatibilidad entre plataformas. Podemos encontrar este tipo de arquitectura en *BMW*, *Starbucks*, *Flipboard*, etc.
* **Arquitectura de Renderizado del Lado del Servidor (SSR)**: Las páginas web se renderizan en un servidor tras ser solicitadas por el usuario, reduciendo de esta forma la carga en el dispositivo del cliente. Este tipo de aplicaciones son muy usuales en *blogs* y en *comercio electrónico*.
* **Arquitectura Orientada al Servicio(SOA)**: Las aplicaciones se dividen en servicios y cada servicio representa una unidad funcional que se encuentra débilmente acoplada al resto. Los servicios interactúan a través de mensajes. Según una entrada en el blog RevistaCloud:

  > *Se destaca por permitir la integración de los elementos del software implementados y que se mantienen por separado. De ese modo, estos se comunican entre sí y logran trabajar de manera conjunta para generar, en los distintos sistemas, aplicaciones de software.*
  >

  Algunos ejemplos que utilizan este tipo de arquitectura son *Cisco* y *Delaware Electric*.
* **Arquitectura de Microservicios**: Los microservicios son componentes modulares que encajan entre sí, permitiendo construir una página web, manteniendo cada componente pequeño y con contexto limitado (cada servicio tiene su código y mantiene las mínimas dependencias con otros microservicios). Ejemplos de uso de esta arquitectura son *Netflix, Amazon* y *Ebay*.

## Mecanismos de Ejecución de Código en un Navegador Web. Capacidades y Limitaciones de Ejecución. Compatibilidad con Navegadores Web

El motor de Javascript ejecuta el código de forma secuencial en cuanto se carga el navegador. Cada línea se convierte a binario y luego se ejecuta en el navegador. Cada navegador tiene su propio motor, lo que permite que se ejecute el código. Como podemos leer en Atatus en How Javascript works - Behind the Scenes, "*the Chrome V8 engine is one of the most well-known JavaScript engines*". Sin embargo, no es el único navegador que tiene motor de javascript. A continuación, algunos navegadores con sus correspondientes motores:

* Google Chrome: V8
* Safari: JavaScriptCore
* Mozilla Firefox: Spider Monkey
* Microsoft Edge: Chakra

Algunas diferencias que podemos encontrar en los navegadores es el ECMA que, como dice Open Webinars:

> *ECMAScript específicamente es el **estándar** que a partir del año 2015 a la actualidad se encarga de  **regir como debe ser interpretado y funcionar el lenguaje JavaScript** , siendo este (JS – JavaScript) interpretado y procesado por multitud de plataformas, entre las que se encuentran los navegadores web, NodeJS u otros ambientes como el desarrollo de aplicaciones para los distintos sistemas operativos que actualmente existen en el mercado. Los responsables de dichos navegadores y JavaScript deben encargarse de interpretar el lenguaje tal como lo fija ECMAScript.*

Otras diferencias que podemos encontrar es el OS, quién lo usa y, cómo no, cada uno de ellos tiene sus propios puntos fuertes.

| NOMBRE         | ECMA    | OS                     | PUNTOS FUERTES                                                                                | QUIÉN LO USA                                   |
| -------------- | ------- | ---------------------- | --------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| V8             | es5     | windows/unix, .NET     | Mejora de rendimiento para cuellos de botella, eliminado de código basura, API propia, debug | NodeJS, Google Chrome, akshell                  |
| JavaScriptCore | es5     | windows/unix           | Incluye un recolector de basura, alta portabilidad                                            | Apple's Safari, Webkit Internal Engine          |
| Spider Monkey  | es5/es6 | windows/unix           | Extensiones propias, manipulación directa de XML (E4X)                                       | Mozilla/NetScape, Adobe, CouchDB, MongoDB, etc |
| Chakra         | es5     | windows 7, x86/x64/arm | Eliminado de código basura                                                                   | Internet Explorer 9+                            |

Según wikipedia, traduciendo textualmente lo que dice:

> *La compatibilidad entre navegadores es la capacidad de un sitio web o una aplicación web para funcionar en diferentes navegadores y degradarse correctamente cuando las funciones del navegador están ausentes o faltan.*

Es decir, es la capacidad de hacer que la web funcione correctamente en cualquier navegador. Para asegurarnos de que nuestra web funciona correctamente, hay que realizar pruebas exhaustivas en una variedad de navegadores y dispositivos, incluyendo también diferentes versiones de cada navegador.

## Lenguajes de Programación en Entorno Cliente

Los lenguajes de programación más comunes en Entorno Cliente son:

* **JavaScript**: Es el lenguaje principal para el desarrollo web en el lado cliente. Entre sus ventajas podemos destacar la velocidad, simplicidad, compatibilidad, etc. JavaScript nos permite realizar webs interactivar y manipular el DOM.
* **TypeScript**: Es un superconjunto de JavaScript que está pensado para grandes proyectos. TypeScript usa la misma sintaxis que JavaScript sólo que, en este caso, es un lenguaje de alto tipado. Fue el lenguaje predeterminado de Google para desarrollar Angular.
* **Python**: Se trata de un lenguaje multiparadigma de código abierto que aunque normalmente se utiliza en servidor, se puede utilizar en el lado cliente mediante WebAssembly. Se utiliza sobretodo para el manejado de datos e Inteligencia Artificial.

## Características de los Lenguajes de Script. Ventajas y Desventajas

**VENTAJAS**:

* Tienen una sintaxis simple, por lo que son fáciles de aprender.
* Requieren menos memoria al no crear un archivo compilable.
* Se integran fácilmente con otras tecnologías y aplicaciones, lo que los hace ideales para la automatización y la interoperabilidad.
* Se pueden transferir de un OS a otro sin mucha dificultad.
* Suelen tener una amplia disponibilidad de bibliotecas.
* Permiten crear webs interactivas.

**DESVENTAJAS**:

* El intérprete es más lento que el compilador al ir línea a línea en tiempo de ejecución.
* Para proyectos de software muy grandes y complejos, los lenguajes de script no suelen ser la mejor elección.
* Para ejecutar scripts, se requiere un intérprete o una máquina virtual específica para el lenguaje.

## Tecnologías y Lenguajes Asociados. Integración del Código con las Etiquetas HTML.

Según Wikipedia,

> ***HTML** , siglas en inglés de **HyperText Markup Language** (‘lenguaje de marcado de hipertexto’), hace referencia al lenguaje de marcado para la elaboración de páginas web.*

> ***CSS** (siglas en inglés de **C**ascading **S**tyle **S**heets), en español «Hojas de estilo en cascada», es un lenguaje de diseño gráfico para definir y crear la presentación de un documento estructurado escrito en un lenguaje de marcado.*

En la creación de una página web es habitual utilizar la combinación de HTML y CSS. Con el HTML podemos crear la estructura base de la página web, mientras con el CSS podemos dar forma y personalizar la misma. De igual forma, podemos añadir JavaScript para hacer dinámica e interactiva nuestra web.

Nuestro código JavaScript podemos integrarlo de varias formas. Una de ellas es inyectándolo directamente en nuestro archivo .html como podemos ver en el siguiente ejemplo:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>
        document.write("¡Hola, mundo!")
    </script>
</body>
</html>
```

Y también podemos añadirlo al final de nuestro código.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
</body>
<script src="js/myscript.js"></script>
</html>
```

## Herramientas de Programación

* **VISUAL STUDIO CODE (VSCode)**: Es un editor de código fuente desarrollado por Microsoft. Es multiplataforma, software libre y puede utilizarse en diferentes sistemas operativos tales como Windows, Linux y MacOS. Algunas de sus catacterísticas son:
  * *IntelliSense*: Permite agilizar la escritura del código gracias a sugerencias de código y terminaciones inteligente, con funciones como autocompletado, resaltado del código, etc.
  * *Depuración*: Esta función nos permite encontrar errores en el código. Además, VSCode también detecta pequeños errores de forma automática sin necesidad de debugear.
  * *Uso de control de versiones*: Tiene compatibilidad con GIT, pudiendo revisar archivos y diferencias de versiones, realizar commits desde el editor, etc.
* 

## Bibliografía

https://rockcontent.com/es/blog/arquitectura-web/#:~:text=La%20arquitectura%20web%20es%20la,medio%20para%20ejecutar%20su%20trabajo.

https://kinsta.com/es/blog/arquitectura-aplicaciones-web/

https://colorlib.com/wp/spa-websites/

https://www.simicart.com/blog/progressive-web-apps-examples/

https://revistacloud.com/ejemplos-de-arquitectura-soa/

https://openwebinars.net/blog/microservicios-que-son/

https://www.atatus.com/blog/how-does-javascript-works/#:~:text=The%20JavaScript%20engine%20runs%20each,then%20run%20on%20the%20browser.

https://openwebinars.net/blog/que-es-ecmascript/

https://www.etnassoft.com/2011/05/31/comparativa-entre-los-distintos-motores-ecmascript/

https://es.wikipedia.org/wiki/JavaScriptCore

https://en.wikipedia.org/wiki/Cross-browser_compatibility

https://www.freecodecamp.org/espanol/news/ventajas-y-desventajas-de-javascript/

https://openwebinars.net/blog/que-es-php/

https://www.codesdope.com/blog/article/scripting-language/

https://es.wikipedia.org/wiki/HTML

https://es.wikipedia.org/wiki/CSS

https://openwebinars.net/blog/que-es-visual-studio-code-y-que-ventajas-ofrece/
