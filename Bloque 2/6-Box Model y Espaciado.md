# Módulo 4: Box Model y Espaciado

En este módulo aprenderás los conceptos fundamentales del **Box Model** en CSS y cómo manipular el espaciado de los elementos para crear diseños más organizados y visualmente atractivos.

## 1. ¿Qué es el Box Model?

El Box Model es el modelo que describe cómo se renderizan los elementos en CSS. Cada elemento HTML es considerado como una caja que tiene las siguientes partes:

-   **Content**: El contenido del elemento.
-   **Padding**: Espacio entre el contenido y el borde.
-   **Border**: El borde que rodea el padding (o contenido si no hay padding).
-   **Margin**: Espacio entre el borde del elemento y otros elementos.

```css
/* Ejemplo básico del Box Model */
.box {
    width: 200px;
    height: 100px;
    padding: 10px;
    border: 5px solid black;
    margin: 15px;
    background-color: lightblue;
}
```

### Visualización del Box Model

Puedes usar herramientas del navegador para inspeccionar y visualizar el Box Model de un elemento.

---

## 2. Propiedades del Box Model

### 2.1 Propiedad `width` y `height`

Definen el tamaño del contenido de la caja.

```css
.box {
    width: 300px;
    height: 150px;
}
```

### 2.2 Propiedad `padding`

Define el espacio interior entre el contenido y el borde. Puede ser especificado de forma individual o general.

```css
/* Padding general */
.box {
    padding: 20px;
}

/* Padding individual */
.box {
    padding-top: 10px;
    padding-right: 15px;
    padding-bottom: 10px;
    padding-left: 15px;
}
```

### 2.3 Propiedad `border`

Define el grosor, estilo y color del borde.

```css
.box {
    border: 2px solid red; /* grosor, estilo, color */
}
```

### 2.4 Propiedad `margin`

Define el espacio exterior entre el borde del elemento y otros elementos.

```css
/* Margen general */
.box {
    margin: 20px;
}

/* Margen individual */
.box {
    margin-top: 10px;
    margin-right: 15px;
    margin-bottom: 10px;
    margin-left: 15px;
}
```

---

## 3. Propiedad `box-sizing`

Controla cómo se calcula el tamaño total de una caja.

-   **`content-box`** (valor por defecto): Solo considera el contenido al calcular el tamaño del elemento.
-   **`border-box`**: Incluye `padding` y `border` dentro del tamaño total.

```css
.box {
    width: 300px;
    height: 150px;
    padding: 20px;
    border: 10px solid black;
    box-sizing: border-box;
}
```

---

## 4. Prácticas

### Ejercicio 1: Ajustar una caja

```html
<div class="box">Contenido</div>
```

```css
.box {
    width: 200px;
    height: 100px;
    padding: 20px;
    border: 5px solid blue;
    margin: 10px;
    background-color: lightgreen;
}
```

### Ejercicio 2: Comparar `content-box` y `border-box`

```html
<div class="content-box">Content Box</div>
<div class="border-box">Border Box</div>
```

```css
.content-box {
    width: 200px;
    height: 100px;
    padding: 20px;
    border: 5px solid red;
    box-sizing: content-box;
    background-color: lightcoral;
}

.border-box {
    width: 200px;
    height: 100px;
    padding: 20px;
    border: 5px solid green;
    box-sizing: border-box;
    background-color: lightblue;
}
```

---

## 5. Buenas prácticas

-   Usa `box-sizing: border-box;` para simplificar el cálculo de tamaños.
-   Combina márgenes y padding sabiamente para evitar diseños desordenados.
-   Inspecciona los elementos con las herramientas del navegador para verificar cómo se aplican estas propiedades.

---
