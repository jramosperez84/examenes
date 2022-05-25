# Guia de estudio Lenguaje de marcas

## UF1

---

### Principales lenguajes de marcas

#### **XML**

*Fue diseñado para almacenar y transportar datos, además de usarse en
servicios web.*

#### **HTML**

*Se utiliza para estructurar y desplegar una página web y sus contenidos.*

#### **CSS**

*Se utiliza para controlar el aspecto de los documentos escritos en html o xhtml.*

#### **XHTML**

*Su propósito era reemplazar a html. Es una forma de html definida como una
aplicación xml.*

---

### Diferencias en html y xhtml

Las diferencias que existen son basicamente sintacticas. La sintaxis de HTML está inspirada en SGML (Standard Generalized Markup Languaje)
Por su parte XHTML esta basada en recomendación XML

---

### Utilidad de XML

- Para la definición de archivos de configuración.
- Para protocolos de comunicación.
- Intercambio de datos entre sistemas.
- Para su uso en bases de datos.
- Como medio conversor entre distintos formatos, PDF, HTML, docx, XHTML.
- Para compartir grandes volúmenes de datos.

---

### Estructura de un HTML

~~~html
<!-- ESTO ES UN HTML 5 -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>TITULO</title>
</head>
<body>
    
</body>
</html>
~~~

---

### Elementos en linea y elementos en bloque

Los elementos en línea son aquellos que se encuentran en una misma línea. Si
colocamos varios elementos de este tipo seguidos se colocarán en la misma línea, a
menos que indiquemos lo contrario con un salto de línea.
Algunos ejemplos son:

~~~html
<span>, <code>, <img>, <input>
~~~

Los elementos en bloque no necesitan de saltos de línea ya que cada vez que se
utilizan lo realizan de forma predeterminada. Por ejemplo, si colocamos un...

~~~html
<p>texto</p><p>seguido de texto</p> 
~~~

aunque estén en línea dentro del código se
mostraran uno debajo del otro.
Algunos ejemplos son...

~~~html
<div>, <p>, <h1>, <table>
~~~

---

### Estructura de una lista en HTML

~~~html
<ul>
    <caption>Listas con elementos</caption> <!--Titulo de una lista-->
    <li>Primero</li>
    <li>Segundo</li>
    <li>Tercero</li>
    <li>Cuarto</li>
</ul>
<ul>
    <caption>Listas con sublistas</caption>
    <li>Primero</li>
    <ul>
        <li>1.1</li>
        <li>1.2</li>
        <li>1.3</li>
    </ul>
    <li>Segundo</li>
    <li>Tercero</li>
    <li>Cuarto</li>
</ul>
~~~

---

### Enlaces

~~~html
<body>
    <ul>
        <caption>Lista con enlaces web internos y
    externos</caption>
        <li>
            <a href="http://www.google.es">Link a web externa
            (Google)</a>
        </li>
        <li>
            <a href="listas.html">Enlace a web interna (Ejercicio
            listas.html)</a>
        </li>
        <li>
            <a href="http://duckduckgo.com">Enlace a web externa
            (Duckduckgo)</a>
        </li>
        <li>
            <a href="Proyecto3\index.html">Enlace a web interna
            (Proyecto3)</a>
        </li>
    </ul>
</body>
~~~

---

### Insertar a imagenes

~~~html
<body>
    <a href="https://www.ifp.es/">
        <img src="ifp.png" alt="logo ifp">
    </a>
</body>
~~~

---

### Esqueleto de un HTML

~~~html
<!DOCTYPE html>

<html lang="es">
    
    <head>

        <meta charset="UTF-8">
        <title>Document</title>
    
    </head>

    <body>

        <header><h1>Página web de IFP</h1></header>
    
        <nav>
            <a href="m1.html">IR SECCIÓN 1</a>
            <a href="m2.html">IR SECCIÓN 2</a>
        </nav>
        
        <article>
            <h1>CONTENIDO PRINCIPAL</h1>
            11
            <p>Este es el contenido principal de mi web</p>
        </article>
        
        <aside>
            <h3>Banner de publicidad</h3>
            <a href=""><img width="200px" src="images.png"
            alt=""></a>
            <h3>Testimonios</h3>
            <p>Me gusta mucho esta página.</p>
        </aside>
        
        <footer>
            <p><b>Avisos legales</b></p>
            <a href="">Política de cookies</a>
        </footer>

    </body>

</html>
~~~

---

### Estructura de una tabla

~~~html
<table>
    <thead>
        <caption><h3>Titulo</h3></caption>
        <tr>
            <th>texto</th>
            <th>texto</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>texto</td>
            <td>texto</td>
            <td>texto</td>
        </tr>
    </tbody>
</table>
~~~

---

### CSS

Hoja de estilo en cascada...

Referencia

~~~html
<link rel="stylesheet" href="style.css">
~~~

Sintaxis

~~~css
/* Table hace referencia a una tabla de html <table>  */
table {
    border: 3px solid green;
}
/* td hace referencia a la estructura de la tabla en html */
td {
    text-align: center;
    width: 250px;
    height: 150px;
}

/* Como declarar una clase en css: Primero añadimos el codigo a html
    <td class="black"></td>
y la declaracion en html seria la siguiente:
*/

.black {
    text-align: center;
}

~~~

---

### Estructura de un XML

~~~xml
<?xml version="1.0" encoding="UTF-8"?>

<personas>

<nombre>Pedro</nombre>
<edad>46</edad>
<ocupacion>Arquitecto</ocupacion>
<aficiones>Fútbol</aficiones>

<nombre>Juan</nombre>
<edad>27</edad>
<ocupacion>Carpintero</ocupacion>
<aficiones>Natación</aficiones>

<nombre>Jorge</nombre>
<edad>39</edad>
<ocupacion>Programador</ocupacion>
<aficiones>Robótica</aficiones>

</personas>
~~~

---

## UF2

### Sintaxis de XML, normas sintacticas

La sintaxis de un documento XML es muy sencilla, ya que se basa en un docu-
mento de texto ASCII, una cabecera y un conjunto extendido de etiquetas. Sólo
hay que tener en cuenta una serie de reglas sintácticas a la hora de escribir archivos en XML. Veamos cuáles son:

- Todos los elementos XML deben tener una etiqueta de cierre.
- El XML distingue entre mayúsculas y minúsculas.
- Los elementos XML tienen que estar correctamente anidados.
- Los documentos XML deben tener siempre un único elemento raíz.
- Los atributos XML deben ir entre comillas, simples o dobles.
- Existen caracteres especiales que tienen un determinado significado para el XML. Por ejemplo, el carácter < puede confundirse con el principio de una etiqueta. Para
evitarlo se usan entidades de referencia (más adelante veremos cómo crearlas).
- La sintaxis para escribir un comentario dentro de un archivo XML es igual que en
HTML (entre los signos \<!-- Comentario -->).

#### Reglas sobre las etiquetas

- Pueden contener letras, números y otros caracteres.
- No pueden empezar con un número o un carácter de puntuación.
- No pueden empezar con las letras xml (o XML, Xml, etc.); excepto esta salvedad, puede usarse cualquier palabra.
- No pueden contener espacios.
- Pueden escribirse etiquetas sin contenido, pero hay que cerrarla.

~~~xml
<etiqueta> </etiqueta>
~~~

#### Consejos de nomenclatura

En XML, los elementos, atributos, etc., tienen nombre, el cual debe cumplir estas
reglas: en XML se distingue entre mayúsculas y minúsculas, por lo que hay que
tener cuidado al utilizar el nombre desde otro punto del documento. Éste debe
comenzar, además, por una letra, a la que después le seguirán más letras, números o el signo de subrayado o guión bajo. Veamos algunos consejos básicos a la hora de
escribir los nombres de las etiquetas:

- Utilizar nombres descriptivos, cortos y simples.
- Sustituir los espacios por el guión bajo.
- No usar los caracteres - . :
- Los documentos XML suelen tener su correspondencia en una base de datos,
por lo que conviene utilizar las reglas de nomenclatura de la base de datos del documento.
- Los caracteres no ingleses son legales en XML, pero pueden tener problemas de compatibilidad.

---

### Bloques de texto no analizados por XML

~~~xml
<![CDATA[
    <a href="https://mireceta.com/receta1">Mi receta</a>
]]>
~~~

Las entidades predefinidas tales como &lt;, &gt;, y &amp; requieren escribir y, por lo general, son difíciles de leer en el markup. En tales casos, sección CDATA se puede utilizar. Mediante sección CDATA, se ordena el analizador que una sección en particular de el documento no contiene marcado y debe ser tratado como texto normal.

~~~xml
&lt;, &gt;, y &amp;
~~~

### Sindicación (RSS)

#### Estrucctura de un RSS

~~~xml
<?xml version="1.0" encoding="UTF-8" ?>
<rss version="2.0">
    <channel>
        <title>Spoilers</title>
        <link>http://www.decine.es</link>
        <description>Las mejores RSS sobre cine</description>
        <item>
            <title>Cinemania</title>
            <link>https://www.20minutos.es/cinemania/</link>
            <description>Cine, series, críticas y mucho más</description>
        </item>
        <item>
            <title>Estrenos de cine</title>
            <link>https://www.sensacine.com/peliculas/estrenos/es/</link>
            <description>Estrenos de la semana. Encuentra aquí cada viernes los estrenos en cines.
            Películas más esperadas Estrenos de cine por mes Próximos estrenos EEUU.</description>
        </item>
        <item>
            <title>Espinof</title>
            <link>https://www.espinof.com/</link>
            <description>Espinof, últimas noticias de cine, televisión y series</description>
        </item>
    </channel>
</rss>
~~~

### Añadir CSS a un XML

~~~xml
<?xml-stylesheet href="style.css" ?>
~~~

~~~css
nombre {
    color: blue;
    font-weight: bold;
    font-size: larger;
}
ingredientes {
    color: greenyellow;
    display: list-item;
    margin-left: 20px;
}
preparacion {
    font-weight: bolder;
    color: crimson;
}

~~~

---

### ¿Que es un DTD?

Un documento DTD (Definición de Tipo de Documento) establece las reglas de formación del len-
guaje formal, es decir, qué combinaciones de símbolos elementales son sintácticamente correctas
en un documento XML.

#### DTD interno

Un DTD se denomina DTD interno cuando los elementos se han declarado dentro del archivo XML. Para referenciarlo como DTD interno, el atributo standalone en la declaración XML se debe marcar con un Si. Esto significa que la declaración funciona al margen de la fuente externa.

~~~xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE coches [
<!ELEMENT coches (coches+)>
<!ELEMENT coches (matricula, marca, modelo, hibrido?)>
<!ELEMENT matricula (#PCDATA)>
<!ELEMENT modelo (#PCDATA)>
<!ELEMENT hibrido EMPTY>
]>
<coches>
<matricula>1234ABC</matricula>
<marca>Toyota</marca>
<modelo>Prius</modelo>
<hibrido/>
</coches>
~~~

#### DTD externo

En los DTD externos, los elementos se declaran fuera del archivo XML. Se puede acceder a ellos especificando los atributos del sistema que pueden ser o un archivo legal .dtd o una dirección URL válida. Para referenciarlo como DTD externo, el atributo standalone en la declaración XML se debe marcar con un no. Esto significa, que la declaración incluye información de una fuente externa.

~~~xml
archivo_dtd

<!ELEMENT alumno (nombre, apellidos, dirección, edad)>
<!ELEMENT nombre (#PCDATA)>
<!ELEMENT apellidos (#PCDATA)>
<!ELEMENT direccion(#PCDATA)>
<!ELEMENT edad (#PCDATA)>

archivo_xml

<?xml version="1.0" encoding="UTF-8" standalone="no" ?>
<!DOCTYPE address SYSTEM "archivo.dtd">

...
~~~

---

### XML Schema

Es una recomendación desarrollada por W3C, permite definir la estructura y contenido de un
documento XML. Es mucho más potente y versátil que DTD, además de ser más complicado.
Tiene un tipado fuerte, con tipos de datos similares a los lenguajes de programación y bases
de datos, el usuario puede definir tipos de datos a partir de los existentes.
Tiene características de orientación a objetos y cardinalidad precisa.
XML schema es un documento XML por lo que no hay que aprender otra sintaxis. Permite
representación de claves primarias y ajenas.
El uso de XML schema se recomienda a la hora de manejar ficheros XML de gran tamaño y
mas complejos.
