# 🎓 Guión — Lección 4: Introducción a CSS

---

## 🎬 Introducción — Nuestra página está a punto de cambiar

> "Hasta ahora hemos dedicado nuestras primeras lecciones a construir la estructura de nuestra página."

"Ya sabemos utilizar HTML para crear títulos, párrafos, listas, imágenes y enlaces."

"Pero si hemos estado trabajando en CodePen, probablemente hayan notado algo."

"**Nuestra página funciona... pero no se ve especialmente interesante.**"

"Tenemos nuestro contenido, pero el navegador decide prácticamente toda la apariencia."

"Los títulos tienen un tamaño determinado, los textos tienen un color determinado y todo aparece con un estilo bastante básico."

"Entonces aparece nuestra segunda herramienta:

**CSS.**"

"En la primera lección dijimos que HTML se encarga de la estructura y CSS de la apariencia."

"Hoy vamos a comprobarlo directamente."

"Vamos a tomar la página que ya construimos y vamos a empezar a cambiar cómo se ve."

---

## 🎨 ¿Qué es CSS?

"CSS significa **Cascading Style Sheets**, o **Hojas de Estilo en Cascada**."

"Su función principal es definir **cómo queremos que se vea el contenido de nuestra página HTML**."

"Con CSS podemos modificar, entre muchas otras cosas:"

- colores,
- tamaños de texto,
- tipos de letra,
- fondos,
- espacios,
- bordes,
- posiciones y distribución de elementos.

"Por ejemplo, podemos tener este título en HTML:"

```html
<h1>Mi página web</h1>
```

"HTML nos está diciendo algo importante:

**Esto es un encabezado principal.**"

"Pero HTML no necesita decidir exactamente qué color queremos utilizar."

"Podemos dejar esa decisión a CSS."

"Por ejemplo:"

```css
h1 {
    color: purple;
}
```

"Ahora el navegador sabe que queremos que los elementos `h1` tengan el color púrpura."

> **Nota visual:** En CodePen, mostrar primero el HTML sin CSS y después añadir la regla CSS. El cambio debe ser visible inmediatamente.

"Y aquí aparece una idea fundamental."

> **HTML describe el contenido.  
> CSS define cómo se presenta.**

---

## 🧩 La estructura de una regla CSS

"Ahora vamos a mirar con atención la regla que acabamos de escribir."

```css
h1 {
    color: purple;
}
```

"Aquí tenemos tres partes importantes."

"Primero tenemos:"

```css
h1
```

"Esto se llama **selector**."

"El selector indica **qué elemento HTML queremos modificar**."

"Después tenemos:"

```css
color
```

"Esto se llama **propiedad**."

"La propiedad indica **qué característica queremos cambiar**."

"Y finalmente tenemos:"

```css
purple
```

"Esto es el **valor**."

"El valor indica **qué queremos aplicar a esa propiedad**."

"Podemos verlo así:"

```text
h1       → selector
color    → propiedad
purple   → valor
```

"Todo esto forma una **regla CSS**."

"Y hay algo importante en la forma de escribirla."

"Después del selector abrimos unas llaves:"

```css
h1 {
    
}
```

"Dentro de esas llaves colocamos las propiedades y sus valores."

"Una propiedad se escribe seguida de dos puntos `:` y después colocamos su valor."

```css
color: purple;
```

"Finalmente utilizamos un punto y coma `;` para indicar que esa declaración termina."

"Por ahora no necesitamos memorizar todos los detalles de la sintaxis."

"Lo importante es entender esta estructura:"

```text
selector {
    propiedad: valor;
}
```

> **Esta es la estructura básica que vamos a repetir muchísimo cuando escribamos CSS.**

---

## 🎯 Nuestro primer selector

"Vamos a utilizar nuestro HTML de la lección anterior."

```html
<h1>Mis intereses</h1>

<p>
    Estas son algunas cosas que me gustan.
</p>
```

"Si queremos cambiar el color del título, podemos seleccionar todos los elementos `h1`:"

```css
h1 {
    color: purple;
}
```

"Y si queremos cambiar los párrafos:"

```css
p {
    color: darkblue;
}
```

"El selector `h1` selecciona los encabezados `h1`."

"El selector `p` selecciona los párrafos."

"Por eso podemos pensar en los selectores como una forma de decirle a CSS:

**'Quiero trabajar con estos elementos.'**"

---

## 🌈 Cambiando colores

"Una de las cosas más sencillas que podemos hacer con CSS es cambiar colores."

"Ya vimos la propiedad `color`."

```css
h1 {
    color: purple;
}
```

"También podemos cambiar el color de fondo utilizando otra propiedad:"

```css
body {
    background-color: lightgray;
}
```

"Aquí estamos haciendo algo diferente."

"El selector es `body`, así que estamos seleccionando el cuerpo completo de nuestra página."

"La propiedad es `background-color`."

"Y el valor es `lightgray`."

"Podemos combinar ambas reglas:"

```css
body {
    background-color: lightgray;
}

h1 {
    color: purple;
}
```

"Ahora tenemos una página cuyo fondo y título tienen una apariencia diferente."

> **Nota visual:** Cambiar primero solamente `background-color`, después solamente `color`, y finalmente mostrar ambas reglas juntas.

---

## 🔤 Cambiando el tamaño del texto

"Los colores son solo una parte de lo que podemos modificar."

"También podemos cambiar el tamaño del texto utilizando `font-size`."

```css
h1 {
    font-size: 40px;
}
```

"En este caso, `40px` indica el tamaño que queremos utilizar."

"También podemos cambiar el tamaño de los párrafos:"

```css
p {
    font-size: 18px;
}
```

"Ahora tenemos tres propiedades diferentes que ya podemos reconocer:"

```text
color
background-color
font-size
```

"Y todas funcionan siguiendo exactamente la misma estructura."

```css
selector {
    propiedad: valor;
}
```

"Esto es importante porque CSS tiene muchísimas propiedades."

"No necesitamos aprenderlas todas de memoria."

"Lo que necesitamos aprender primero es **cómo funcionan las reglas**."

---

## 🧠 Una regla puede tener varias propiedades

"Hay otra cosa muy útil que podemos hacer."

"Un mismo selector puede tener varias propiedades."

"Por ejemplo:"

```css
h1 {
    color: purple;
    font-size: 40px;
}
```

"En este caso seguimos seleccionando los elementos `h1`, pero ahora estamos modificando dos características."

"El color será púrpura."

"Y el tamaño será de 40 píxeles."

"También podemos hacer algo parecido con el cuerpo de nuestra página:"

```css
body {
    background-color: lightgray;
    color: darkblue;
}
```

"Ahora todas las propiedades que coloquemos dentro de las llaves forman parte de la misma regla para `body`."

"Podemos añadir más propiedades cuando las necesitemos."

"Pero cada una debe tener su propia declaración."

```css
selector {
    propiedad: valor;
    propiedad: valor;
}
```

---

## 🔗 ¿Cómo trabajan HTML y CSS juntos?

"Ahora podemos conectar todo lo que hemos aprendido."

"Tenemos nuestro HTML:"

```html
<h1>Mis intereses</h1>

<p>Me gusta aprender desarrollo web.</p>
```

"Y tenemos nuestro CSS:"

```css
h1 {
    color: purple;
    font-size: 40px;
}

p {
    color: darkblue;
}
```

"HTML creó los elementos."

"CSS modificó su apariencia."

"Podemos volver a nuestra comparación de la casa."

> **HTML construye y organiza la casa.  
> CSS decide cómo se ve.**

"Si cambiamos el HTML, estamos cambiando la estructura o el contenido."

"Si cambiamos el CSS, podemos cambiar la apariencia sin tener que reescribir todo nuestro contenido."

"Y esta separación será muy importante cuando nuestras páginas empiecen a crecer."

---

## 🧪 Actividad — Dale estilo a tu página

"Ahora vamos a volver a la página que construimos en la lección anterior."

"Esta vez vamos a utilizar **HTML y CSS juntos**."

"En CodePen tenemos dos áreas principales que vamos a utilizar."

```text
HTML → estructura y contenido

CSS → apariencia
```

"En la sección HTML coloca o utiliza tu página anterior."

"Después vamos a escribir nuestras primeras reglas CSS."

### Tu página debe incluir como mínimo:

- Un color para el título principal.
- Un tamaño diferente para el título.
- Un color para los párrafos.
- Un color de fondo para la página.

"Puedes experimentar con diferentes valores."

"Por ejemplo:"

```css
h1 {
    color: blue;
    font-size: 40px;
}

p {
    color: darkgreen;
}

body {
    background-color: lightgray;
}
```

"Pero no tienen que utilizar exactamente estos colores."

"Prueben diferentes valores y observen qué ocurre."

"Lo importante es que puedan identificar las tres partes de cada regla:"

```text
¿A quién estamos modificando?
        ↓
    selector

¿Qué característica cambiamos?
        ↓
     propiedad

¿Qué valor queremos utilizar?
        ↓
       valor
```

"Y si algo no funciona, no borren todo inmediatamente."

"Primero revisen si escribieron correctamente el selector, la propiedad, los dos puntos, el valor y el punto y coma."

"Los errores pequeños son completamente normales cuando estamos aprendiendo a escribir código."

---

## 🔍 Una última idea: CSS no cambia el contenido

"Antes de terminar, quiero que nos quedemos con una diferencia muy importante."

"Imaginemos que tenemos:"

```html
<h1>Mi videojuego favorito</h1>
```

"Y aplicamos:"

```css
h1 {
    color: red;
    font-size: 50px;
}
```

"El texto sigue diciendo exactamente lo mismo."

"CSS no cambió el contenido."

"Lo que cambió fue **cómo se presenta ese contenido**."

"Esta separación entre contenido y presentación es una de las ideas fundamentales del desarrollo web."

> **HTML → qué es y qué contiene.  
> CSS → cómo se ve.**

"Y cuanto más grande sea nuestra página, más útil será tener estas responsabilidades separadas."

---

## 🚀 Cierre

"Hoy hemos dado un paso importante."

"Ya no solamente podemos construir una página con HTML."

"Ahora podemos empezar a controlar su apariencia utilizando CSS."

"Aprendimos que una regla CSS tiene esta estructura:"

```css
selector {
    propiedad: valor;
}
```

"El **selector** indica qué elementos queremos modificar."

"La **propiedad** indica qué característica queremos cambiar."

"Y el **valor** indica qué queremos aplicar."

"También vimos que podemos utilizar varias propiedades dentro de una misma regla."

"En la siguiente lección vamos a aprovechar estas bases para trabajar con **más estilos y comenzar a construir un diseño mucho más completo**."

**¡Nos vemos en la siguiente lección! 👋**