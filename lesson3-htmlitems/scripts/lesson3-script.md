# 🎓 Guión — Lección 3: Elementos HTML comunes

---

## 🎬 Introducción — Nuestra página empieza a crecer

> "Hasta ahora ya sabemos construir la estructura básica de un documento HTML."

"Tenemos nuestro `<html>`, nuestro `<head>`, nuestro `<body>`, y podemos colocar títulos y párrafos."

"Pero una página web real necesita mucho más que eso."

"Necesitamos organizar información, mostrar imágenes, crear enlaces y presentar listas."

"Hoy vamos a conocer varios de los elementos HTML que más vamos a utilizar durante este curso."

"Y lo mejor es que vamos a empezar a ampliar la página que ya construimos."

---

## 🏷️ Encabezados: `<h1>` hasta `<h3>`

"Comencemos con los encabezados."

"En HTML podemos utilizar diferentes niveles de encabezado."

"El más importante es `<h1>`."

```html id="2h9q7r"
<h1>Mi página web</h1>
```

"`h1` representa el encabezado principal de nuestra página."

"Después podemos utilizar `<h2>` para secciones dentro de nuestra página."

```html id="q3s2cb"
<h2>Mis intereses</h2>
```

"Y también tenemos `<h3>` para subsecciones."

```html id="7k5r6p"
<h3>Videojuegos favoritos</h3>
```

"Podemos imaginarlo como una organización de títulos:"

```text id="kq4q6r"
<h1>Mi página web</h1>

    <h2>Mis intereses</h2>

        <h3>Videojuegos</h3>

        <h3>Películas</h3>

    <h2>Sobre mí</h2>
```

"Por ahora vamos a trabajar principalmente con `<h1>`, `<h2>` y `<h3>`."

"Lo importante es que los utilicemos para **organizar el contenido**, no simplemente para conseguir un texto más grande."

---

## 📝 Párrafos: `<p>`

"Ya conocemos `<p>` de las lecciones anteriores."

"Esta etiqueta representa un párrafo."

```html id="b2r5s9"
<p>
    Me gusta aprender desarrollo web y crear mis propias páginas.
</p>
```

"Podemos utilizar tantos párrafos como necesitemos."

"Por ejemplo, una sección puede tener un encabezado y varios párrafos debajo."

```html id="2a3w9f"
<h2>Sobre mí</h2>

<p>Estoy aprendiendo HTML.</p>

<p>En el futuro quiero crear mis propios sitios web.</p>
```

"Así conseguimos que nuestro contenido sea mucho más fácil de leer y organizar."

---

## 📋 Listas: `<ul>`, `<ol>` y `<li>`

"Ahora vamos a aprender algo especialmente útil: las listas."

"Existen dos tipos principales que utilizaremos."

"Primero tenemos las listas **no ordenadas**, usando `<ul>`."

```html id="3x4z1m"
<p>Lista de hobbys:</p>

<ul>
    <li>Videojuegos</li>
    <li>Música</li>
    <li>Películas</li>
</ul>
```

"El resultado será una lista con elementos marcados."

"Cada elemento de la lista se escribe utilizando `<li>`."

"`li` significa *list item*, es decir, elemento de lista."

"También tenemos las listas **ordenadas**, utilizando `<ol>`."

```html id="0kq6jv"
<p>Pasos para este curso:</p>

<ol>
    <li>Encender el ordenador</li>
    <li>Abrir el navegador</li>
    <li>Empezar a programar</li>
</ol>
```

"En este caso el navegador muestra los elementos utilizando una numeración."

"Entonces podemos recordar la diferencia de esta manera:"

```text id="3l5r8d"
<ul> → lista sin orden específico
<ol> → lista ordenada
<li> → elemento dentro de la lista
```

"No necesitamos inventar los números nosotros mismos. HTML se encarga de la numeración cuando utilizamos `<ol>`."

---

## 🖼️ Imágenes: `<img>`

"Una página web también puede contener imágenes."

"Para eso utilizamos `<img>`."

```html id="p7r4a2"
<img src="imagen.jpg" alt="Descripción de la imagen">
```

"Aquí aparecen dos atributos importantes."

"`src` indica **dónde está la imagen** que queremos mostrar."

"`alt` proporciona un texto alternativo que describe la imagen."

"Por ejemplo:"

```html id="5h7q2c"
<img 
    src="https://picsum.photos/400/250"
    alt="Paisaje de ejemplo"
>
```

"En este caso estamos utilizando una dirección web como fuente de la imagen."

"Hay algo diferente en `<img>` que debemos notar."

"No tenemos un elemento con contenido entre una etiqueta de apertura y una de cierre como ocurría con `<p>`."

"`img` es un elemento que utilizamos para insertar una imagen."

"Por ahora no necesitamos preocuparnos demasiado por todos sus detalles. Lo importante es entender que `src` nos dice **qué imagen mostrar** y `alt` nos dice **qué representa**."

---

## 🔗 Enlaces: `<a>`

"El último elemento que veremos hoy es uno de los más importantes de la web: los enlaces."

"Los enlaces permiten navegar hacia otra página."

"Para crear uno utilizamos `<a>`."

```html id="8m1r6v"
<a href="https://www.wikipedia.org">
    Visitar Wikipedia
</a>
```

"`href` indica **a dónde nos llevará el enlace**."

"El texto que colocamos entre `<a>` y `</a>` es lo que el usuario verá y podrá seleccionar."

"Por ejemplo:"

```html id="q7t3ne"
<a href="https://www.youtube.com">
    Visitar YouTube
</a>
```

"Cuando hacemos clic sobre el texto, el navegador puede llevarnos a la dirección indicada."

"Y esto es una de las ideas fundamentales de la web: **las páginas pueden conectarse entre sí mediante enlaces**."

---

## 🧩 Juntando todos los elementos

"Ahora vamos a combinar todo lo que hemos aprendido."

"Imaginemos que estamos creando una página sobre nuestros intereses."

```html id="s3f9kx"
<h1>Mis intereses</h1>

<p>
    Estas son algunas cosas que me gustan.
</p>

<h2>Videojuegos</h2>

<ul>
    <li>Hollow Knight</li>
    <li>Minecraft</li>
    <li>Portal</li>
</ul>

<h2>Mis lugares favoritos</h2>

<img 
    src="https://picsum.photos/400/250"
    alt="Imagen de un paisaje"
>

<h2>Enlaces</h2>

<p>
    Puedes encontrar más información en
    <a href="https://www.wikipedia.org">
        Wikipedia
    </a>.
</p>
```

"Ya tenemos una página mucho más completa."

"Tenemos encabezados para organizar las secciones, párrafos para explicar información, una lista para nuestros intereses, una imagen y un enlace."

"Y lo más importante: **no hemos necesitado utilizar una etiqueta diferente para cada línea de texto**."

"Cada elemento tiene una función concreta."

---

## 🧠 ¿Cómo elegir qué elemento utilizar?

"Cuando estamos escribiendo HTML, una buena pregunta que podemos hacernos es:

**¿Qué representa este contenido?**"

"Si es el título principal, podemos utilizar `<h1>`."

"Si es una sección, `<h2>`."

"Si es un párrafo, `<p>`."

"Si tenemos varios elementos relacionados, podemos utilizar una lista."

"Si queremos mostrar una imagen, utilizamos `<img>`."

"Y si queremos permitir que alguien visite otra página, utilizamos `<a>`."

"Esta forma de pensar es más importante que memorizar las etiquetas."

"HTML no consiste en decorar texto. Consiste en **describir y organizar el contenido**."

---

## 🧪 Actividad — Amplía tu página

"Ahora vamos a volver a la página que construimos en la lección anterior."

"Esta vez vamos a convertirla en una página mucho más completa."

### Tu página debe incluir:

- Un `<h1>` como título principal.
- Al menos dos `<h2>` para organizar secciones.
- Al menos un `<h3>`.
- Dos párrafos utilizando `<p>`.
- Una lista no ordenada utilizando `<ul>` y `<li>`.
- Una lista ordenada utilizando `<ol>` y `<li>`.
- Una imagen utilizando `<img>`.
- Un enlace utilizando `<a>`.

"Puedes mantener el mismo tema que utilizaste en la lección anterior o cambiar completamente de tema."

"Por ejemplo, podrías crear una página sobre tus videojuegos favoritos, una película, un deporte, una mascota o cualquier otro tema que te interese."

"Lo importante es que cada elemento tenga sentido dentro del contenido."

---

## 🚀 Cierre

"Hoy nuestra página pasó de ser un simple documento con un título y unos párrafos a tener diferentes tipos de contenido."

"Ya podemos organizar información, crear listas, mostrar imágenes y conectar nuestra página con otras mediante enlaces."

"Pero probablemente también hayas notado algo..."

"Por ahora, nuestras páginas siguen teniendo una apariencia bastante sencilla."

"Eso está a punto de cambiar."

"En la siguiente lección vamos a conocer **CSS** y aprenderemos cómo transformar la apariencia de nuestras páginas: colores, tamaños, fuentes, espacios y mucho más."

**¡Nos vemos en la siguiente lección! 👋**