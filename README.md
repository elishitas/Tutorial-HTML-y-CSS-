### Introducción

HTML, o HyperText Markup Language, es el "esqueleto" de la web. CSS 'viste' el HTML y JavaScript le da vida, HTML es el cuerpo de la aplicación web. La sintaxis de HTML incluso refleja esa idea, ya que incluye etiquetas "head", "body" y "footer".

Vamos a usar HTML para diseñar el 'esqueleto' de la interfaz de nuestra página. La interfaz se va a ver un poco extraña; no te preocupes! En la siguiente clase agregamos estilos CSS a la interfaz para que se vea mejor.

### Elementos Básicos de HTML

HTML define una serie de elementos (o etiquetas, o tags) que serviran para delimitar texto, nosotras lo vamos a llamar Tag, cada tag está encerrado en   `< >` y tiene un nombre. Los tags se abren y se cierran, los tags de cuando se cierran incluyen un "/". Por ejemplo:

 `<element>
    ...
 </element>
 `
Algunos tags html no necesitan tener nada adentro. Por lo tanto podemos abreviar su escritura y en vez de abrir y cerrar el tag, simplemente agregamos un `/` antes del `>`

En pocas palabras ¿qué estamos mirando aquí? Que un HTML consta de estas boquitas que abren y cierran.

Por ejemplo, `<html>` es un tag y la tag de cierre para ella es `</html>`, lo mismo con `<head>` y `</head>`, `<body>` y `</body>` y así sucesivamente

Las etiquetas o tag organizan nuestra página y le dicen al navegador en qué consiste la misma. Hay toneladas de tags, algunas que quizás nunca uses.
Aquí hay algunas listas de tags :

[Lista de etiquetas en W3school](https://www.w3schools.com/tags/default.asp)

[Otra lista de etiquetas de HTML](https://www.quackit.com/html/tags/)

[Una hermosa Tabla Periodica de Etiquetas!](http://mialtoweb.es/webs/tabla/#style)

## Las tags DocType y html

La primera línea de un archivo HTML es su doctype. Es un poco sorprendente que necesite tener esta línea en la parte superior del archivo, pero le dice a los navegadores más antiguos que el navegador necesita representar una página HTML entonces cada documento HTML y sitio web debe tener esta etiqueta especial, ya que le dice al navegador qué idioma estamos usando. Esta es una de esas etiquetas especiales que mencionamos que no necesita una etiqueta de cierre.

## Head
Este tag sirve para contener tags que contengan información sobre el documento, pero es información que no queremos que se vea en nuestro body. Comunmente contiene el titulo de la página y links a recursos externos que pueda usar la página (javascript o css), metadatos, etc

## Title
Es el título de la página, se mostrará en el tab del browser o en la parte superior (pero no en la página).

## Body
En este tag estára encerrado todo lo que querramos que se vea en la pantalla.

Entonces, hasta ahora, un documento HTML se ve así:

```
<!DOCTYPE html>
<html>

 <head>
     <title>
         My Website
     </title>
</head>

<body>
    Hello, World!
</body>

</html> 
```

Para mayor fácilidad en la lectura y la estructuración del documento el documento HTML se escribe indentando (o usando sangría) ¿Qué es [indentar](https://es.wikipedia.org/wiki/Indentaci%C3%B3n)?

-Todos los tags que presentamos más abajo van siempre adentro del body-

## h1 a h6 
Son los tags de encabezado o títulos, están pensandos del 1 al 6, para indicar la importancia del contenido y su jerarquía.

```
 <h1>  El título más importante </h1>
 
 <h3> El título medianamente importante.</h3>
 
 <h6>El título menos importante.</h6>
```

## p
Es el tag para los párrafos. Mostrará el texto contenido dentro en una nueva línea.
  `<p>Soy un párrafo</p>`  
  
## span
El elemento span es un contenedor de texto genérico. No inserta una nueva linea, como lo hace el elemento p. Sirve básicamente para darle estilo al texto.

## div
El elemento div es un contenedor genérico. Es usado principalmente para dar estilo, imaginen que es una caja (cuyo tamaño y color podes modificar a piacere), y que dentro podés poner otras cajas iguales.

## a
El tag a (del inglés anchor), nos permite crear links a otros documentos y páginas. Este tag recibe el atributo href que indica a dónde apunta el link.

  `<a href="http://www.chicasprogramadoras.club/!</a>` 

## img
Este tag nos permite mostrar imágenes en la pantalla. Necesita el atributo src que indica la URL de donde sacar la imagen a mostrar.

```
  <img src="http://www.chicasprogramadoras.club/wp-content/uploads/2016/09/cropped-cropped-logo-chicas-1.png" />
```
  
## ul
Este tag representa una lista desordenada (del inglés unordered list). Etá diseñado para contener otros tags de tipo item. También existe el tag ol que reprensentan las listas en HTML ordenadas.

## li
Son los tags que contienen los items de la lista ('list item').

```
<ul>
    <li>
      <span>Elemento uno</span>
    </li>
    <li>
      <p>Podemos anidar cualquier tipo de tag adentro</p>
    </li>
    <li>
      <span>tercer elemento</span>
    </li>
</ul>
```
# ¡Recapitulamos!
A modo de resumen vamos a escribir las etiquetas que estuvimos usando:

- Tag Nombre del elemento (ejemplo `a`)
- Atributo Modificadores de HTML (ejemplo `href`)
- Valor Valor aplicado a un atributo (ejemplo `http:/clubdechicas.dev`)
- Elemento Todo lo que se encuentra dentro de la etiqueta HTML: atributos, valores y contenido
