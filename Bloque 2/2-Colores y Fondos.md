# Módulo 2: Colores y Fondos

En este módulo aprenderemos cómo trabajar con colores y fondos en CSS, elementos esenciales para darle vida y personalidad a nuestras páginas web.

## Objetivos del módulo

- Entender los diferentes formatos para definir colores en CSS.
- Aplicar colores a texto y elementos.
- Configurar fondos con colores sólidos, degradados e imágenes.
- Conocer las propiedades avanzadas para controlar fondos.

---

## 1. **Colores en CSS**

### 1.1. Formatos de colores

CSS permite definir colores en diferentes formatos:

- **Nombres de colores**: `red`, `blue`, `green`, etc.
- **Hexadecimal**: `#RRGGBB` o `#RGB`.
  ```css
  color: #ff5733;
  ```
- **RGB y RGBA**:
  ```css
  color: rgb(255, 87, 51);
  color: rgba(255, 87, 51, 0.5); /* Con transparencia */
  ```
- **HSL y HSLA**:
  ```css
  color: hsl(14, 100%, 60%);
  color: hsla(14, 100%, 60%, 0.5);
  ```

### 1.2. Propiedades para aplicar colores

- **`color`**: Define el color del texto.
  ```css
  p {
      color: #3498db;
  }
  ```
- **`background-color`**: Define el color de fondo de un elemento.
  ```css
  div {
      background-color: #2ecc71;
  }
  ```

---

## 2. **Fondos en CSS**

### 2.1. Colores de fondo

- Usar la propiedad `background-color`:
  ```css
  body {
      background-color: #f0f0f0;
  }
  ```

### 2.2. Imágenes de fondo

- Usar la propiedad `background-image`:
  ```css
  div {
      background-image: url('ruta-a-la-imagen.jpg');
  }
  ```

### 2.3. Posicionamiento y tamaño del fondo

- **`background-position`**: Controla la posición de la imagen de fondo respecto al contenedor.
  ```css
  div {
      background-position: center center;
  }
  ```

- **`background-size`**: Ajusta el tamaño de la imagen de fondo en relación con el contenedor.
  ```css
  div {
      background-size: cover;
      /* Valores posibles: auto, cover, contain */
  }
  ```

### 2.4. Repetición del fondo

- **`background-repeat`**: Define si la imagen de fondo se repite.
  ```css
  div {
      background-repeat: no-repeat;
      /* Valores posibles: repeat, repeat-x, repeat-y, no-repeat */
  }
  ```

### 2.5. Fondos múltiples

- CSS permite definir múltiples fondos separados por comas.
  ```css
  div {
      background-image: url('imagen1.jpg'), url('imagen2.png');
      background-position: top left, bottom right;
      background-repeat: no-repeat;
  }
  ```

---

## 3. **Degradados en CSS**

CSS soporta degradados como fondos mediante la función `linear-gradient` o `radial-gradient`.

- **Degradado lineal**:
  ```css
  div {
      background: linear-gradient(to right, #ff7e5f, #feb47b);
  }
  ```

- **Degradado radial**:
  ```css
  div {
      background: radial-gradient(circle, #ff7e5f, #feb47b);
  }
  ```

---

## 4. **Propiedades abreviadas para fondos**

- La propiedad `background` permite resumir varias propiedades en una sola línea:
  ```css
  div {
      background: #2ecc71 url('fondo.jpg') no-repeat center/cover;
  }
  ```

---

## Ejercicios prácticos

1. Crea una página con un fondo degradado lineal que vaya de azul a verde.
2. Aplica una imagen de fondo que no se repita y se ajuste al tamaño del contenedor.
3. Diseña un bloque con texto en color blanco sobre un fondo negro con un degradado radial.

---

## Proyecto final del módulo

- Diseña una tarjeta de presentación donde utilices:
  - Colores aplicados a texto y fondo.
  - Una imagen de fondo.
  - Un degradado como fondo de un encabezado.

---

¡Con esto concluye el Módulo 2! Ahora estás listo para darle estilo y personalidad a tus páginas web con colores y fondos.
