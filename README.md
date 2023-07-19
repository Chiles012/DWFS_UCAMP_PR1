# DWFS_UCAMP_PR1

Primer modulo de DWSF

* [HTML](#HTML)

  * [¿Que es HTML?](#¿Que es HTML?)
  * [Historia](#Historia)
  * [Etiquetas HTML](#Etiqueras HTML)
  * [Etiquetas Semanticas](#Etiquetas Semanticas)
  * [Etiquetas de texto](#Etiquetas de texto)
  * [Etiquetas de contenido](#Etiquetas de contenido)
* [CSS](#CSS)

  * [Selectores](#Selectores)
  * [Variables](#Variables)
  * [Flexbox](#Flexbox)
  * [Grid](#Grid)
  * [Responsive](#Responsive)

# HTML {HTML}

## ¿Que es HTML? {¿Que es HTML?}

HTML, siglas de HyperText Markup Language (Lenguaje de Marcado de Hipertexto), es el lenguaje estándar utilizado para crear y estructurar el contenido de las páginas web. Es el bloque de construcción fundamental de cualquier sitio web y proporciona la estructura y el significado semántico del contenido.

## Historia HTML {#Historia}

1. Años 1980:
   * A medida que Internet comenzaba a tomar forma, surgieron diferentes formatos de documentos electrónicos. No había un estándar común en ese momento.
2. Años 1990:
   * En 1990, Tim Berners-Lee, conocido como el padre de la web, desarrolló el lenguaje HTML (HyperText Markup Language) como una forma de estructurar y formatear documentos para la World Wide Web (WWW).
   * La versión inicial de HTML se basó en el lenguaje SGML (Standard Generalized Markup Language) y permitía la creación de enlaces hipertexto.
3. HTML 2.0:
   * En 1995, se publicó la especificación HTML 2.0 como el primer estándar formal de HTML.
   * Esta versión introdujo características como formularios, tablas y soporte para imágenes.
4. HTML 3.2:
   * En enero de 1997, se publicó la especificación HTML 3.2.
   * HTML 3.2 agregó nuevas características como marcos (frames), estilos incorporados (inline styles) y soporte para scripts en el lado del cliente.
5. HTML 4.01:
   * En diciembre de 1999, se lanzó la especificación HTML 4.01.
   * Esta versión proporcionó mejoras en la estructura del documento y agregó nuevas características como estilos CSS (Cascading Style Sheets) y elementos semánticos como `header`, `footer`, `nav`, entre otros.
6. XHTML:
   * XHTML (Extensible HyperText Markup Language) fue introducido como una versión más estricta y basada en XML de HTML.
   * XHTML combinó la sintaxis de XML con las reglas de HTML y promovió buenas prácticas de codificación y una estructura más precisa del documento.
7. HTML5:
   * HTML5 es la versión más reciente y actualizada de HTML.
   * Lanzada en octubre de 2014, HTML5 introdujo muchas mejoras y nuevas características, incluyendo elementos semánticos (como `article`, `section`, `header`, `footer`), etiquetas de video y audio, almacenamiento local, lienzo (canvas) para gráficos, soporte para aplicaciones web y mucho más.

## Etiquetas HTML {Etiquetas HTML}

Las etiquetas HTML son elementos utilizados para estructurar y dar formato al contenido de una página web.

Toda etiqueta debe tener una etiqueta de inicio y una de cierre dentro de estas debe tener el contenido un ejemplo sería el siguiente: <> apertura, </> cierre

```
<p>Hola mundo!</p>
```

Pero existen etiquetas que no ocupan la etiqueta de cierre esto se puede suplir con la diagonal antes o despues del nombre de la eitqueta

```
</br>
```

Ejemplos comunes de etiquetas incluyen `<div>`, `<p>`, `<h1>` a `<h6>`, `<a>`, `<img>`, `<ul>`, `<li>`, entre otros.

**Los atributos HTML proporcionan información adicional o configuraciones específicas para las etiquetas.**

* Los atributos se agregan a las etiquetas utilizando la sintaxis `nombreAtributo="valor"`.
* Ejemplos de atributos comunes incluyen `class`, `id`, `src`, `href`, `alt`, `style`, entre otros.

`<p class="title">Hola Mundo</p>`

Existen etiquetas indispensables al crear un archivo HTML a continuación se mostrara un ejemplo de un template base de un archivo HTML:

```
<!DOCTYPE html> <!-- Indica el tipo del documento en este caso html, anteriormente era común ver xml o otros formatos por esta razon existe esta etiqueta -->
<html lang="es">
<!-- La etiqueta html indica el inicio del archivo y podemos crear nuestro cotenido debajo de esta etiqueta -->
<!-- El atributo lang indica el idioma en este caso es = español -->
<head> <!-- La etiqueta head se agregan meta-datos, generalmente importaciones ( cdn, estilos, librerias ) y configuracion del proyecto -->
    <meta charset="UTF-8"> <!-- meta = metadatos, el atributo charset es el tipo de formato en este caso UTF-8 que acepta caracteres latinos -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- Configuración de la pantalla -->
    <title> <!-- Titulo -->
        Landing Page | Gym
    </title>
</head>
<body> <!-- body es donde se agregara todo el contenido visual -->
	<!-- ¡Aqui agrega tu contenido! -->
</body>
</html>
```

## Etiquetas Semanticas {Etiquetas Semanticas}

Al utilizar estas etiquetas, le proporcionas un significado claro al contenido y facilitas la comprensión tanto para los desarrolladores como para los motores de búsqueda. Recuerda que el uso adecuado de las etiquetas semánticas mejora la accesibilidad y la experiencia de usuario, además de ser beneficioso para el SEO (Optimización para Motores de Búsqueda).

`<header>`: Se utiliza para representar el encabezado o sección introductoria de un documento o de una sección específica de contenido.

```
<header>
  <h1>Título del sitio web</h1>
  <nav>
    <ul>
      <li><a href="#">Inicio</a></li>
      <li><a href="#">Acerca de</a></li>
      <li><a href="#">Contacto</a></li>
    </ul>
  </nav>
</header>
```

`<nav>`: Se utiliza para representar una sección de navegación, como un menú de navegación principal o enlaces de navegación.

```
<nav>
  <ul>
    <li><a href="#">Inicio</a></li>
    <li><a href="#">Productos</a></li>
    <li><a href="#">Servicios</a></li>
    <li><a href="#">Contacto</a></li>
  </ul>
</nav>
```

`<main>`: Representa el contenido principal de un documento o de una sección específica de contenido.

```
<main>
  <h1>Bienvenido al sitio web</h1>
  <p>Este es el contenido principal del sitio.</p>
</main>

```

`<article>`: Se utiliza para representar un contenido independiente y autónomo que puede ser reutilizable por sí mismo, como una publicación de blog o un artículo de noticias.

```
<article>
  <h2>Título del artículo</h2>
  <p>Contenido del artículo...</p>
</article>

```

`<section>`: Representa una sección temática de contenido dentro de un documento, como secciones de introducción, contenido relacionado o bloques de contenido separados.

```
<section>
  <h2>Sección 1</h2>
  <p>Contenido de la sección 1...</p>
</section>

<section>
  <h2>Sección 2</h2>
  <p>Contenido de la sección 2...</p>
</section>

```

`<footer>`: Se utiliza para representar el pie de página de un documento o de una sección específica de contenido.

```
<footer>
  <p>Derechos de autor © 2023 Sitio web. Todos los derechos reservados.</p>
</footer>

```

Estos son solo algunos ejemplos de etiquetas semánticas en HTML.

## Etiquetas de texto


`<h1>` a `<h6>` (Encabezados):

* Se utilizan para representar diferentes niveles de encabezados o títulos en una página web. `<h1>` es el encabezado principal y `<h6>` es el encabezado de nivel más bajo.
* Ejemplo:

```
<h1>Encabezado principal</h1>
<h2>Encabezado secundario</h2>
<h3>Encabezado terciario</h3>

```

`<p>` (Párrafos):

* Se utiliza para envolver y presentar párrafos de texto.
* Ejemplo:

```
<p>Este es un párrafo de ejemplo.</p>

```


`<strong>` y `<em>` (Énfasis):

* `<strong>` se utiliza para resaltar el texto de forma semántica y darle importancia visualmente.
* `<em>` se utiliza para enfatizar el texto, generalmente se muestra en cursiva por defecto.
* Ejemplo:

```
<p>Este texto es <strong>importante</strong> y este otro es <em>énfasis</em>.</p>

```


`<span>`:

* Se utiliza para aplicar estilos o agregar atributos a partes específicas de un texto dentro de un elemento.
* Por si solo no hace nada.
* Ejemplo:

```
<p>Este es un texto de ejemplo <span style="color: blue;">con una parte resaltada en azul</span>.</p>

```


`<a>` (Enlaces):

* Se utiliza para crear enlaces a otras páginas web o recursos.
* Ejemplo:

```
<p>Visita nuestro <a href="https://www.ejemplo.com">sitio web</a> para obtener más información.</p>

```


`<br>` (Salto de línea):

* Se utiliza para realizar un salto de línea dentro de un párrafo o en lugares donde no se puede utilizar el espaciado entre párrafos.
* Ejemplo:

```
<p>Este es un texto de ejemplo.<br>Y esta es otra línea.</p>

```

Estas son solo algunas de las etiquetas de texto más comunes en HTML.

## Etiquetas de contenido

Las etiquetas de contenido en HTML permiten la incorporación de elementos multimedia en una página web. Aquí tienes una explicación y ejemplos de las etiquetas `<img>`, `<video>` y `<audio>`:


`<img>` (Imágenes):

* La etiqueta `<img>` se utiliza para insertar imágenes en una página web.
* El atributo `src` especifica la URL o la ruta de la imagen que se va a mostrar.
* Ejemplo:

```
<img src="ruta-de-la-imagen.jpg" alt="Descripción de la imagen">

```


`<video>` (Videos):

* La etiqueta `<video>` se utiliza para insertar videos en una página web.
* Puede contener uno o varios formatos de video diferentes para que el navegador elija el que sea compatible.
* Ejemplo:

```
<video src="ruta-del-video.mp4" controls>
  Tu navegador no soporta el elemento de video.
</video>

```


`<audio>` (Audio):

* La etiqueta `<audio>` se utiliza para insertar archivos de audio en una página web.
* Puede contener uno o varios formatos de audio diferentes para que el navegador elija el que sea compatible.
* Ejemplo:

```
<audio src="ruta-del-audio.mp3" controls>
  Tu navegador no soporta el elemento de audio.
</audio>

```

Es importante mencionar que en cada etiqueta se utiliza el atributo `src` para especificar la ubicación del archivo multimedia (imagen, video o audio). Además, el atributo `alt` se utiliza en la etiqueta `<img>` para proporcionar una descripción alternativa de la imagen en caso de que no se pueda mostrar.

Recuerda que al utilizar estas etiquetas de contenido multimedia, debes asegurarte de tener los archivos multimedia en la ruta correcta y en el formato adecuado para garantizar que se muestren correctamente en la página web.

Experimentar con diferentes atributos y opciones (como `controls`, `autoplay`, `loop`, entre otros)

# CSS

CSS (Cascading Style Sheets) es un lenguaje utilizado para definir la apariencia y el diseño de una página web. Su objetivo principal es separar el contenido (HTML) de la presentación (CSS), lo que permite tener un mayor control y flexibilidad sobre la apariencia visual de un sitio web.

CSS es un lenguaje de estilo que describe cómo se deben mostrar los elementos HTML en una página web.

Permite controlar aspectos como el color, el tamaño, el espaciado, la tipografía y la disposición de los elementos.

## Selectores

Selectores de elementos:

* Los selectores de elementos se utilizan para seleccionar elementos HTML basados en su nombre de etiqueta.
* Ejemplo: `p` selecciona todos los elementos de párrafo en la página.

Selectores de clase:

* Los selectores de clase se utilizan para seleccionar elementos HTML que tienen un atributo de clase específico.
* Ejemplo: `.destacado` selecciona todos los elementos con la clase "destacado".
* La clase en un elemento HTML lo encuentras con el atributo class=""

Selectores de ID:

* Los selectores de ID se utilizan para seleccionar elementos HTML que tienen un atributo de ID específico.
* Ejemplo: `#logo` selecciona el elemento con el ID "logo".
* Se usa el atributo id=""

Selectores descendentes:

* Los selectores descendentes se utilizan para seleccionar elementos que son descendientes de otros elementos.
* Ejemplo: `div p` selecciona todos los elementos de párrafo que son descendientes de elementos `<div>`.

Selectores de atributo:

* Los selectores de atributo se utilizan para seleccionar elementos HTML basados en los valores de sus atributos.
* Ejemplo: `a[href="https://www.ejemplo.com"]` selecciona todos los enlaces con el atributo `href` igual a "[https://www.ejemplo.com](https://www.ejemplo.com/)".

Selectores de pseudo-clase:

* Los selectores de pseudo-clase se utilizan para seleccionar elementos en estados o condiciones específicas.
* Ejemplo: `a:hover` selecciona todos los enlaces cuando el cursor está sobre ellos.


## Variables

En CSS, las variables se conocen como "variables personalizadas" o "variables CSS". Se definen utilizando la sintaxis `--nombre-variable` y se asigna un valor después de dos puntos `:`. Por ejemplo:

```
/* Creación de una variable CSS */
:root {
  --color-primario: #007bff;
  --tamanio-fuente: 16px;
}

```

* En el ejemplo anterior, hemos creado dos variables CSS: `--color-primario` y `--tamanio-fuente`.
* El selector `:root` se utiliza para establecer las variables en el nivel más alto del documento, lo que hace que estén disponibles para todo el documento.

Las variables CSS se pueden utilizar en cualquier lugar donde se apliquen valores CSS. Por ejemplo, puedes utilizarlas en las propiedades `color`, `font-size`, `background-color`, entre otras.

```
/* Uso de variables CSS */
body {
  font-size: var(--tamanio-fuente);
}

a {
  color: var(--color-primario);
}

.header {
  background-color: var(--color-primario);
}

```

## Flexbox

Flexbox es un sistema de diseño unidimensional que permite organizar elementos en un contenedor de manera flexible, ya sea en una fila (eje principal horizontal) o en una columna (eje principal vertical). Esto hace que el diseño sea más adaptable y fácil de manejar en diferentes tamaños de pantalla.

#### Propiedades clave de Flexbox:

1. `display: flex;`: Esta propiedad se aplica al contenedor y establece el contenedor como un contenedor flex, para usar flexbox es indispensable usar esta propiedad.
2. `flex-direction: row | row-reverse | column | column-reverse;`: Define la dirección principal en la que los elementos flexibles se muestran dentro del contenedor. Los valores pueden ser "row" (fila), "column" (columna), "row-reverse" (fila en sentido inverso) o "column-reverse" (columna en sentido inverso).
3. `justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;`: Controla la alineación de los elementos a lo largo del eje principal (horizontal si `flex-direction` es "row" y vertical si es "column").
4. `align-items: flex-start | flex-end | center | baseline | stretch;`: Controla la alineación de los elementos a lo largo del eje secundario (vertical si `flex-direction` es "row" y horizontal si es "column").
5. `flex-wrap: nowrap | wrap | wrap-reverse;`: Controla si los elementos flexibles se deben envolver en líneas adicionales o no, cuando el espacio del contenedor es insuficiente. Los valores son "nowrap" (no se envuelve), "wrap" (se envuelve) y "wrap-reverse" (se envuelve en sentido inverso).

## Grid

Grid es un sistema de diseño bidimensional que permite organizar elementos en filas y columnas dentro de un contenedor. Es especialmente útil para crear diseños complejos y alinear elementos en diferentes áreas de la página.

#### Propiedades clave de Grid:

1. `display: grid;`: Esta propiedad se aplica al contenedor y lo convierte en un contenedor de cuadrícula, esta propiedad es indispensable para usar grid.
2. `grid-template-columns` y `grid-template-rows`: Define las columnas y filas de la cuadrícula. Puedes establecer tamaños fijos (`px`, `%`) o utilizar valores flexibles (`fr`, `auto`, etc.).
3. `grid-column` y `grid-row`: Estas propiedades permiten controlar el posicionamiento y el espacio que ocupa un elemento en la cuadrícula.
4. `grid-gap`: Establece el espacio entre filas y columnas en la cuadrícula.
5. `grid-template-areas`: Permite asignar nombres a áreas específicas de la cuadrícula y organizar los elementos utilizando esos nombres.

## ¿Qué es Responsive Web Design?

El Diseño Web Responsivo es un enfoque de diseño y desarrollo web que busca crear sitios web que se adapten y respondan de manera fluida a diferentes tamaños de pantalla y dispositivos, como computadoras de escritorio, tablets y smartphones. El objetivo es proporcionar una experiencia óptima para los usuarios, independientemente del dispositivo que estén utilizando, evitando la necesidad de crear versiones separadas para cada tipo de dispositivo.

### Cómo lograr Responsive Web Design con CSS:

1. **Unidades flexibles y fluidas** : Utiliza unidades relativas como porcentajes (`%`), em (`em`) o viewport width (`vw`) para definir anchos, alturas y márgenes. Esto permitirá que los elementos se ajusten proporcionalmente al tamaño de la pantalla.
2. **Media Queries** : Las Media Queries son una característica clave de CSS que permite aplicar estilos específicos a diferentes rangos de tamaño de pantalla. Se definen utilizando la regla `@media` y se pueden aplicar diferentes estilos según la resolución, el ancho o el tipo de dispositivo.

```
/* Ejemplo de Media Query para pantallas más pequeñas */
@media screen and (max-width: 768px) {
  /* Estilos aplicados a pantallas de 768px o menos */
  body {
    font-size: 14px;
  }
}

/* Ejemplo de Media Query para pantallas grandes */
@media screen and (min-width: 1200px) {
  /* Estilos aplicados a pantallas de 1200px o más */
  body {
    font-size: 18px;
  }
}

```

1. **Imágenes y multimedia adaptables** : Utiliza imágenes con atributos `max-width: 100%; height: auto;` para que se ajusten al ancho del contenedor y no se desborden en pantallas pequeñas.
2. **Layout flexible con Flexbox y Grid** : Utiliza Flexbox y Grid para crear diseños flexibles y adaptables que se ajusten automáticamente a diferentes tamaños de pantalla.
3. **Menús y navegación adaptable** : Crea menús y barras de navegación que se contraigan en un menú desplegable para pantallas más pequeñas, utilizando técnicas como "hamburguesa" o "toggle".
4. **Testing en diferentes dispositivos** : Siempre prueba el sitio en diferentes dispositivos reales o utilizando herramientas de desarrollo web que permitan simular diferentes tamaños de pantalla.
