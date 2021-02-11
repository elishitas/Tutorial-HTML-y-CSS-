### Introducción

HTML, o HyperText Markup Language, es el "esqueleto" de la web. CSS 'viste' el HTML y JavaScript le da vida, HTML es el cuerpo de la aplicación web. La sintaxis de HTML incluso refleja esa idea, ya que incluye etiquetas "head", "body" y "footer".

Vamos a usar HTML para diseñar el 'esqueleto' de la interfaz de nuestra página. La interfaz se va a ver un poco extraña; no te preocupes! En la siguiente clase agregamos estilos CSS a la interfaz para que se vea mejor.

### Elementos Básicos de HTML

HTML define una serie de elementos (o etiquetas, o tags) que serviran para delimitar texto, nosotras lo vamos a llamar Tag, cada tag está encerrado en   `< >` y tiene un nombre. Los tags se abren y se cierran, los tags de cerrado incluyen con un "/". Por ejemplo:

 `<element>
    ...
 </element>
 `
Algunos tags html no necesitan tener nada adentro. Por lo tanto podemos abreviar su escritura y en vez de abrir y cerrar el tag, simplemente agregamos un `/` antes del `>`

En pocas palabras ¿qué estamos mirando aquí? Un HTML consta de estas cosas llamadas tag

Por ejemplo, <html> es una etiqueta y la etiqueta de cierre para ella es </html>, lo mismo con <head>y </head>y <body>y </body>, y así sucesivamente

Las etiquetas o tag organizan tu página y le dicen al navegador en qué consiste su página. Hay toneladas de tags, algunas que quizás nunca uses.
Aquí hay algunas listas de tags si realmente te interesa verlas todas en este momento:

[Lista de etiquetas en W3school](https://www.w3schools.com/tags/default.asp)

[Otra lista de etiquetas de HTML](https://www.quackit.com/html/tags/)

[Una hermosa Tabla Periodica de Etiquetas!](http://mialtoweb.es/webs/tabla/#style)

## Las tags DocType y html

La primera línea de un archivo HTML es su doctype. Es un poco sorprendente que necesite tener esta línea en la parte superior del archivo, pero le dice a los navegadores más antiguos que el navegador necesita representar una página HTML entonces cada documento HTML y sitio web debe tener esta etiqueta especial, ya que le dice al navegador qué idioma estamos usando. Esta es una de esas etiquetas especiales que mencionamos que no necesita una etiqueta de cierre.
