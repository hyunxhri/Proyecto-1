---
marp: true
theme: uncover
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---
# **PRESENTACIÓN**

#### Sara Bulpe Martínez

---

### **Modelos de Arquitectura web**

- **Single Page Application (SPA)**
  - Una vez cargada no necesita navegar a otra web.
- **Arquitectura de Aplicaciones Web Progresivas (PWA)**
  - Basadas en las SPA pero con propiedades offline. Pueden instalarse en los dispositivos.
- **Arquitectura de Renderizado del Lado del Servidor (SSR)**
  - Las páginas web se renderizan en un servidor tras ser solicitadas por el usuario.

---

### **Modelos de Arquitectura web**

- **Arquitectura Orientada al Servicio(SOA)**
  - Las aplicaciones se dividen en servicios y cada servicio representa una unidad funcional.
- **Arquitectura de Microservicios**
  - Los microservicios son componentes modulares que encajan entre sí, manteniendo cada componente pequeño y con contexto limitado.

---

### **Mecanismos de Ejecución de Código en un Navegador Web**

- El motor de Javascript ejecuta el código de forma secuencial en cuanto se carga el navegador. Cada navegador tiene su propio motor.

  - **Google Chrome**: V8
  - **Safari**: JavaScriptCore
  - **Mozilla Firefox**: Spider Monkey
  - **Microsoft Edge**: Chakra

---

### **Mecanismos de Ejecución de Código en un Navegador Web**

* La compatibilidad entre navegadores es la capacidad de hacer que la web funcione correctamente en cualquier navegador.
  * Realizar pruebas exhaustivas en una variedad de navegadores y dispositivos, incluyendo también diferentes versiones de cada navegador.

---

## **Lenguajes de Programación en Entorno Cliente**

![Logo JavaScript](https://cdn.iconscout.com/icon/free/png-256/free-javascript-2038874-1720087.png) ㅤ![Logo TypeScript](https://cdn.iconscout.com/icon/free/png-256/free-typescript-1174965.png?f=webp)ㅤㅤ![Logo Python](https://cdn.iconscout.com/icon/free/png-256/free-python-3628999-3030224.png?f=webp) 

---

## **Lenguajes de Programación en Entorno Cliente**

- **JavaScript**: Lenguaje principal. Permite crear webs interactivas y manipular el DOM. 
- **TypeScript**: Misma sintaxis que JavaScript pero siendo un lenguaje de alto tipado.
- **Python**: Normalmente se utiliza en servidor, pero se puede utilizar en el lado cliente mediante WebAssembly.

---

### **Características de los Lenguajes de Script. Ventajas y Desventajas**

- **VENTAJAS**
  - Sintaxis simple.
  - Requieren menos memoria.
  - Se integran fácilmente con otras tecnologías y aplicaciones.
  - Se pueden transferir de un OS a otro sin mucha dificultad.
  - Amplia disponibilidad de bibliotecas.
  - Permiten crear webs interactivas.

---

### **Características de los Lenguajes de Script. Ventajas y Desventajas**

- **DESVENTAJAS**
  - El intérprete es más lento que el compilador.
  - No son buenos para proyectos de software muy grandes y complejos.
  - Se requiere un intérprete o una máquina virtual específica para el lenguaje.

---

### **Tecnologías y Lenguajes Asociados. Integración del Código con las Etiquetas HTML**

* Con el HTML podemos crear la estructura base de la página web, mientras con el CSS podemos dar forma y personalizar la misma. Usamos JavaScript para hacer dinámica e interactiva nuestra web.

* Podemos inyectarlo dentro de nuestro archivo html o añadirlo al final de nuestro código.

--- 

### **Integración del Código con las Etiquetas HTML**
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
<script src="js/myscript.js"></script>
</html>
```

---

## **Herramientas de Programación**

![Logo VSCode](https://code.visualstudio.com/assets/apple-touch-icon.png) ㅤ![Logo Chrome DevTools](https://static-00.iconduck.com/assets.00/chrome-devtools-icon-256x256-s41ravx1.png)ㅤ![width:250px](https://static-00.iconduck.com/assets.00/git-icon-512x512-61zfmvxk.png) 

---

## **Herramientas de Programación**

- **Visual Studio Code (VSCode)**: Es un editor de código fuente multiplataforma, de software libre y que puede utilizarse en diferentes SO.
- **Chrome DevTools**: Es una herramienta de desarrollo integrada en el navegador para diagnosticar errores o testear las modificaciones mínimas.
- **GIT**: Es un sistema de control de versiones distribuido, diseñado para la eficiencia, confiabilidad y compatibilidad de las diferentes versiones de una aplicación.