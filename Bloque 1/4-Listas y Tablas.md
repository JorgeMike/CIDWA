# Módulo 4: Listas y Tablas en HTML

## Listas

### Tipos de Listas

1. **Listas no ordenadas**: Usan el elemento `<ul>` y cada ítem dentro de la lista se representa con `<li>`.
2. **Listas ordenadas**: Usan el elemento `<ol>` y también utilizan `<li>` para cada ítem.
3. **Listas de descripción**: Usan el elemento `<dl>` para contener pares de `<dt>` (término) y `<dd>` (descripción).

### Ejemplo de Listas

#### Lista no ordenada:

```html
<ul>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
    <li>Elemento 3</li>
</ul>
```

#### Lista ordenada:

```html
<ol>
    <li>Primer elemento</li>
    <li>Segundo elemento</li>
    <li>Tercer elemento</li>
</ol>
```

#### Lista de descripción:

```html
<dl>
    <dt>HTML</dt>
    <dd>Lenguaje de marcado para la web.</dd>

    <dt>CSS</dt>
    <dd>Lenguaje de estilos para diseñar páginas web.</dd>
</dl>
```

---

## Tablas

### Estructura básica de una tabla

1. **Encabezado de la tabla**: Se define con `<thead>` y contiene filas `<tr>` con encabezados `<th>`.
2. **Cuerpo de la tabla**: Se define con `<tbody>` y contiene filas `<tr>` con datos `<td>`.
3. **Pie de tabla**: Se define con `<tfoot>` para mostrar información adicional o un resumen.

### Ejemplo básico de tabla:

```html
<table border="1">
    <thead>
        <tr>
            <th>Nombre</th>
            <th>Edad</th>
            <th>País</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ana</td>
            <td>25</td>
            <td>México</td>
        </tr>
        <tr>
            <td>Juan</td>
            <td>30</td>
            <td>España</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="3">Total: 2 registros</td>
        </tr>
    </tfoot>
</table>
```

### Atributos comunes en tablas

-   `border`: Controla el borde de la tabla.
-   `cellpadding`: Añade espacio dentro de las celdas.
-   `cellspacing`: Añade espacio entre las celdas.
-   `colspan`: Permite que una celda ocupe varias columnas.
-   `rowspan`: Permite que una celda ocupe varias filas.

#### Ejemplo con `colspan` y `rowspan`:

```html
<table border="1">
    <tr>
        <th colspan="2">Encabezado</th>
    </tr>
    <tr>
        <td rowspan="2">Celda 1</td>
        <td>Celda 2</td>
    </tr>
    <tr>
        <td>Celda 3</td>
    </tr>
</table>
```

---

## Actividades

1. Crea una página que contenga:

    - Una lista ordenada con los días de la semana.
    - Una lista no ordenada con tus comidas favoritas.
    - Una tabla con tres columnas (Nombre, Edad, País) y al menos 4 filas de datos.

2. Experimenta con los atributos `border`, `colspan` y `rowspan` en una tabla.

3. Combina listas dentro de una celda de tabla para estructurar mejor la información.

---

## Conclusión

Las listas y tablas son herramientas clave para organizar contenido en la web. Dominar estas estructuras te permitirá crear páginas más organizadas y fáciles de leer.
