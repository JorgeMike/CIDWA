# Módulo 8: Animaciones y Transiciones

En este módulo aprenderás a dar vida a tus páginas web con efectos visuales dinámicos utilizando animaciones y transiciones en CSS. 

---

## Objetivos del Módulo

1. Comprender cómo funcionan las transiciones en CSS.
2. Aprender a crear animaciones utilizando `@keyframes`.
3. Combinar animaciones y transiciones para mejorar la experiencia del usuario.
4. Aplicar técnicas avanzadas para crear efectos visuales atractivos.

---

## Contenido

### 8.1 Transiciones en CSS

Las transiciones permiten animar cambios en las propiedades CSS de un elemento. Esto se logra especificando una duración y una propiedad a animar.

#### Propiedades clave de las transiciones:

- `transition-property`: Define qué propiedades serán animadas.
- `transition-duration`: Especifica la duración de la transición.
- `transition-timing-function`: Controla la aceleración de la transición.
- `transition-delay`: Establece un retraso antes de iniciar la transición.

#### Ejemplo básico:
```css
.button {
  background-color: blue;
  transition: background-color 0.3s ease;
}

.button:hover {
  background-color: green;
}
```

### 8.2 Animaciones con `@keyframes`

Las animaciones en CSS permiten crear secuencias más complejas de cambios de propiedades, definidas en pasos intermedios dentro de `@keyframes`.

#### Sintaxis básica de `@keyframes`:
```css
@keyframes example {
  0% {
    transform: translateX(0);
  }
  50% {
    transform: translateX(50px);
  }
  100% {
    transform: translateX(0);
  }
}
```

#### Propiedades relacionadas con las animaciones:

- `animation-name`: Especifica el nombre de la animación.
- `animation-duration`: Duración de la animación.
- `animation-timing-function`: Controla la aceleración de la animación.
- `animation-delay`: Establece un retraso antes de iniciar la animación.
- `animation-iteration-count`: Define cuántas veces se repite la animación.
- `animation-direction`: Establece la dirección de la animación (normal, inversa, alterna).

#### Ejemplo:
```css
.box {
  width: 100px;
  height: 100px;
  background-color: red;
  animation: example 2s infinite;
}

@keyframes example {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.5);
  }
  100% {
    transform: scale(1);
  }
}
```

### 8.3 Combinando Transiciones y Animaciones

Las transiciones y animaciones se pueden combinar para lograr efectos más impactantes. Por ejemplo, utilizar una transición para suavizar el cambio de color mientras una animación mueve el elemento.

#### Ejemplo combinado:
```css
.card {
  width: 200px;
  height: 200px;
  background-color: lightblue;
  transition: box-shadow 0.5s ease;
  animation: move 3s infinite alternate;
}

.card:hover {
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
}

@keyframes move {
  from {
    transform: translateY(0);
  }
  to {
    transform: translateY(-20px);
  }
}
```

### 8.4 Técnicas avanzadas

#### Animaciones personalizadas con múltiples pasos:
```css
@keyframes complexAnimation {
  0% {
    opacity: 0;
    transform: translateY(-50px);
  }
  50% {
    opacity: 1;
    transform: translateY(0);
  }
  100% {
    opacity: 0.5;
    transform: translateY(20px);
  }
}
```

---

## Actividades prácticas

1. **Transiciones**: Crea un botón que cambie de color y tamaño al pasar el cursor.
2. **Animaciones**: Diseña un cuadro que rebote indefinidamente.
3. **Combinaciones**: Implementa una tarjeta interactiva con animaciones y transiciones al hacer hover.
