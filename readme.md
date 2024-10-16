# Titulo Del Proyecto:

**Blog De Noticias Realizado En HTML Y CSS (Contenido Flexible)** 

## Descripción Detallada Del Proyecto
**Elaboramos un pequeño blog de Noticias donde aplicamos las propiedades de CSS contenido flexible, además se implementó para poder verlo en 3 dispositivos diferentes en este caso fue una Computadora, un Ipad y un dispositivo móvil solo utilizando CSS y algunas de sus propiedades como el Media Query**

## Estructura HTML Del Proyecto
**Para realizar el blog lo que hicimos fue estructurar nuestra página web en secciones, además con un navbar  y para poder mostrar la información de la noticia haciendo uso de la etiqueta <article>, así mismo tenemos párrafos, imágenes y contenedores que nos van a permitir aplicarle algunos estilos CSS para poder hacer una responsiva en los dispositivos antes mencionados por ultimo tenemos la parte del pie de página conocido también como footer que es la parte final de una página web. Puedes checar nuestro archivo index.html de nuestro repositorio para ver el código completo**

## Adaptable A una computadora
**Para poder verlo en una computadora basta con aplicar algunos estilos normales o propiedades de CSS como puedes ver en el archivo style.css de nuestro repositorio algunas propiedades como lo son: fondos, tamaños, márgenes o paddings, aplicando contenido flexible en el navbar con las propiedades display:flex ,align-items,flex-grow anchos máximos, etc. con estas propiedades vamos a poder distribuir de forma flexible todo el contenido de nuestra blog como los párrafos, secciones, contenedores e imágenes y nuestro footer. A continuación muestro un poco del código de antes mencionado puedes ver el código completo en nuestro archivo styles.css**
```CSS
    nav{
        max-width: 900px;
        margin: auto;
    }
    nav ul{
        display: flex;
        align-items: center;
    }
    nav li{
        background: #7e7e7e;
        padding: 5px;
        height: 25px;
        list-style: none;
        margin-right: 8px;
        border-radius: 3px;

    }
    .categoria{
        display: flex;
        background: #f1f1f1;
        padding: 10px;
        margin-bottom: 10px
        border-bottom 1.5px solid #b5b5b5;
        border: solid 1.5px  rgb(194, 193, 193);
    }
    .articulorelacionado{
        width: 280px;
        /*height: 150px;*/
        background: #3cb2c8;
        margin:auto;
        margin-bottom: 5px;
        padding: 6px;
        color: #ffffff;
        transition: all .2s;
    }
```
# Vista previa del blog funcionando en nuestra computadora:
![vista previa del proyecto](/IMG/blog1.png)
![vista previa del proyecto](/IMG/blog2.png)
![vista previa del proyecto](/IMG/blog3.png)

## Adaptable a una Tablet o IPAD
**Para poder adaptar nuestro proyecto a una resolución de una Tablet o IPAD aquí si tenemos que hacer uso de la propiedad de CSS Media Queries es decir que aplique ciertos estilos dependiendo la resolución de la pantalla en este caso hicimos que se adaptara  a un tamaño como ancho máximo a 768px al igual colocamos propiedades de CSS de contenido flexible para acomodar los elementos de la página. A continuación muestro el código CSS aplicando un Media Query** 
```CSS
    @media (max-width: 768px){
        #contenedor{
            flex-direction: column;
            margin-bottom: 0px;
        }
        #contenedor aside{
            width: 100%;
            padding: 10px;
            display: flex;
            flex-wrap: wrap;
            align-items: flex-start;
            background: #3cb2c8;
        }
        .articulorelacionado{
            width: 47%;
        }
        nav, footer{
            max-width: 95%;
        }
        nav li.menu{
            padding-bottom: 25px;
        }
    }
```
# Vista de cómo se adaptó la pantalla que tiene una Tablet(contenido en dos columnas)
![vista previa del proyecto](/IMG/flex.png)

## Adaptable a una dispositivo móvil
**Para adaptar a un dispositivo móvil es decir a una pantalla de celular también tenemos que hacer uso del Media Query pero esta vez en una resolución más pequeña que la anterior es decir un ancho máximo de 412px, para poder aplicarles los estilos de CSS flexibles que harán que el contenido se adapte al tamaño de la pantalla aplicándoselas al logo, texto, navbar, imágenes, footer es decir a todo el artículo en general. A continuación muestro el código CSS del uso del Media Query en un dispositivo móvil:**
```CSS
    @media (max-width: 412px){
        ul{
            max-width: 95%;
            flex-wrap: wrap-reverse;
        }
        .logo{
            margin: auto;
            margin-bottom: 10px;
        }
        nav ul{
            display: flex;
            justify-content: center;
        }
        nav li.menu{
            margin-left:24px;
        }
        footer{
            padding-bottom: 0px;
            flex-direction: column;
            text-align: center;
            background: #414141;
            padding-bottom: 12px;
        }
        .articulorelacionado{
            width: 100%;
        }

    }
```

# Vista de cómo se adaptó la pantalla de un celular(contenido en una sola columna)
![vista previa del proyecto](/IMG/movil1.png)
![vista previa del proyecto](/IMG/movil2.png)

## Lista De Tecnologías, Herramientas Y Algunas Propiedades Web Que Se Usaron En Nuestro Proyecto

1. HTML(Estructura General)
2. CSS (Responsive)    
3. CSS(display flex,flex-direction,flex-wrap y align-items)
4. CSS(justify-content y flex-grow,etc)
5. HTML(Etiquetado Web(div,article,seccion,p,img,h,footer,etc))
6. CSS(paaddings,margins,background,borders,height,max-width,etc.)
7. CSS(Uso De Media Query)
8. GitHub
9. Herramienta de Visual Studio Code(live Server)

*Elaborado Por: Mario Martínez Aguilar*
