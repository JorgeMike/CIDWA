# Módulo 1: Introducción a CSS

## ¿Qué es CSS?

CSS (Cascading Style Sheets) es un lenguaje utilizado para describir la presentación de un documento HTML. Permite controlar el diseño y el estilo visual de las páginas web, como colores, tipografías, márgenes, y más.

---

## Beneficios de Usar CSS

-   Separación de contenido (HTML) y diseño (CSS).
-   Reutilización de estilos en múltiples páginas.
-   Mejora la accesibilidad y el mantenimiento del código.
-   Facilita la creación de diseños responsivos.

---

## Formas de Aplicar CSS

### CSS Inline

El estilo se aplica directamente en los elementos HTML utilizando el atributo `style`.

```html
<p style="color: red; font-size: 20px;">
    Este texto es rojo y tiene un tamaño de 20px.
</p>
```

### CSS Interno

El estilo se incluye en el archivo HTML dentro de la etiqueta `<style>`.

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            p {
                color: blue;
                font-size: 18px;
            }
        </style>
    </head>
    <body>
        <p>Este texto es azul y tiene un tamaño de 18px.</p>
    </body>
</html>
```

### CSS Externo

El estilo se coloca en un archivo separado con la extensión `.css` y se enlaza al archivo HTML con la etiqueta `<link>`.

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="styles.css" />
    </head>
    <body>
        <p>Este texto tiene estilo desde un archivo externo.</p>
    </body>
</html>
```

Archivo `styles.css`:

```css
p {
    color: green;
    font-size: 16px;
}
```

---

## Selectores Básicos

Los selectores se utilizan para apuntar a elementos específicos en el HTML.

### Selección por Etiqueta

Selecciona todos los elementos de una etiqueta específica.

```css
p {
    color: purple;
}
```

### Selección por Clase

Se utiliza un punto (`.`) antes del nombre de la clase.

```html
<p class="resaltado">Texto con clase "resaltado".</p>
```

```css
.resaltado {
    color: orange;
    font-weight: bold;
}
```

### Selección por ID

Se utiliza un símbolo de almohadilla (`#`) antes del nombre del ID.

```html
<p id="especial">Texto con ID "especial".</p>
```

```css
#especial {
    color: red;
    text-decoration: underline;
}
```

---

## Sintaxis Básica de CSS

Un bloque CSS consiste en un selector y un conjunto de reglas.

```css
selector {
    propiedad: valor;
}
```

Ejemplo:

```css
h1 {
    color: blue;
    font-size: 24px;
}
```

---

## Ejercicios Prácticos

### 1. Estilo Inline

Crea un párrafo en HTML y aplica estilo inline para que el texto sea de color rojo y tamaño 18px.

### 2. Estilo Interno

Crea un archivo HTML con un estilo interno que aplique los siguientes estilos:

-   Los encabezados `<h1>` deben ser de color azul.
-   Los párrafos `<p>` deben ser de color verde y tener un tamaño de 16px.

### 3. Estilo Externo

Crea un archivo CSS externo que aplique estos estilos:

-   Los enlaces (`<a>`) deben ser de color naranja.
-   Las listas (`<ul>` y `<ol>`) deben tener un margen izquierdo de 20px.

Archivo HTML:

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="styles.css" />
    </head>
    <body>
        <h1>Hola, CSS Externo</h1>
        <p>¡Estiliza este texto desde un archivo externo!</p>
    </body>
</html>
```

Archivo CSS (`styles.css`):

```css
h1 {
    color: blue;
    text-align: center;
}

p {
    color: gray;
    font-style: italic;
}
```
