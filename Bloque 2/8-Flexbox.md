# Módulo 6: Flexbox

## Introducción a Flexbox

Flexbox, o "Flexible Box Layout", es un modelo de diseño en CSS que permite alinear y distribuir elementos dentro de un contenedor, incluso cuando sus tamaños son dinámicos o desconocidos. Es especialmente útil para crear layouts responsivos y flexibles.

## Objetivos del Módulo

-   Comprender el concepto de Flexbox.
-   Identificar los principales términos y propiedades asociadas.
-   Aplicar Flexbox para alinear y distribuir elementos en diferentes escenarios.

## Conceptos Clave

### Ejes de Flexbox

-   **Eje principal (main axis):** El eje en el que se distribuyen los ítems. Por defecto, es horizontal.
-   **Eje transversal (cross axis):** Perpendicular al eje principal. Por defecto, es vertical.

### Terminología

-   **Contenedor flex (flex container):** Elemento que tiene la propiedad `display: flex;` o `display: inline-flex;`.
-   **Ítems flex (flex items):** Elementos hijos directos del contenedor flex.

---

## Propiedades del Contenedor Flex

### `display`

```css
.container {
    display: flex; /* o inline-flex */
}
```

Activa el modelo Flexbox en el contenedor.

### `flex-direction`

Define la dirección del eje principal.

-   Valores: `row` (por defecto), `row-reverse`, `column`, `column-reverse`.

```css
.container {
    flex-direction: row;
}
```

### `justify-content`

Controla la distribución de los ítems a lo largo del eje principal.

-   Valores: `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`.

```css
.container {
    justify-content: center;
}
```

### `align-items`

Alinea los ítems a lo largo del eje transversal.

-   Valores: `stretch` (por defecto), `flex-start`, `flex-end`, `center`, `baseline`.

```css
.container {
    align-items: center;
}
```

### `align-content`

Alinea múltiples líneas (si existen) en el eje transversal.

-   Valores: `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `stretch`.

```css
.container {
    align-content: space-between;
}
```

### `flex-wrap`

Controla si los ítems deben ajustarse o permanecer en una sola línea.

-   Valores: `nowrap` (por defecto), `wrap`, `wrap-reverse`.

```css
.container {
    flex-wrap: wrap;
}
```

---

## Propiedades de los Ítems Flex

### `flex`

Define cómo un ítem puede crecer, encogerse y su tamaño base.

```css
.item {
    flex: 1; /* flex-grow flex-shrink flex-basis */
}
```

### `order`

Cambia el orden de los ítems (por defecto, todos tienen un valor de `0`).

```css
.item {
    order: 1;
}
```

### `align-self`

Sobrescribe la alineación definida por `align-items` para un ítem específico.

-   Valores: `auto`, `flex-start`, `flex-end`, `center`, `baseline`, `stretch`.

```css
.item {
    align-self: center;
}
```

---

## Ejemplos Prácticos

### Distribución Básica

```html
<div class="container">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
</div>
```

```css
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
    background-color: #f0f0f0;
}

.item {
    background-color: #4caf50;
    color: white;
    padding: 10px;
}
```

### Flexbox en Layouts Responsivos

```html
<div class="container">
    <div class="item">Header</div>
    <div class="item">Sidebar</div>
    <div class="item">Main Content</div>
</div>
```

```css
.container {
    display: flex;
    flex-wrap: wrap;
}

.item {
    flex: 1 1 200px;
    margin: 5px;
    padding: 20px;
    background-color: #2196f3;
    color: white;
}
```

---
