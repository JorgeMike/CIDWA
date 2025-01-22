# Módulo 3: Tipografía y Estilo de Texto

En este módulo aprenderás cómo utilizar las propiedades de CSS para aplicar estilos tipográficos a los textos de tu página web. Esto incluye cambiar fuentes, ajustar tamaños, colores, espaciados, y más.

---

## **Objetivos del módulo**

- Comprender la importancia de la tipografía en el diseño web.
- Aplicar propiedades básicas de texto utilizando CSS.
- Conocer cómo usar fuentes personalizadas.
- Controlar el espaciado y alineación del texto.

---

## **Conceptos clave**

### **1. Propiedades básicas de texto**

#### **Color del texto**
```css
/* Cambia el color del texto */
p {
  color: #333333; /* Color en formato hexadecimal */
}
```

#### **Fuente y tamaño de texto**
```css
/* Cambia la fuente y el tamaño del texto */
h1 {
  font-family: Arial, sans-serif; /* Lista de fuentes con fallback */
  font-size: 24px; /* Tamaño de fuente */
}
```

#### **Peso de la fuente**
```css
/* Cambia el grosor del texto */
p {
  font-weight: bold; /* Valores: normal, bold, bolder, lighter o números (100-900) */
}
```

#### **Estilo de la fuente**
```css
/* Aplica cursiva al texto */
blockquote {
  font-style: italic;
}
```

### **2. Fuentes personalizadas**

#### **Fuentes del sistema**
```css
/* Usa una lista de fuentes comunes del sistema */
body {
  font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
}
```

#### **Uso de Google Fonts**
1. Ve a [Google Fonts](https://fonts.google.com/).
2. Selecciona una fuente y copia el enlace proporcionado.
3. Inclúyelo en tu archivo HTML:

```html
<head>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
```

4. Aplica la fuente en CSS:
```css
body {
  font-family: 'Roboto', sans-serif;
}
```

### **3. Espaciado de texto**

#### **Interlineado (line-height)**
```css
/* Ajusta la altura de línea */
p {
  line-height: 1.5; /* Proporción o unidades como px */
}
```

#### **Espaciado entre letras (letter-spacing)**
```css
/* Añade espacio entre las letras */
h1 {
  letter-spacing: 2px;
}
```

#### **Espaciado entre palabras (word-spacing)**
```css
/* Añade espacio entre las palabras */
p {
  word-spacing: 4px;
}
```

### **4. Alineación del texto**

#### **Propiedad text-align**
```css
/* Alinea el texto */
header {
  text-align: center; /* Valores: left, right, center, justify */
}
```

#### **Transformaciones de texto**
```css
/* Cambia el formato del texto */
h2 {
  text-transform: uppercase; /* Valores: capitalize, lowercase, uppercase */
}
```

### **5. Decoración del texto**

#### **Propiedad text-decoration**
```css
/* Decora el texto */
a {
  text-decoration: none; /* Valores: none, underline, overline, line-through */
}
```

---

## **Práctica**

1. Crea un archivo HTML y enlázalo con un archivo CSS.
2. Aplica estilos a los textos utilizando:
   - Una fuente personalizada desde Google Fonts.
   - Diferentes tamaños, pesos y colores.
   - Espaciado y alineación del texto.
3. Experimenta con transformaciones y decoraciones para mejorar la estética del texto.

---

## **Ejercicio final**

Diseña una página web con un título, subtítulo y párrafos estilizados. Utiliza al menos:

- Una fuente de Google Fonts.
- Propiedades de alineación y espaciado.
- Decoraciones y transformaciones de texto.

---