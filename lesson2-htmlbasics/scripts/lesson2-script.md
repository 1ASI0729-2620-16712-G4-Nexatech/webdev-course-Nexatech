# 🎓 Guión — Lección 2: Estructura HTML básica

---

## 🎬 Introducción — Ahora sí, vamos a mirar dentro

> "En la lección anterior descubrimos qué es una página web y conocimos a nuestros dos protagonistas: **HTML y CSS**."

"También modificamos algunos elementos de una página y vimos que unas pocas etiquetas HTML pueden convertirse en contenido visible en el navegador."

"Pero seguramente quedó una pregunta:

**¿Por qué todos esos elementos están escritos de esa manera?**

¿Por qué tenemos etiquetas como `<html>`, `<head>`, `<body>`, `<h1>` y `<p>`?"

"Hoy vamos a conocer la estructura básica que tienen prácticamente todos los documentos HTML."

---

## 🏗️ ¿Qué es la estructura HTML?

"Un documento HTML tiene una estructura organizada."

"Esto es importante porque el navegador necesita saber **qué contiene nuestro documento y cómo está organizado**."

"Podemos imaginarlo como un documento con diferentes partes."

"Primero tenemos una parte exterior que contiene todo nuestro documento HTML."

```html
<html>
    ...
</html>
```

"Dentro de ella encontraremos principalmente dos grandes secciones:

- `<head>`
- `<body>`"

"Y cada una tiene una función diferente."

> **Nota visual:** Mostrar una estructura HTML completa y señalar cada sección en una pestaña de CodePen.

```text
<html>
│
├── <head>
│     Información del documento
│
└── <body>
      Contenido visible
</html>
```

"Vamos a conocerlas una por una."

---

## 🧠 `<html>`: el elemento principal

"Empecemos por `<html>`."

"Esta etiqueta representa el **documento HTML completo**."

"Todo el contenido de nuestra página se encuentra dentro de ella."

```html
<html>
    
    <!-- Todo nuestro documento va aquí -->

</html>
```

"Fíjense en algo importante."

"Tenemos una etiqueta de apertura:"

```html
<html>
```

"Y una etiqueta de cierre:"

```html
</html>
```

"La etiqueta de cierre tiene una barra `/`."

"Esta idea de apertura y cierre va a aparecer constantemente en HTML."

---

## 🏷️ Etiquetas y elementos

"Antes de continuar, tenemos que aclarar dos conceptos: **etiquetas y elementos**."

"Una etiqueta es algo como esto:"

```html
<p>
```

"Nos indica qué tipo de contenido estamos utilizando."

"Cuando combinamos una etiqueta de apertura, su contenido y una etiqueta de cierre, tenemos un **elemento HTML**."

```html
<p>Hola, mundo</p>
```

"En este caso, `<p>` es la etiqueta de apertura, `Hola, mundo` es el contenido y `</p>` es la etiqueta de cierre."

"Todo junto forma un elemento de párrafo."

"Por ahora no necesitamos memorizar una lista enorme de etiquetas."

"Lo importante es entender esta idea:

> **Las etiquetas describen y organizan el contenido de nuestra página.**"

---

## 🧠 `<head>`: información sobre la página

"Ahora vamos con `<head>`."

"El `<head>` contiene información **sobre el documento**, pero normalmente no es el contenido principal que vemos directamente en la página."

"Por ejemplo, aquí podemos colocar el título que aparece en la pestaña del navegador."

```html
<head>

    <title>Mi primera página</title>

</head>
```

"Si abrimos esta página en el navegador, no veremos `Mi primera página` como un título **dentro** del contenido."

"Lo veremos aquí arriba, en la pestaña del navegador."

> **Nota visual:** Mostrar una pestaña suelta del navegador y señalar el `<title>`.

"Más adelante encontraremos otras cosas dentro de `<head>`, especialmente cuando trabajemos con CSS."

"Por ahora basta con recordar:

**`<head>` contiene información y configuración del documento.**"

---

## 👀 `<body>`: lo que vemos

"Y ahora llegamos al `<body>`."

"El `<body>` contiene el **contenido que normalmente vemos en la página**."

"Por ejemplo:"

```html
<body>

    <h1>Mi primera página</h1>

    <p>Estoy aprendiendo HTML.</p>

</body>
```

"El navegador mostrará el título y el párrafo dentro de la página."

"Podemos pensar en la diferencia de esta manera:"

```text
<head>
    Información sobre la página
</head>

<body>
    Contenido de la página
</body>
```

"El `<head>` prepara información para el documento."

"El `<body>` contiene aquello que vamos a mostrar."

---

## 📝 `<h1>` y `<p>`: nuestro contenido

"Dentro del `<body>` podemos utilizar diferentes **elementos** para organizar nuestro contenido."

"Uno de los más importantes es `<h1>`."

```html
<h1>Mi página web</h1>
```

"`h1` representa un **título principal**."

"También tenemos `<p>`, que utilizamos para los párrafos."

```html
<p>Este es un párrafo de mi página web.</p>
```

"Así podemos comenzar a construir una página bastante sencilla."

```html
<body>

    <h1>Sobre mí</h1>

    <p>Hola, soy Diego y estoy aprendiendo desarrollo web.</p>

</body>
```

"Y aquí empieza a verse la verdadera utilidad de HTML."

"No estamos diciéndole solamente al navegador qué texto mostrar."

"También estamos indicando **qué función cumple cada parte del contenido**."

---

## 🧩 Construyendo el documento completo

"Ahora podemos juntar todas las piezas que acabamos de aprender."

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <title>Mi primera página</title>
</head>

<body>

    <h1>¡Hola, mundo!</h1>

    <p>Esta es mi primera página creada con HTML.</p>

</body>

</html>
```

"Vamos a recorrerlo rápidamente."

"`<!DOCTYPE html>` le indica al navegador que estamos trabajando con un documento HTML moderno."

"`<html>` contiene todo nuestro documento."

"`<head>` contiene información sobre la página."

"`<title>` establece el título de la pestaña."

"`<body>` contiene el contenido visible."

"Y dentro del body tenemos nuestro `<h1>` y nuestro `<p>`."

> **Nota visual:** Resaltar cada sección del código mientras se explica.

---

## 🔍 Una última idea: HTML como estructura

"Si recuerdan la comparación de la primera lección, podemos volver a pensar en HTML como la estructura de una casa."

"El documento completo sería nuestra casa."

"`<head>` contiene información necesaria para preparar el documento."

"`<body>` es el espacio donde colocamos nuestro contenido."

"Y dentro del body podemos tener títulos, párrafos, imágenes, enlaces y muchos otros elementos."

"Más adelante aprenderemos muchas más etiquetas, pero todas seguirán esta misma idea:

**HTML nos permite organizar el contenido de nuestra página.**"

---

## 🧪 Actividad — Construye tu propia página

"Ahora es tu turno."

"Vamos a crear una página HTML desde cero."

"Tu página debe tener como mínimo:"

- Un documento HTML correctamente estructurado.
- Un título para la pestaña usando `<title>`.
- Un título principal usando `<h1>`.
- Al menos dos párrafos usando `<p>`.

"El contenido puede ser sobre cualquier cosa que te interese."

"Puede ser una presentación personal, tu videojuego favorito, una mascota, una película o incluso una página completamente llena de ideas aleatorias. Todo vale."

"Lo importante es que tú decidas qué contenido quieres organizar."

---

## 🚀 Cierre

"Hoy aprendimos que un documento HTML no es simplemente un montón de etiquetas."

"Tiene una estructura."

```text
<html>
 ├── <head>
 │    └── Información del documento
 │
 └── <body>
      ├── <h1>
      └── <p>
```

"Y ahora que conocemos esa estructura, podemos empezar a añadir cada vez más contenido."

"En la siguiente lección vamos a aprender cómo trabajar con **texto, enlaces, imágenes y listas** para que nuestras páginas empiecen a parecer sitios web de verdad."

**¡Nos vemos en la siguiente lección! 👋**