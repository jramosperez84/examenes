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
