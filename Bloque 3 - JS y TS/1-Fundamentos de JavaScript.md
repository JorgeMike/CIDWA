# Módulo 1: Fundamentos de JavaScript

## Objetivo del Módulo

Al finalizar este módulo, los alumnos serán capaces de comprender los fundamentos básicos de JavaScript, incluyendo su sintaxis, variables, operadores y estructuras básicas. Este módulo sienta las bases para el desarrollo de habilidades avanzadas en JavaScript.

---

## Introducción a JavaScript

### ¿Qué es JavaScript?

#### Definición y Propósito

JavaScript es un lenguaje de programación interpretado, dinámico y orientado a objetos, diseñado principalmente para crear interactividad en aplicaciones web. Se utiliza junto con HTML y CSS para construir interfaces web dinámicas y responsivas.

#### Historia y Evolución

- **1995**: Brendan Eich desarrolló JavaScript en 10 días, inicialmente llamado "Mocha" y luego "LiveScript", antes de ser renombrado como "JavaScript".
- **1997**: JavaScript se estandarizó como ECMAScript por ECMA International.
- **2009**: Se lanzó Node.js, permitiendo ejecutar JavaScript fuera del navegador.
- **Presente**: JavaScript es un estándar para el desarrollo web moderno, utilizado tanto en el frontend como en el backend.

#### Dónde y Cómo se Utiliza JavaScript

- **Navegadores web**: Añade interactividad, valida formularios, y mejora la experiencia del usuario.
- **Servidores**: Con Node.js, se usa para construir aplicaciones backend escalables y rápidas.
- **Aplicaciones móviles y de escritorio**: Frameworks como React Native y Electron permiten desarrollar aplicaciones multiplataforma.
- **Automatización**: Scripts para tareas repetitivas o pruebas.
- **Inteligencia Artificial**: Con bibliotecas como TensorFlow.js para machine learning.

---

## Configuración Inicial

### Primeros Pasos:

1. **Configura tu entorno de trabajo:**
   - Abre una terminal en tu sistema operativo.
   - Navega a la carpeta donde deseas trabajar usando comandos como `cd`. Por ejemplo:
     ```bash
     cd ~/CIDWA/[TuNumeroDeCuenta]
     ```
   - Abre la carpeta en Visual Studio Code con el siguiente comando:
     ```bash
     code .
     ```
2. **Crea tu primer archivo JavaScript:**
   - Dentro de Visual Studio Code, crea un archivo llamado `index.js`.
   - Agrega comentarios iniciales para documentar tu código:
     ```javascript
     // Archivo: index.js
     // Autor: [Tu Nombre]
     // Descripción: Introducción a los fundamentos de JavaScript
     ```

---

## Conceptos Básicos de JavaScript

### Comentarios en JavaScript

Los comentarios son fundamentales para hacer que el código sea más legible y comprensible. En JavaScript, hay dos tipos principales de comentarios:

1. **Comentarios de una sola línea:**

   ```javascript
   // Este es un comentario de una sola línea
   ```

2. **Comentarios de varias líneas:**
   ```javascript
   /*
   Este es un comentario
   que ocupa varias líneas
   */
   ```

---

### Sintaxis Básica

1. **Declaración de Variables:**
   JavaScript utiliza `var`, `let` y `const` para declarar variables. En este curso, se recomienda usar `let` y `const` debido a su comportamiento moderno.

   ```javascript
   let nombre = "Juan"; // Variable que puede cambiar
   const PI = 3.14159; // Variable constante
   ```

2. **Tipos de Datos:**
   JavaScript admite varios tipos de datos:

   - **Primitivos:** `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint`.
   - **Objetos:** Arrays, funciones, objetos personalizados, etc.

   Ejemplo:

   ```javascript
   let edad = 25; // number
   let nombre = "Ana"; // string
   let esEstudiante = true; // boolean
   let sinValor = null; // null
   let noDefinido; // undefined
   ```

3. **Operadores:**

   - **Aritméticos:** `+`, `-`, `*`, `/`, `%`
   - **Asignación:** `=`, `+=`, `-=`, `*=`
   - **Comparación:** `==`, `===`, `!=`, `!==`, `>`, `<`, `>=`, `<=`
   - **Lógicos:** `&&`, `||`, `!`

   Ejemplo:

   ```javascript
   let resultado = (10 + 5) * 2; // 30
   console.log(resultado);
   ```

4. **Funciones y Parámetros:**
   Las funciones son bloques de código reutilizables que realizan una tarea específica. Puedes definir una función con o sin parámetros.

   **Declaración de una función:**

   ```javascript
   function saludar(nombre) {
     console.log(`Hola, ${nombre}!`);
   }

   saludar("María"); // Llama a la función con el parámetro "María"
   ```

   **Funciones con valor de retorno:**

   ```javascript
   function sumar(a, b) {
     return a + b;
   }

   let resultado = sumar(3, 7);
   console.log(`El resultado de la suma es: ${resultado}`);
   ```

---

En la siguiente sesión, exploraremos **Control de Flujo y Bucles** en JavaScript, donde aprenderás a manejar decisiones y repetir acciones de manera eficiente.
