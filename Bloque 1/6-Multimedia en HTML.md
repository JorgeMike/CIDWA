# Bloque 1: HTML

## Módulo 6: Multimedia en HTML

En este módulo, exploraremos cómo incluir y manejar contenido multimedia en nuestras páginas web utilizando etiquetas HTML. Aprenderemos a agregar imágenes, videos, y audio, así como a optimizar su rendimiento y accesibilidad.

---

### 1. **Introducción al contenido multimedia**

-   ¿Qué es el contenido multimedia?
-   Importancia del contenido multimedia en las páginas web.

---

### 2. **Insertar imágenes**

-   Etiqueta `<img>`
    -   Atributos principales:
        -   `src`: Fuente de la imagen.
        -   `alt`: Texto alternativo para accesibilidad.
        -   `width` y `height`: Dimensiones de la imagen.
-   Ejemplo básico:

```html
<img
    src="imagen-ejemplo.jpg"
    alt="Descripción de la imagen"
    width="300"
    height="200"
/>
```

-   Optimización de imágenes:
    -   Formatos recomendados: JPEG, PNG, WebP.
    -   Comprimir imágenes antes de usarlas.

---

### 3. **Agregar videos**

-   Etiqueta `<video>`

    -   Atributos principales:
        -   `src`: Fuente del video.
        -   `controls`: Muestra controles de reproducción.
        -   `autoplay`: Reproducción automática (usar con precaución).
        -   `loop`: Reproducción en bucle.
        -   `muted`: Silenciar el audio por defecto.

-   Ejemplo básico:

```html
<video src="video-ejemplo.mp4" controls width="640" height="360">
    Tu navegador no soporta la reproducción de videos.
</video>
```

-   Formatos comunes de video:
    -   MP4 (H.264)
    -   WebM
    -   Ogg

---

### 4. **Agregar audio**

-   Etiqueta `<audio>`

    -   Atributos principales:
        -   `src`: Fuente del audio.
        -   `controls`: Muestra controles de reproducción.
        -   `autoplay`, `loop`, `muted`.

-   Ejemplo básico:

```html
<audio src="audio-ejemplo.mp3" controls>
    Tu navegador no soporta la reproducción de audio.
</audio>
```

-   Formatos comunes de audio:
    -   MP3
    -   Ogg
    -   WAV

---

### 5. **Uso de multimedia desde fuentes externas**

-   Integración de videos de YouTube:

```html
<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/ID_DEL_VIDEO"
    frameborder="0"
    allowfullscreen
></iframe>
```

-   Consideraciones de rendimiento:
    -   Usar imágenes y videos optimizados.
    -   Cargar multimedia solo cuando sea necesario (lazy loading).

---

### 6. **Buenas prácticas para contenido multimedia**

-   Usar siempre texto alternativo (`alt`) para imágenes.
-   No abusar de videos o audios que se reproduzcan automáticamente.
-   Proveer transcripciones o subtítulos cuando sea posible.

---

### 7. **Desafío práctico**

Crea una página web que incluya:

1. Una imagen con texto alternativo.
2. Un video con controles de reproducción.
3. Un archivo de audio.
4. Un video incrustado desde YouTube.

---