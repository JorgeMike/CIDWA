# Módulo 3: Enlaces e Imágenes

En este módulo aprenderemos a utilizar los enlaces y las imágenes en HTML para crear contenido interactivo y visualmente atractivo en nuestras páginas web.

## Conceptos Clave

### Enlaces
- Los enlaces permiten a los usuarios navegar entre páginas o sitios web.
- Se crean utilizando la etiqueta `<a>` (anchor).

#### Sintaxis Básica
```html
<a href="URL">Texto del enlace</a>
```
**Atributos importantes:**
- `href`: Especifica la URL del recurso al que apunta el enlace.
- `target`: Define cómo se abre el enlace (por ejemplo, en una nueva pestaña con `_blank`).
- `rel`: Proporciona información adicional sobre el enlace, como `nofollow` o `noopener`.

#### Opciones del atributo `rel`
- `nofollow`: Indica a los motores de búsqueda que no deben seguir el enlace.
- `noopener`: Previene que la nueva página tenga acceso al objeto `window` del origen, mejorando la seguridad.
- `noreferrer`: No envía información de referencia al destino.
- `author`: Especifica que el enlace apunta a la página de un autor.
- `license`: Indica que el enlace lleva a información sobre derechos de autor o licencias.
- `ugc`: Señala que el enlace es generado por usuarios (User Generated Content).

#### Ejemplo
```html
<a href="https://www.google.com" target="_blank" rel="noopener">Ir a Google</a>
```

### Imágenes
- Las imágenes enriquecen el contenido visual de nuestras páginas.
- Se agregan utilizando la etiqueta `<img>`.

#### Sintaxis Básica
```html
<img src="URL" alt="Descripción de la imagen">
```
**Atributos importantes:**
- `src`: Especifica la URL de la imagen.
- `alt`: Proporciona texto alternativo que describe la imagen (útil para accesibilidad y cuando la imagen no carga).
- `width` y `height`: Definen el tamaño de la imagen.

#### Ejemplo
```html
<img src="https://via.placeholder.com/150" alt="Imagen de ejemplo">
```

---

## Ejercicios Prácticos

### Ejercicio 1: Crear un Enlace
Crea un enlace que lleve al sitio de tu elección y que se abra en una nueva pestaña.

```html
<a href="https://www.example.com" target="_blank">Visita mi sitio favorito</a>
```

### Ejercicio 2: Insertar una Imagen
Agrega una imagen desde una URL pública y proporciona un texto alternativo.

```html
<img src="https://via.placeholder.com/300" alt="Imagen genérica">
```

### Ejercicio 3: Combinar Enlaces e Imágenes
Crea un enlace que contenga una imagen. Al hacer clic en la imagen, el usuario será dirigido a otro sitio web.

```html
<a href="https://www.example.com">
  <img src="https://via.placeholder.com/150" alt="Haz clic aquí">
</a>
```

---

## Desafío
Crea una página web que incluya:
1. Un enlace a tu perfil de GitHub o LinkedIn.
2. Una imagen de tu elección con un texto alternativo descriptivo.
3. Un enlace con una imagen como contenido interactivo.

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ejercicio de Enlaces e Imágenes</title>
</head>
<body>
  <h1>Mis Ejemplos de Enlaces e Imágenes</h1>

  <!-- Enlace simple -->
  <p><a href="https://github.com/tuusuario" target="_blank">Visita mi GitHub</a></p>

  <!-- Imagen simple -->
  <p><img src="https://via.placeholder.com/200" alt="Imagen de ejemplo"></p>

  <!-- Enlace con imagen -->
  <p>
    <a href="https://www.linkedin.com/in/tuusuario" target="_blank">
      <img src="https://via.placeholder.com/150" alt="Enlace a LinkedIn">
    </a>
  </p>
</body>
</html>
```
