# Módulo 5: Layout y Posicionamiento

En este módulo aprenderemos a manejar técnicas de diseño de layout y posicionamiento en CSS. Esto incluye cómo estructurar y alinear elementos en una página web.

## Objetivos del módulo

-   Comprender los diferentes tipos de posicionamiento en CSS.
-   Aprender a usar propiedades de layout como `display` y `position`.
-   Utilizar técnicas modernas para construir layouts responsivos y bien estructurados.

---

## 1. Propiedades de `display`

### Tipos comunes de `display`:

1. **`block`**: Ocupa todo el ancho disponible.
2. **`inline`**: Ocupa sólo el espacio necesario.
3. **`inline-block`**: Similar a `inline` pero permite definir ancho y alto.
4. **`none`**: Elimina el elemento del flujo de la página.

**Ejemplo:**

```html
<div style="display: block;">Elemento block</div>
<div style="display: inline;">Elemento inline</div>
```

---

## 2. Posicionamiento en CSS

### Tipos de posicionamiento:

1. **`static`**: Valor por defecto. Los elementos se posicionan en el flujo normal.
2. **`relative`**: Permite desplazar un elemento relativo a su posición normal.
3. **`absolute`**: Posiciona el elemento relativo al contenedor posicionado más cercano.
4. **`fixed`**: El elemento permanece fijo respecto a la ventana del navegador.
5. **`sticky`**: Combina características de `relative` y `fixed`.

**Ejemplo:**

```html
<div style="position: relative; top: 10px; left: 10px;">
    Posicionamiento relativo
</div>
<div style="position: absolute; top: 50px; left: 50px;">
    Posicionamiento absoluto
</div>
```

---

## 3. Uso de `float` y `clear`

### Propiedad `float`:

-   Se utiliza para alinear elementos a la izquierda o derecha.

**Ejemplo:**

```html
<div style="float: left; width: 50%;">Izquierda</div>
<div style="float: right; width: 50%;">Derecha</div>
```

### Propiedad `clear`:

-   Controla el flujo de elementos flotantes.

**Ejemplo:**

```html
<div style="clear: both;">Contenido después de flotantes</div>
```

---

## 4. Técnicas modernas de layout

### Propiedad `display: flex;`

-   Simplifica el diseño de elementos en un contenedor.

**Ejemplo:**

```html
<div
    style="display: flex; justify-content: space-between; align-items: center;"
>
    <div>Elemento 1</div>
    <div>Elemento 2</div>
    <div>Elemento 3</div>
</div>
```

### Propiedad `display: grid;`

-   Crea layouts complejos fácilmente.

**Ejemplo:**

```html
<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 10px;">
    <div>Columna 1</div>
    <div>Columna 2</div>
</div>
```

---

## 5. Ejercicio práctico

Crea un layout simple usando flexbox y grid para alinear elementos en una página.

**Reto:**

1. Diseña un encabezado, contenido principal y pie de página.
2. Usa `flexbox` para centrar el contenido.
3. Aplica `grid` para organizar el contenido principal en 3 columnas.

**Código de referencia:**

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <style>
            body {
                margin: 0;
                font-family: Arial, sans-serif;
            }

            header,
            footer {
                background: #333;
                color: white;
                text-align: center;
                padding: 10px;
            }

            main {
                display: grid;
                grid-template-columns: 1fr 2fr 1fr;
                gap: 15px;
                padding: 20px;
            }

            .flex-container {
                display: flex;
                justify-content: space-around;
                align-items: center;
                height: 100px;
                background: #f4f4f4;
            }
        </style>
    </head>
    <body>
        <header>Encabezado</header>

        <div class="flex-container">
            <div>Elemento A</div>
            <div>Elemento B</div>
            <div>Elemento C</div>
        </div>

        <main>
            <div>Columna 1</div>
            <div>Columna 2</div>
            <div>Columna 3</div>
        </main>

        <footer>Pie de página</footer>
    </body>
</html>
```

---

## Conclusión

El layout y posicionamiento en CSS son fundamentales para crear sitios web organizados y atractivos. Practica combinando técnicas como `flexbox`, `grid` y `position` para lograr diseños modernos y responsivos.
