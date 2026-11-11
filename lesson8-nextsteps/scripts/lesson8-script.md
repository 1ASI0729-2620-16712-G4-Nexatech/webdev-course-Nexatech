# 🎓 Guión — Lección 8: Buenas prácticas y próximos pasos

---

## 🎬 Introducción — ¿Y si algo sale mal?

> "Durante este curso hemos construido nuestra propia página web utilizando HTML y CSS."

"Ya sabemos crear contenido, organizarlo, añadir imágenes y enlaces, y modificar su apariencia."

"Pero hay algo que cualquier persona que programe aprende tarde o temprano: **a veces nuestro código no funciona como esperábamos**."

"Puede faltar una etiqueta, podemos escribir algo incorrectamente o simplemente podemos cambiar una propiedad y descubrir que el resultado no era el que imaginábamos."

"Y eso no significa que hayamos fracasado."

"Significa que tenemos una oportunidad para **aprender a encontrar el problema**."

---

## 🔎 Cuando algo no funciona

"Supongamos que escribimos este código:"

```html
<h1>Mi página<h1>
```

"Quizás esperábamos tener un título correctamente cerrado."

"Pero hay un pequeño problema."

"La etiqueta de cierre debería tener una barra."

```html
<h1>Mi página</h1>
```

"Cuando algo no funciona, lo primero que podemos hacer es **leer nuestro código con calma**."

"Podemos revisar si las etiquetas están correctamente escritas y si las etiquetas que necesitan cierre realmente tienen su cierre."

> **Nota visual:** Mostrar primero el código incorrecto y después corregir únicamente la etiqueta de cierre.

---

## ⚠️ Los errores también enseñan

"Otro ejemplo podría aparecer en CSS."

"Supongamos que queremos cambiar el color de un título:"

```css
h1 {
    color: purple;
}
```

"Pero escribimos accidentalmente:"

```css
h1 {
    color purple;
}
```

"En este caso falta algo importante: el símbolo `:` entre la propiedad y su valor."

"La versión correcta es:"

```css
h1 {
    color: purple;
}
```

"Por eso, cuando un estilo no funciona, podemos revisar tres cosas:"

```text
1. ¿Escribí correctamente el selector?

2. ¿Escribí correctamente la propiedad?

3. ¿Separé la propiedad y el valor correctamente?
```

> **Nota visual:** Mostrar el error de CSS y señalar visualmente el lugar donde falta `:`.

---

## 🧪 Cambiar una cosa a la vez

"También hay una estrategia muy útil cuando estamos aprendiendo."

> **Cambiar una cosa a la vez.**

"Por ejemplo, si queremos experimentar con el título, podemos cambiar primero su color."

```css
h1 {
    color: purple;
}
```

"Después podemos cambiar su tamaño."

```css
h1 {
    color: purple;
    font-size: 40px;
}
```

"Y después podemos probar con el espacio."

```css
h1 {
    color: purple;
    font-size: 40px;
    padding: 20px;
}
```

"De esta manera podemos observar qué efecto produce cada cambio."

"Si modificamos diez cosas al mismo tiempo y algo sale mal, será mucho más difícil saber cuál cambio provocó el problema."

> **Nota visual:** Mostrar el CSS y agregar cada propiedad una por una, observando el resultado después de cada cambio.

---

## 🧠 Tres hábitos para seguir aprendiendo

"Durante el curso hemos aprendido muchas cosas, pero también podemos llevarnos algunos hábitos para continuar."

### 1. Mantén tu código organizado

"Utiliza sangrías, separa las diferentes partes y escribe títulos claros."

### 2. Prueba tus cambios

"No tengas miedo de modificar un color, cambiar un tamaño o probar otra estructura."

"Si algo no funciona, puedes volver atrás y analizar qué ocurrió."

### 3. Experimenta

"Una de las mejores formas de aprender desarrollo web es preguntarse:

**¿Qué pasaría si cambio esto?**"

"Puedes cambiar colores, tamaños, textos, listas o cualquier otra cosa que ya conozcas."

"Experimentar convierte el código en algo que podemos descubrir, no solamente memorizar."

---

## 🌐 ¿Qué podemos aprender después?

"Y este curso no tiene que terminar aquí."

"HTML y CSS tienen muchísimas más posibilidades."

"Podemos seguir aprendiendo a crear páginas más completas, utilizar nuevas propiedades de CSS y organizar nuestros proyectos de diferentes maneras."

"Más adelante también podemos conocer **JavaScript**, que permite añadir comportamiento e interacción a nuestras páginas."

> **Nota visual:** Mostrar una progresión sencilla.

```text
HTML
  ↓
Estructura y contenido

CSS
  ↓
Apariencia y diseño

JavaScript
  ↓
Interacción y comportamiento
```

"Pero no necesitamos aprenderlo todo de una vez."

"Lo importante es seguir practicando y construir proyectos cada vez más completos."

---

## 🎤 Actividad final — Comparte tu proyecto

"Ahora llegamos al final del curso."

"Cada uno tiene una página web construida a partir de su propia idea."

"Vamos a compartir nuestro proyecto y explicar brevemente qué hemos creado."

> **Nota visual:** Mostrar una página terminada en el navegador mientras se explica.

"Puedes contar:"

- Qué tema elegiste.
- Qué parte de tu página te gusta más.
- Qué elemento HTML utilizaste.
- Qué cambio de CSS te pareció más interesante.
- Qué te gustaría agregar si tuvieras más tiempo.

"No importa si tu página no quedó exactamente como la imaginabas."

"Lo importante es que **la construiste tú y ahora sabes cómo modificarla**."

---

## 🚀 Cierre — Esto es solo el comienzo

"Durante este curso aprendimos a construir una página web desde cero."

"Aprendimos que HTML organiza el contenido."

"Aprendimos que CSS controla su apariencia."

"Y también aprendimos algo que será importante para cualquier proyecto futuro: **los errores forman parte del proceso de aprendizaje**."

> **HTML → estructura**  
> **CSS → apariencia**  
> **Práctica → experiencia**

"Ahora ya puedes abrir tu código, cambiarlo, experimentar y construir algo nuevo."

"Así que no pienses en esta página como el final del curso."

"Piensa en ella como **tu primer proyecto web**."

"Hay mucho más que te espera por delante."

**¡Felicitaciones por completar el curso! 🎉🌐**

**#WebDevBeginners**
