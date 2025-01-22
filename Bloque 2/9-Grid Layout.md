# Módulo 7: Grid Layout

## Introducción a Grid Layout

CSS Grid Layout es un sistema de diseño bidimensional que permite la creación de diseños web más complejos y flexibles. Proporciona un control preciso sobre filas y columnas, y es ideal para construir estructuras de diseño avanzadas en páginas web.

---

## Objetivos del Módulo

1. Comprender la estructura básica de Grid Layout.
2. Aprender a definir contenedores y elementos grid.
3. Explorar propiedades para filas, columnas, alineación y distribución.
4. Construir diseños responsivos utilizando Grid Layout.

---

## Contenido del Módulo

### 1. Configuración Inicial

#### HTML Base

```html
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Grid Layout</title>
        <link rel="stylesheet" href="styles.css" />
    </head>
    <body>
        <div class="grid-container">
            <div class="item">1</div>
            <div class="item">2</div>
            <div class="item">3</div>
            <div class="item">4</div>
            <div class="item">5</div>
            <div class="item">6</div>
        </div>
    </body>
</html>
```

#### CSS Base

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f3f3f3;
}

.grid-container {
    display: grid;
    gap: 10px;
    background-color: #ffffff;
    padding: 20px;
}

.item {
    background-color: #007bff;
    color: white;
    padding: 20px;
    text-align: center;
    border-radius: 5px;
}
```

---

### 2. Definiendo Filas y Columnas

-   Usando `grid-template-columns` y `grid-template-rows`:

```css
.grid-container {
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: auto;
}
```

-   Propiedades importantes:
    -   `repeat()`: Repite valores según la cantidad especificada.
    -   `1fr`: Una fracción del espacio disponible.

---

### 3. Espaciado y Alineación

-   `gap`: Define el espacio entre filas y columnas.
-   `justify-items` y `align-items`:

```css
.grid-container {
    justify-items: center;
    align-items: center;
}
```

---

### 4. Controlando el Posicionamiento

-   Usando `grid-column` y `grid-row` en los elementos:

```css
.item:nth-child(1) {
    grid-column: span 2;
}

.item:nth-child(2) {
    grid-row: span 2;
}
```

---

### 5. Diseño Responsivo con Grid

#### Usando Media Queries

```css
@media (max-width: 768px) {
    .grid-container {
        grid-template-columns: 1fr;
    }
}
```

---

### Ejercicio Práctico

Crea un diseño de tablero de ajedrez utilizando Grid Layout. Usa los siguientes estilos:

```css
.grid-container {
    grid-template-columns: repeat(8, 50px);
    grid-template-rows: repeat(8, 50px);
}

.item {
    background-color: #ffffff;
}

.item:nth-child(odd) {
    background-color: #000000;
}
```

---

### Proyecto Final

Construye una galería de imágenes responsiva utilizando Grid Layout. Los requisitos son:

-   La galería debe adaptarse al tamaño de la pantalla.
-   Incluir al menos 3 filas y 3 columnas en pantallas grandes.
-   Usar `gap` para el espaciado entre imágenes.

---

## Recursos Adicionales

-   [Guía de CSS Grid de MDN](https://developer.mozilla.org/es/docs/Web/CSS/CSS_Grid_Layout)
-   [CSS Tricks: A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

---

## Conclusión

CSS Grid Layout es una herramienta poderosa para diseñar interfaces web modernas y flexibles. A través de este módulo, los alumnos aprenderán a aprovechar su potencial para crear diseños dinámicos y responsivos.
