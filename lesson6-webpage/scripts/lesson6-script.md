# 🎓 Guión — Lección 6: Construyendo una página web completa

---

## 🎬 Introducción — Ahora vamos a construir algo nuestro

> "Hasta ahora hemos aprendido las piezas principales que necesitamos para crear una página web."

"Primero aprendimos qué son HTML y CSS."

"Después construimos la estructura básica de un documento HTML."

"Aprendimos a utilizar títulos, párrafos, listas, imágenes y enlaces."

"Y finalmente comenzamos a utilizar CSS para cambiar colores, tamaños, espacios, bordes, fondos y alineación."

"Hoy vamos a hacer algo diferente."

"En lugar de aprender una propiedad nueva tras otra, vamos a **utilizar todo lo que ya conocemos para construir una página web completa**."

"Y esta vez la idea será nuestra."

---

## 💡 Antes de escribir código: piensa en tu página

"Antes de abrir CodePen y empezar a escribir etiquetas, necesitamos decidir qué vamos a construir."

"Una página web no empieza con código."

"Empieza con una idea."

"Puede ser cualquier tema que te interese."

### Algunas posibilidades:

- 🎮 Un videojuego favorito.
- 🎬 Una película o serie.
- 🐶 Una mascota.
- ⚽ Un deporte.
- 🎵 Un artista o género musical.
- 📚 Un libro.
- 🌎 Un lugar que te gustaría visitar.
- 🚀 Un tema que te gustaría explicar.

"Lo importante es que podamos organizar la información en diferentes secciones."

"Por ejemplo, si queremos crear una página sobre un videojuego, podríamos tener:"

```text id="w8m3pa"
Mi videojuego favorito
│
├── Introducción
│
├── Personajes
│
├── Características
│
└── Más información
```

"Esto nos da una estructura antes de escribir código."

> **Primero pensamos qué queremos comunicar. Después decidimos cómo organizarlo.**

---

## 🧱 Paso 1 — Construimos la estructura HTML

"Vamos a comenzar únicamente con HTML."

"Por ahora no nos preocuparemos por los colores ni por el diseño."

"Primero necesitamos construir el contenido."

"Nuestro documento puede comenzar así:"

```html id="c5t7vq"
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <title>Mi página</title>
</head>

<body>

    <h1>Mi página web</h1>

</body>

</html>
```

"Ya tenemos la estructura básica que aprendimos en la segunda lección."

"Ahora vamos a añadir nuestras secciones."

```html id="r4k8sn"
<h1>Mi videojuego favorito</h1>

<h2>¿De qué trata?</h2>

<p>
    Aquí podemos explicar brevemente de qué trata
    nuestro videojuego.
</p>

<h2>Características</h2>

<ul>
    <li>Exploración</li>
    <li>Combates</li>
    <li>Historia</li>
</ul>
```

"Fíjense en algo."

"No estamos utilizando una etiqueta diferente para cada tipo de contenido."

"Estamos reutilizando los elementos que ya conocemos."

"`h1` para el título principal."

"`h2` para las secciones."

"`p` para explicar información."

"`ul` y `li` para organizar elementos relacionados."

"Esto demuestra algo importante."

> **Aprender HTML no consiste en memorizar cientos de etiquetas. Consiste en saber qué elemento representa mejor cada parte de nuestro contenido.**

---

## 🗂️ Paso 2 — Organizamos el contenido

"Ahora podemos añadir más información."

"Por ejemplo, podemos incluir una imagen."

```html id="x2n7bc"
<h2>Una imagen</h2>

<img
    src="https://picsum.photos/500/300"
    alt="Imagen relacionada con el tema"
>
```

"También podemos añadir un enlace."

```html id="p9m4zk"
<h2>Más información</h2>

<p>
    Puedes encontrar más información
    <a href="https://www.wikipedia.org">
        en este enlace
    </a>.
</p>
```

"Ahora nuestra página tiene diferentes tipos de contenido."

"Podemos empezar a pensar en ella como una pequeña estructura de información."

```text id="d6q1vz"
<h1>
    Título principal
</h1>

<h2>
    Sección
</h2>

<p>
    Información
</p>

<ul>
    Lista de elementos
</ul>

<img>
    Imagen

<a>
    Enlace
```

"Y todo esto vive dentro del `body`."

---

## 🎨 Paso 3 — Ahora entra CSS

"Una vez que tenemos nuestra estructura, podemos empezar a trabajar en la presentación."

"Vamos a abrir el panel CSS de CodePen."

"Y aquí podemos comenzar con algo sencillo."

```css id="j8v2mt"
body {
    background-color: #f2f2f2;
}
```

"Ya tenemos un fondo para toda la página."

"Ahora podemos trabajar con nuestro título principal."

```css id="n5r7qx"
h1 {
    color: #5b2c83;
    text-align: center;
    padding: 15px;
    border: 2px solid #5b2c83;
}
```

"Con una sola regla estamos modificando varias características del mismo elemento."

"Estamos cambiando su color."

"Estamos centrando el texto."

"Estamos añadiendo espacio interior."

"Y estamos creando un borde."

"Después podemos trabajar con nuestros encabezados secundarios."

```css id="a3k6wp"
h2 {
    background-color: #d9c2e9;
    padding: 10px;
    border: 2px solid #5b2c83;
}
```

"Y finalmente podemos mejorar nuestros párrafos."

```css id="q7m2cz"
p {
    color: #333333;
    margin: 20px;
}
```

"De esta forma, poco a poco, nuestra página empieza a tener una identidad visual."

---

## 🔄 HTML y CSS trabajando juntos

"Ahora quiero que nos detengamos un momento."

"Tenemos dos archivos o dos áreas diferentes en CodePen."

```text id="h5x9rp"
HTML
│
├── Título
├── Secciones
├── Párrafos
├── Listas
├── Imágenes
└── Enlaces

        ↓

CSS
│
├── Colores
├── Fondos
├── Espacios
├── Bordes
└── Alineación
```

"Pero el resultado que vemos en pantalla es uno solo."

"Esto ocurre porque HTML y CSS trabajan juntos."

"Por ejemplo, HTML puede crear esto:"

```html id="b8v4ns"
<h2>Características</h2>
```

"Y CSS puede decidir cómo queremos presentarlo:"

```css id="f3y7ka"
h2 {
    background-color: lightblue;
    padding: 10px;
}
```

"El HTML sigue representando un encabezado."

"CSS simplemente controla su presentación."

"Esta separación nos permite modificar el diseño sin tener que cambiar todo nuestro contenido."

---

## 🧩 Paso 4 — Construimos una página completa

"Ahora vamos a juntar todo."

"Nuestro proyecto puede tener una estructura como esta:"

```text id="r2k8mf"
Mi página web
│
├── Título principal
│
├── Introducción
│   └── Párrafo
│
├── Información principal
│   ├── Párrafo
│   └── Lista
│
├── Imagen
│
└── Más información
    └── Enlace
```

"Esta estructura es solamente un ejemplo."

"Ustedes pueden utilizar un tema completamente diferente."

"Lo importante es que la página tenga una organización clara."

---

## 🧠 Paso 5 — Piensa como diseñador

"Ahora que sabemos construir la página, podemos empezar a tomar pequeñas decisiones de diseño."

"Pregúntate:"

### 🎨 ¿Qué colores quiero utilizar?

"Puedes elegir colores que combinen con el tema de tu página."

### 📐 ¿Qué elementos necesitan espacio?

"Si varios elementos están demasiado juntos, podemos utilizar `margin` o `padding`."

### 🧱 ¿Qué elementos quiero destacar?

"Podemos utilizar un fondo o un borde para destacar determinadas secciones."

### ↔️ ¿Cómo quiero alinear el contenido?

"Podemos utilizar `text-align` cuando tenga sentido."

"Estas decisiones no tienen una única respuesta correcta."

"Dos personas pueden construir una página sobre el mismo tema y obtener diseños completamente diferentes."

"Lo importante es que puedan explicar **por qué eligieron determinados estilos**."

---

## 🧪 Proyecto — Construye tu propia página web

"Ahora llega la parte principal de la clase."

"Vamos a crear una página web utilizando todo lo que hemos aprendido."

### 📋 Requisitos del proyecto

"Tu página debe incluir como mínimo:"

#### HTML

- Un documento HTML correctamente estructurado.
- Un `<title>` para la pestaña.
- Un `<h1>` como título principal.
- Al menos dos `<h2>` para organizar secciones.
- Al menos tres párrafos.
- Una lista utilizando `<ul>` o `<ol>`.
- Una imagen utilizando `<img>`.
- Un enlace utilizando `<a>`.

#### CSS

"También debe tener estilos propios."

- Un color de fondo utilizando `background-color`.
- Colores para el contenido utilizando `color`.
- Al menos un elemento con `padding`.
- Al menos un elemento con `margin`.
- Al menos un borde utilizando `border`.
- Algún texto alineado utilizando `text-align`.

"Y hay una última condición."

> **La página debe tratar sobre un tema que tú hayas elegido.**

"No importa si eliges videojuegos, música, deportes, películas, animales, tecnología o cualquier otro tema."

"Lo importante es que puedas organizar la información y presentarla utilizando HTML y CSS."

---

## 🛠️ Paso 6 — Construye por partes

"Si intentamos escribir toda la página de una sola vez, es fácil perderse."

"Por eso vamos a dividir el trabajo."

### 1️⃣ Primero: el HTML

"Construye la estructura y coloca tu contenido."

"Comprueba que la página tenga sentido incluso antes de añadir CSS."

```text id="q7w4kn"
¿La información está organizada?
¿Los títulos tienen sentido?
¿Los párrafos explican algo?
¿La lista corresponde al contenido?
¿La imagen tiene una descripción?
¿El enlace funciona?
```

### 2️⃣ Después: el CSS

"Cuando el contenido funcione, empieza a trabajar en la presentación."

"Puedes comenzar con el fondo."

```css id="v6r2jp"
body {
    background-color: ...;
}
```

"Después el título."

```css id="k9m3tw"
h1 {
    color: ...;
    text-align: ...;
    padding: ...;
}
```

"Después las secciones."

```css id="x4p8zc"
h2 {
    background-color: ...;
    border: ...;
    padding: ...;
}
```

"Y finalmente ajusta los espacios."



```css id="m7q2yf"
p {
    margin: ...;
}
```

"De esta forma podemos construir el diseño paso a paso."

> **Nota visual:** Mostrar la esctructura ya completa y señalar cada sección en una pestaña de CodePen.

---

## 🔍 Paso 7 — Revisa tu página

"Cuando hayas terminado, no cierres el proyecto inmediatamente."

"Vamos a revisar nuestro trabajo."

### ✅ Comprobación HTML

"Pregúntate:"

- ¿Mi página tiene un título principal?
- ¿Las secciones están organizadas?
- ¿El contenido se entiende?
- ¿La imagen aparece correctamente?
- ¿El enlace funciona?
- ¿Los elementos están dentro del `body`?

### ✅ Comprobación CSS

"Después revisa el diseño:"

- ¿Tengo un color de fondo?
- ¿Utilicé `margin`?
- ¿Utilicé `padding`?
- ¿Tengo algún borde?
- ¿El texto está alineado como quiero?
- ¿Los colores permiten leer fácilmente el contenido?

"Y finalmente una pregunta importante:"

> **¿El diseño ayuda a entender el contenido?**

"Un buen diseño no consiste simplemente en utilizar muchos colores."

"Consiste en hacer que la información sea clara y fácil de recorrer."

---

## 🧠 Lo que acabamos de construir

"Si completaron el proyecto, acabamos de hacer algo importante."

"Ya no estamos trabajando solamente con ejemplos aislados."

"Tenemos una página que tiene:"

```text id="n4x7mq"
Contenido
    ↓
Estructura
    ↓
Presentación
    ↓
Página completa
```

"Y todo esto utilizando únicamente las herramientas que hemos aprendido hasta ahora."

"Eso significa que ya tenemos una base suficiente para empezar a construir pequeños proyectos propios."

---

## 🚀 Cierre — De aprender propiedades a construir proyectos

"Hoy no aprendimos una gran cantidad de propiedades nuevas."

"Aprendimos algo diferente."

"Aprendimos a **combinar lo que ya sabemos**."

"HTML nos permitió construir la estructura y organizar el contenido."

"CSS nos permitió controlar colores, espacios, bordes, fondos y alineación."

"Y al combinar ambos conseguimos una página web completa."

> **HTML define la estructura.  
> CSS define la presentación.  
> Juntos nos permiten construir páginas web.**

"Y ahora que ya sabemos construir una página desde cero, en las siguientes lecciones vamos a empezar a prestar atención a algo igual de importante: **cómo escribir nuestro código de una manera más clara, ordenada y fácil de mantener**."

**¡Excelente trabajo! Ya construiste tu primera página web completa. Nos vemos en la siguiente lección👋**
