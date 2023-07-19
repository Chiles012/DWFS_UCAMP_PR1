# DWFS_UCAMP_PR1

# HTML

## ¿Que es HTML?

HTML, siglas de HyperText Markup Language (Lenguaje de Marcado de Hipertexto), es el lenguaje estándar utilizado para crear y estructurar el contenido de las páginas web. Es el bloque de construcción fundamental de cualquier sitio web y proporciona la estructura y el significado semántico del contenido.

## Historia HTML

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

## Etiquetas HTML

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

## Etiquetas Semanticas

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
