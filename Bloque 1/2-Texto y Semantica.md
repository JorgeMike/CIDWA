# Módulo 2: Texto y Semántica

## Etiquetas de Texto

### Encabezados: `<h1>` a `<h6>`

-   Utilizados para jerarquizar títulos.
-   `<h1>` es el más importante y `<h6>` el menos importante.

```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
<h3>Sección</h3>
```

### Párrafos: `<p>`

-   Para agregar bloques de texto.

```html
<p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis
    excepturi quaerat saepe dolorum vero et quas aliquid quia soluta? Iste
    repellendus laboriosam sed necessitatibus ipsam voluptatum deserunt autem
    molestiae minus.
</p>
```

### Énfasis en Texto

-   `<strong>`: Da importancia al texto (negritas, semánticamente fuerte).
-   `<em>`: Agrega énfasis (cursivas, semánticamente relevante).

```html
<p>
    Este es un <strong>texto importante</strong> y este un
    <em>texto destacado</em>.
</p>
```

### Texto en Línea

-   `<span>`: Agrupa texto en línea para aplicar estilos específicos.

```html
<p>Este texto tiene una <span style="color: red;">palabra roja</span>.</p>
```

---

## Introducción a la Semántica Web

### ¿Qué es la Semántica Web?

La **semántica web** consiste en el uso de etiquetas HTML significativas que describen el propósito del contenido. Esto mejora:

-   **Accesibilidad**: Facilita la interpretación por herramientas como lectores de pantalla.
-   **SEO** (Optimización para Motores de Búsqueda): Mejora la indexación en buscadores.
-   **Legibilidad del código**: Ayuda a otros desarrolladores a comprender mejor la estructura del contenido.

### Ejemplo Comparativo

#### Sin Semántica:

```html
<div>Este es un título</div>
<div>Este es un párrafo</div>
```

#### Con Semántica:

```html
<h1>Este es un título</h1>
<p>Este es un párrafo</p>
```

---

## Agrupación y Secciones

### Agrupación Básica

-   **`<div>`**: Contenedor genérico para agrupar contenido. Útil para estilos o scripts.

```html
<div>
    <h2>Subsección</h2>
    <p>Texto dentro de un contenedor.</p>
</div>
```

### Etiquetas Semánticas Modernas

-   **`<section>`**: Agrupa contenido relacionado (secciones generales).
-   **`<article>`**: Contenido independiente como artículos o publicaciones.
-   **`<header>`**: Encabezado de una página o sección.
-   **`<footer>`**: Pie de página o información complementaria.
-   **`<aside>`**: Información secundaria o contextual.

```html
<section>
    <header>
        <h2>Título de la Sección</h2>
    </header>
    <article>
        <p>Contenido del artículo.</p>
    </article>
    <footer>
        <p>Fin de la sección.</p>
    </footer>
</section>
```

---

## Comentarios en HTML

-   Los comentarios no son visibles en la página web y se utilizan para anotar el código.

```html
<!-- Este es un comentario -->
```

---

## Práctica Sugerida

1. Crear una página con la siguiente estructura:
    - Un título principal (`<h1>`).
    - Dos subsecciones (`<section>`), cada una con:
        - Un encabezado (`<h2>`).
        - Un párrafo descriptivo (`<p>`).
    - Un pie de página (`<footer>`).

### Ejemplo de Código

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Document</title>
    </head>
    <body>
        <header>
            <h1>Bienvenidos a mi página</h1>
        </header>
        <main>
            <section>
                <h2>Primera Sección</h2>
                <p>Este es el contenido de la primera sección.</p>
            </section>
            <section>
                <h2>Segunda Sección</h2>
                <p>Este es el contenido de la segunda sección.</p>
            </section>
        </main>
        <footer>
            <p>&copy; 2025 Mi Página Web</p>
        </footer>
    </body>
</html>
```
