# 🎓 Guión — Lección 5: Estilos y diseño simple

---

## 🎬 Introducción — Nuestra página necesita espacio

> "En la lección anterior aprendimos los fundamentos de CSS."

"Ya sabemos utilizar selectores, propiedades y valores."

"También aprendimos a cambiar colores y tamaños de texto."

"Pero seguramente habrán notado algo."

"Podemos cambiar el color de nuestra página, pero todavía hay algo que hace que muchas páginas se vean bastante simples."

**El contenido está demasiado junto.**

"Los textos necesitan espacio."

"Las secciones necesitan separarse."

"Algunos elementos pueden tener bordes o fondos."

"Y también podemos decidir cómo queremos alinear nuestro contenido."

"Hoy vamos a aprender justamente eso."

"Vamos a utilizar CSS para empezar a **organizar visualmente nuestra página**."

---

## 📦 Antes de empezar: los elementos ocupan espacio

"Para entender lo que vamos a hacer hoy, tenemos que pensar en algo muy sencillo."

"Cada elemento HTML que colocamos en nuestra página ocupa un espacio."

"Por ejemplo:"

```html id="m8r3qk"
<h1>Mi página web</h1>

<p>
    Estoy aprendiendo desarrollo web.
</p>
```

"El navegador coloca estos elementos uno después del otro."

"Pero CSS nos permite controlar mejor el espacio que los rodea."

"Podemos imaginar cada elemento como una pequeña caja."

```text id="7x4n2p"
┌─────────────────────────────┐
│        Mi página web        │
└─────────────────────────────┘

┌─────────────────────────────┐
│ Estoy aprendiendo desarrollo│
│            web.             │
└─────────────────────────────┘
```

"Y alrededor de estas cajas podemos controlar diferentes aspectos."

"Hoy vamos a trabajar principalmente con **espacio, bordes, fondos y alineación**."

---

## ↔️ `margin`: espacio alrededor

"Empecemos con `margin`."

"`margin` controla el **espacio que queda alrededor de un elemento**."

"Por ejemplo:"

```css id="5f7k2a"
h1 {
    margin: 30px;
}
```

"Estamos diciendo que queremos dejar un espacio de 30 píxeles alrededor del `h1`."

"Podemos visualizarlo así:"

```text id="q4m9st"
        espacio
    ←─────────────→

    ┌─────────────┐
    │     h1      │
    └─────────────┘

        espacio
```

"Esto puede ser muy útil cuando tenemos varios elementos y queremos evitar que estén demasiado juntos."

"Por ejemplo, podemos separar nuestros párrafos:"

```css id="j6r8wp"
p {
    margin: 20px;
}
```

"Ahora cada párrafo tendrá espacio alrededor."

> **Idea clave:**
>
> **`margin` = espacio fuera del elemento.**

---

## 📥 `padding`: espacio dentro

"Ahora tenemos otra propiedad que puede parecer muy parecida."

"`padding`."

"Y aquí es donde debemos tener cuidado."

"`padding` también crea espacio, pero **dentro del elemento**."

"Por ejemplo:"

```css id="a2z7kc"
h1 {
    padding: 20px;
}
```

"El texto del `h1` tendrá espacio entre él y los bordes de su propia caja."

"Podemos imaginarlo así:"

```text id="z5r1vx"
┌───────────────────────────────┐
│        padding                │
│    ┌─────────────────────┐    │
│    │        Texto        │    │
│    └─────────────────────┘    │
│        padding                │
└───────────────────────────────┘
```

"Entonces tenemos una diferencia muy importante:"

```text id="k3p9dy"
margin
→ espacio fuera del elemento

padding
→ espacio dentro del elemento
```

"Esta diferencia puede parecer pequeña ahora, pero es fundamental cuando empecemos a diseñar páginas más completas."

---

## 🧱 `border`: añadir un borde

"Ahora que sabemos trabajar con el espacio, podemos añadir un borde y con esto visualizaremos los conceptos anteriores mucho mejor."

"Para eso utilizamos `border`."

```css id="r8c4hm"
h1 {
    border: 2px solid purple;
}
```

"Esta declaración tiene varias partes."

"`2px` indica el grosor del borde."

"`solid` indica el tipo de borde."

"Y `purple` indica su color."

"Podemos verlo de forma simplificada como:"

```text id="v7n2ka"
border: grosor estilo color;
```

"Por ejemplo:"

```css id="q6m1fs"
border: 2px solid purple;
```

"Ahora nuestro elemento tendrá un borde púrpura."

"Podemos combinarlo con `padding`:"

```css id="b4t9xz"
h1 {
    border: 2px solid purple;
    padding: 15px;
}
```

"El borde rodea al elemento y el `padding` crea espacio entre el contenido y ese borde."

"¡Prueba ponerle un `margin` también!"

---

## 🎨 `background-color`: fondos

"Ya utilizamos `background-color` en la lección anterior."

"Ahora vamos a utilizarlo para crear una sección visualmente diferenciada."

"Por ejemplo:"

```css id="n5y2qp"
h2 {
    background-color: lightblue;
}
```

"Ahora cada `h2` tendrá un fondo azul claro."

"Podemos combinarlo con otras propiedades:"

```css id="w3f8kc"
h2 {
    background-color: lightblue;
    padding: 10px;
    border: 2px solid darkblue;
}
```

"Ahora tenemos un encabezado con fondo, espacio interior y borde."

"Esto ya empieza a parecer más una decisión de diseño que simplemente cambiar colores."

---

## ↔️ `text-align`: alinear el texto

"Nos queda una propiedad muy sencilla pero muy útil."

"`text-align`."

"Esta propiedad nos permite controlar la alineación del texto."

"Por defecto, normalmente veremos el texto alineado a la izquierda."

"Podemos cambiarlo utilizando:"

```css id="2x6v8r"
h1 {
    text-align: center;
}
```

"Ahora el texto del `h1` estará centrado."

"También podemos utilizar otros valores."

```css id="8r1m5q"
text-align: left;
text-align: center;
text-align: right;
```

"Por ejemplo, si queremos que los párrafos estén centrados:"

```css id="j9c4wt"
p {
    text-align: center;
}
```

"Esto nos permite controlar rápidamente la organización visual del texto."

---

## 🧩 Juntando todo

"Ahora vamos a combinar las propiedades que acabamos de aprender."

"Imaginemos que tenemos esta sección:"

```html id="c7v2nm"
<h2>Mis videojuegos favoritos</h2>

<p>
    Estos son algunos juegos que me gustan.
</p>
```

"Podemos darle un estilo sencillo:"

```css id="h3k8pq"
h2 {
    background-color: lightblue;
    border: 2px solid darkblue;
    padding: 10px;
    text-align: center;
}

p {
    margin: 20px;
}
```

"Vamos a identificar qué hace cada propiedad."

```text id="f6t2zr"
background-color
→ cambia el fondo

border
→ añade un borde

padding
→ crea espacio dentro

text-align
→ alinea el texto

margin
→ crea espacio alrededor
```

"Y aquí podemos ver cómo varias propiedades diferentes pueden trabajar juntas para conseguir un resultado visual."

---

## 🧠 Una diferencia importante: `margin` y `padding`

"Antes de continuar, quiero que nos quedemos especialmente con esta diferencia que puede ser confusa para un primer contacto."

"Supongamos que tenemos un elemento con un borde."

```css id="x8m3kd"
h2 {
    border: 2px solid purple;
}
```

"Si añadimos `padding`:"

```css id="p4n7ys"
h2 {
    border: 2px solid purple;
    padding: 20px;
}
```

"Estamos aumentando el espacio **entre el texto y el borde**."

"Pero si utilizamos `margin`:"

```css id="z2w6hc"
h2 {
    border: 2px solid purple;
    margin: 20px;
}
```

"Estamos aumentando el espacio **entre este elemento y los elementos que lo rodean**."

"Podemos recordarlo con una frase sencilla:"

> **`padding` empuja el contenido desde dentro.**  
> **`margin` separa el elemento desde fuera.**

"Esta pequeña diferencia nos va a acompañar durante prácticamente todo nuestro aprendizaje de CSS."

---

## 🧪 Actividad — Mejora el diseño de tu página

"Ahora vamos a volver a nuestra página."

"Esta vez no vamos a añadir contenido nuevo."

"Vamos a concentrarnos en **mejorar su presentación**."

### Tu página debe utilizar:

- `margin` para separar elementos.
- `padding` para crear espacio interior.
- `border` para añadir al menos un borde.
- `background-color` para crear un fondo.
- `text-align` para cambiar la alineación de algún texto.

"Por ejemplo, puedes empezar con algo como esto:"

```css id="u6p3ra"
body {
    background-color: lightgray;
}

h1 {
    color: purple;
    text-align: center;
    padding: 15px;
    border: 2px solid purple;
}

p {
    margin: 20px;
}
```

"Pero no tienes que copiar exactamente este diseño."

"Prueba diferentes colores, tamaños de espacio y estilos de borde."

"Observa qué ocurre cuando aumentas el `padding`."

"Después prueba aumentando el `margin`."

"Y fíjate en que **no producen el mismo resultado**."

> **Nota visual:** Aprovechar CodePen para modificar los valores en vivo. Probar, por ejemplo, `padding: 5px`, `padding: 30px` y después comparar con `margin: 5px` y `margin: 30px`.

"El objetivo no es conseguir una página perfecta."

"El objetivo es que puedan mirar una regla CSS y entender **qué cambio visual está provocando**."

---

## 🧠 ¿Qué hemos aprendido realmente?

"Puede parecer que hoy solamente hemos aprendido cinco propiedades."

"Pero en realidad hemos aprendido algo más importante."

"Ya podemos controlar diferentes aspectos del espacio y la presentación de nuestros elementos."

"Esto significa que ya podemos pasar de una página que simplemente funciona a una página que empieza a tener una **organización visual propia**."

---

## 🚀 Cierre

"Hoy aprendimos a utilizar CSS no solamente para cambiar colores, sino también para controlar **cómo se distribuye visualmente nuestro contenido**."

"Aprendimos que `margin` crea espacio alrededor de un elemento."

"`padding` crea espacio dentro del elemento."

"`border` añade un borde."

"`background-color` permite cambiar el fondo."

"Y `text-align` nos permite controlar la alineación del texto."

"Con estas propiedades ya podemos conseguir cambios bastante grandes utilizando muy pocas líneas de CSS."

"Y esto es solo el comienzo."

"En la siguiente lección vamos a utilizar todo lo que hemos aprendido hasta ahora para **construir una página web mucho más completa**, combinando estructura HTML y estilos CSS."

**¡Nos vemos en la siguiente lección! 👋**