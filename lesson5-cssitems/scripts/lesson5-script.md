# Lección 5: Estilos y diseño simple

## Introducción

En la lección anterior aprendimos selectores, propiedades y valores. Pero nuestra página todavía se ve sencilla: necesita espacio, separación y mejor organización.

Hoy aprenderemos cinco propiedades de CSS: `margin`, `padding`, `border`, `background-color` y `text-align`. Las aplicaremos sobre nuestra página de intereses.

---

## 1. Background-color: color de fondo

Empezamos con el `body`, que representa todo el cuerpo de la página.

```css
body {
    background-color: #f2f2f2;
}
```

Con `background-color` cambiamos el color de fondo. Aquí usamos un gris claro.

---

## 2. Margin: espacio exterior

`margin` controla el espacio **alrededor** de un elemento.

```css
p {
    margin: 20px;
}
```

Dejamos 20 píxeles alrededor de cada párrafo. El contenido se ve más ordenado.

---

## 3. Padding: espacio interior

`padding` controla el espacio **dentro** del elemento, entre el texto y los límites de su caja.

```css
h1 {
    padding: 15px;
}
```

Prueba cambiarlo a 30px. Cuanto mayor el valor, mayor el espacio interior.

> **Recuerda:** `margin` = espacio exterior, `padding` = espacio interior.

---

## 4. Border: bordes

Los bordes nos ayudan a ver mejor estos espacios.

```css
h1 {
    padding: 15px;
    border: 2px solid #5b2c83;
}
```

Estructura de la propiedad:

```css
border: grosor estilo color;
```

- `2px`: grosor
- `solid`: línea continua
- `#5b2c83`: color

Observa cómo el `padding` crea espacio entre el texto y el borde.

---

## 5. Estilos para los subtítulos (h2)

Combinamos fondo, color de texto, padding y borde:

```css
h2 {
    background-color: #d9c2e9;
    color: #3d1f5c;
    padding: 10px;
    border: 2px solid #5b2c83;
}
```

Con pocas propiedades, los subtítulos ya destacan.

---

## 6. Text-align: alineación del texto

Por defecto el texto se alinea a la izquierda. Con `text-align` lo cambiamos:

```css
h1 {
    text-align: center;
}
```

Valores posibles:

```css
text-align: left;
text-align: center;
text-align: right;
```

Dejaremos el título principal centrado.

---

## 7. Juntando todo

```css
/* ===== PÁGINA ===== */
body {
    background-color: #f2f2f2;
}

/* ===== TÍTULO PRINCIPAL ===== */
h1 {
    color: #5b2c83;
    text-align: center;
    padding: 15px;
    border: 2px solid #5b2c83;
}

/* ===== SECCIONES ===== */
h2 {
    background-color: #d9c2e9;
    color: #3d1f5c;
    padding: 10px;
    border: 2px solid #5b2c83;
}

/* ===== PÁRRAFOS ===== */
p {
    color: #333333;
    margin: 20px;
}
```

El HTML sigue igual; solo cambió la presentación. Eso es lo poderoso de CSS.

---

## 8. Actividad: mejora el diseño de tu página

En tu página de intereses, usa:

- `margin` para separar elementos
- `padding` para crear espacio interior
- `border` para agregar al menos un borde
- `background-color` para cambiar un fondo
- `text-align` para alinear algún texto

Experimenta: cambia el `padding` de 10px a 30px, prueba otros colores y grosores de borde. El objetivo no es una página perfecta, sino entender qué hace cada propiedad.

---

## Cierre

- `margin`: espacio exterior
- `padding`: espacio interior
- `border`: bordes
- `background-color`: color de fondo
- `text-align`: alineación del texto

En la siguiente lección pondremos todo en práctica para construir una página web más completa, combinando HTML y CSS.

¡Nos vemos en la próxima lección!