# Módulo 5: Formularios Básicos en HTML

En este módulo, aprenderás los conceptos básicos para crear formularios en HTML. Los formularios son fundamentales para recolectar información de los usuarios en las aplicaciones web.

## Conceptos Clave

### 1. Etiqueta `<form>`

La etiqueta `<form>` se utiliza para definir un formulario.

```html
<form action="/submit" method="POST">
    <!-- Campos del formulario -->
</form>
```

-   **`action`**: Define la URL a la que se enviarán los datos del formulario.
-   **`method`**: Define el método HTTP para enviar los datos (`GET` o `POST`).

### 2. Campos de Entrada

Los campos de entrada se crean con la etiqueta `<input>`.

#### Tipos Comunes de Entrada:

```html
<input type="text" name="nombre" placeholder="Ingresa tu nombre" />
<input type="email" name="correo" placeholder="Ingresa tu correo electrónico" />
<input type="password" name="contraseña" placeholder="Ingresa tu contraseña" />
<input type="number" name="edad" placeholder="Ingresa tu edad" />
<input type="checkbox" name="acepto" value="sí" /> Acepto los términos y
condiciones <input type="radio" name="genero" value="masculino" /> Masculino
<input type="radio" name="genero" value="femenino" /> Femenino
```

-   **`type`**: Especifica el tipo de campo (texto, correo, contraseña, número, etc.).
-   **`name`**: Nombre del campo para identificarlo en el servidor.
-   **`placeholder`**: Texto que aparece como guía dentro del campo.

### 3. Etiqueta `<label>`

La etiqueta `<label>` mejora la accesibilidad al asociar etiquetas con los campos de entrada.

```html
<label for="nombre">Nombre:</label>
<input type="text" id="nombre" name="nombre" />
```

-   **`for`**: Relaciona la etiqueta con el campo mediante su atributo `id`.

### 4. Área de Texto

Para texto más extenso, se usa `<textarea>`.

```html
<textarea
    name="comentarios"
    rows="4"
    cols="50"
    placeholder="Escribe tus comentarios"
></textarea>
```

### 5. Selección de Opciones

Usa `<select>` para listas desplegables.

```html
<select name="pais">
    <option value="mx">México</option>
    <option value="us">Estados Unidos</option>
    <option value="ca">Canadá</option>
</select>
```

### 6. Botones de Envío

Los botones son esenciales para enviar los datos del formulario.

```html
<button type="submit">Enviar</button> <input type="reset" value="Limpiar" />
```

-   **`type="submit"`**: Envía el formulario.
-   **`type="reset"`**: Limpia los campos del formulario.

## Ejemplo Completo

```html
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Formulario Básico</title>
    </head>
    <body>
        <h1>Registro</h1>
        <form action="/registro" method="POST">
            <label for="nombre">Nombre:</label>
            <input
                type="text"
                id="nombre"
                name="nombre"
                placeholder="Ingresa tu nombre"
                required
            />

            <label for="correo">Correo:</label>
            <input
                type="email"
                id="correo"
                name="correo"
                placeholder="Ingresa tu correo electrónico"
                required
            />

            <label for="contraseña">Contraseña:</label>
            <input
                type="password"
                id="contraseña"
                name="contraseña"
                placeholder="Ingresa tu contraseña"
                required
            />

            <label for="pais">País:</label>
            <select id="pais" name="pais">
                <option value="mx">México</option>
                <option value="us">Estados Unidos</option>
                <option value="ca">Canadá</option>
            </select>

            <label for="comentarios">Comentarios:</label>
            <textarea
                id="comentarios"
                name="comentarios"
                rows="4"
                cols="50"
                placeholder="Escribe tus comentarios"
            ></textarea>

            <button type="submit">Enviar</button>
            <input type="reset" value="Limpiar" />
        </form>
    </body>
</html>
```

### Tareas Prácticas

1. Crea un formulario para registro de eventos que incluya nombre, correo, número de teléfono, y una lista de opciones para elegir el tipo de evento.
2. Añade validación básica a los campos usando atributos como `required`, `min`, `max`, y `pattern`.
3. Experimenta con diferentes métodos (`GET` y `POST`) y observa los resultados.
