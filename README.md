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
Es el tag para los párrafos: 

  `<p>Soy un párrafo</p>`  
  
## span
El elemento span es un contenedor de texto genérico. No inserta una nueva linea, como lo hace el elemento p. Sirve básicamente para darle estilo al texto.

## div
El elemento div es un contenedor genérico. Es usado principalmente para dar estilo, imaginen que es una caja (cuyo tamaño y color podes modificar a piacere), y que dentro podés poner otras cajas iguales.

## a
El tag a (del inglés anchor), nos permite crear links a otros documentos y páginas. Este tag recibe el atributo href que indica a dónde apunta el link.

  `<a href="http://www.chicasprogramadoras.club>Visita el Club de Chicas Programadoras!</a>` 

## img
Este tag nos permite mostrar imágenes en la pantalla. Necesita el atributo src que indica la URL de donde sacar la imagen a mostrar.

```
  <img src="http://www.chicasprogramadoras.club/wp-content/uploads/2016/09/cropped-cropped-logo-chicas-1.png" />
```
  
## li
El tag `li` define un elemento de la lista. Se usa dentro de listas ordenadas `ol`y en las listas desordenadas `ul` 

## ol y ul
Una lista HTML ordenada `ol` y una desordenada `ul`

![1](https://i.imgur.com/MJREDHQ.png)

## ¡Recapitulamos!
A modo de resumen vamos a escribir las etiquetas que estuvimos usando:

- Tag: Nombre del elemento (ejemplo `a`)
- Atributo: Modificadores de HTML (ejemplo `href`)
- Valor: Valor aplicado a un atributo (ejemplo `http:/clubdechicas.dev`)
- Elemento: Todo lo que se encuentra dentro de la etiqueta HTML: atributos, valores y contenido

Ejemplo
 `tag attibute=""
``` <tag attribute="value">element contents</tag>```

# Fundamentos de CSS
Vamos a repasar algunos conceptos básicos de CSS: Sintasis, selectores y especificidad

## Sintaxis CSS

Hay 3 partes principales de CSS: selectores, propiedades y valores

- **Selectores**: los elementos que estan seleccionados
- **Propiedades**: el aspecto que se está diseñando
- **Valores**: el estilo que se aplica

![1](https://i.imgur.com/iZVjCec.png)

Esto hará que todos los `h1` tag sean azules

# CSS Selectores

Desde el **menos especifico** al **más específico** (lo vemos más adelante) estos son los principales selectores:

- **Selector Universal**: Seleccional todos los los elementos
- **Selector de Tipo**: Apunta a los elementos por etiquetas de HTML (inclute **pseudo elementos**)
- **Selector de clases**, **Selector de atributos**: Elementos de destino por clase o atributo (incluye **pseudo elementos** )
- **Selector ID**: Apunta a un elemento po ID

![1](https://i.imgur.com/rjtwoGL.png)

Los **pseudo elementos** tienen dos dos puntos (`::`, o `::before`) y las **pseudo clases** tiene un solo dos puntos (`:`, o `:hover`)

## Propiedades CSS

Aquí hay una lista de la mayoría de las propiedades que creo que son esenciales para conocer CSS

El mínimo para poder hacer cualquier cosa:

- `padding`, `margin`, `border`
- `background`
- `color`, `font-family`, `font-weight`, `font-size`, `line-height`
- `width`, `height`, `max-width`, `max-height`

Conceptos básicos de diseño:

- `position`, `z-index`, `top`, `right`, `bottom`, `left`
- `display`, `flex`, `align-items`, `justify-content`
- `@media`

Es bueno saberlo:
- `grid`
- `transform`, `transition`

Ahora vamos a ver algunos conceptos para tener más claro estas propiedades:

## Espaciado: padding y margin

Las dos propiedades principales: `padding` y `margin`

- El `padding` (relleno en español) se usa como bien dice la palabra para rellenar el interior de un elemento (dentro del borde)
- El `margin` (margen en español) se usa para separar elementos (fuera del borde)

``` En Developer Tools el contenido se representa en azul, el padding se representa en verde y los margenes en naranja ``` 

![1](https://i.imgur.com/Az50G0a.png)

El orden de anidación de un elemento es el siguiente: 

- Contenido del elemento -> `padding`->`border`->`margin`

Entonces si queremos un cuadrado con border y margen:

![1](https://i.imgur.com/ARE4LVc.png)
