# Fundaci-n-Semilla
Metodología SCRUM - Projects

Historias de usuario:
Requerimientos del Dashboard
1. Debe tener sección que indique el estado de ánimo del estudiante
2. Fácil manejo
3. Organización de tareas (Horario)
4. Tenga 6 animaciones
5. Este acorde con la temática del diplomado, sostenibilidad ambiental
6. Cumpla con estandares producto MVP.
7. Cumpla con tipografia y colores deseados
8. Cuente con el logo de la fundación
9. Espacio para las fotos de perfiles
10.Espacio de comentarios

Documentación Semilla

1.	Se creo el repositorio en el github, posteriormente cada desarrollador clono el repositorio en su pc local; en la rama principal se crearon 2 carpetas, una de estilos y una de imágenes, se creó un archivo html.
2.	se descargaron las imagenes y fuentes a utilizar para el tablero
3.	En la carpeta de estilos cada desarrollador tiene una hoja de estilos personal y ademas se encuentran otras hojas de estilos responsive para movil y tablet.
4.HEADER
en la parte del encabezado se inserto una imagen que iba contener el titulo principal , el menu lateral, y el logo de semillas; 

![image](https://user-images.githubusercontent.com/112130785/199104301-c6e76cc9-8487-4586-94fb-502855ec26fb.png)
![image](https://user-images.githubusercontent.com/112130785/199104510-f1f1951c-64ad-49bd-8131-8856b311ffd0.png)
 
 como se puede evidenciar en la imagen a la imagen que iba a estar en el encabezado se le dio un ancho del 100% para que abarcara todo el ancho de la pantalla, encima del encabezado se sobrepuso el titulo principal y el logo de semillas
 
 5.para el menu vertical  se trabajo dentro de un contenedor; este menu es desplegable y se sobrepone sobre toda la pagina; para que fuera despegable y sobresaliera sobre toda la pagina se utilizo una seudoclase , es decir un hover con ciertas caracteristicas.
 
 ![image](https://user-images.githubusercontent.com/112130785/199105548-30b13f23-4773-47fa-8fd0-25afe1bffaf7.png)
 ![image](https://user-images.githubusercontent.com/112130785/199105678-a1f04d9a-27c0-4cd4-98d3-fa6a660e3146.png)
 
 6.Dentro del menu se agrego unna lista que iba a contener algunas elecciones donde el administrador puede seleccionar y consultar; para las opciones de diplomados, calificaciones y horarios, se aplico una etiqueta de summary para que de ellas se desplegara varias opciones.
 
 ![image](https://user-images.githubusercontent.com/112130785/199106391-b3ffe6c5-0566-4a99-ade3-987717a48fe1.png)
![image](https://user-images.githubusercontent.com/112130785/199106458-097df5fd-395d-417e-b057-4293d93ad4cd.png)

7. para los emojis se hicieron atravez de unos divs anidados , cada uno de ellos contenia una parte del emoji , es decir , cara , ojos y boca; luego se le dio estilos  con background color especificco , border radius para que fuera completamente redondo y una seudoclas hover o transform para que implementarle una animacion respectiva a cada emoji.
![image](https://user-images.githubusercontent.com/112130785/199112952-36eb42d7-bc57-4757-bed9-b4500f1b0d91.png)
![image](https://user-images.githubusercontent.com/112130785/199113001-b715f430-683a-4627-bebe-ff84f7c674e9.png)

8. para el footer se aplico un display flex para alinear las imagnes en una fila al igual que los terminos y condiciones y las opciones de redirigir a otras paginas con la etiqueta a.

![image](https://user-images.githubusercontent.com/112130785/199113322-c9ce8b1d-fa1a-47d3-8355-286512dd1fa6.png)
![image](https://user-images.githubusercontent.com/112130785/199113403-87bf56d8-d6ad-4122-891d-949af6985063.png)

Posición

Posicionar un rectángulo en svg es tan fácil como establecer las coordenadas (X,Y) de la esquina superior izquierda del rectángulo, donde el punto de origen (0,0) será la esquina superior izquierda del lienzo SVG.
Propiedades para posicionar rectángulos:
•	X.- indica la distancia entre el borde izquierdo del lienzo SVG y el borde izquierdo del rectángulo.
•	Y.- indica la distancia entre el borde superior del lienzo SVG y el borde superior del rectángulo.

Ejemplo:

 
Resultado:
 

Veamos un ejemplo en que podamos distinguir el lienzo SVG, el rectángulo dentro de ella y la posición que toma al establecer las propiedades X y Y. Para nuestro propósito colocaremos un borde solido de 1px y color negro al lienzo SVG, luego podremos marcar las distancias de posicionamiento, veamos.
 

 
TABLA
Ya no podemos usar el atributo border="1" porque es algo obsoleto, soportado, sí, pero obsoleto. Para agregar bordes a una tabla de la manera correcta usamos CSS.
Pero antes de eso, vamos a ver cómo es una tabla en HTML.
Una tabla (que se representa con <table>) lleva un encabezado, definido por la etiqueta <thead>, y un cuerpo definido por <tbody>. Y dentro lleva table rows o filas de tabla, con la etiqueta <tr>. Si es un encabezado lleva table headers o <th> y si es cuerpo lleva table data con la etiqueta <td>.
 

Animaciones:
Caminos de SVG
Si hay un elemento sobrecargado en SVG, ese sería el elemento <ruta>.
El elemento ruta es una forma básica que se puede usar para crear casi cualquier forma 2D avanzada que puedas imaginar.
El elemento funciona al tomar una secuencia de comandos de dibujo. Se parece mucho al lenguaje de programación Logo de 1967, solo modernizado y diseñado para gráficos sofisticados. El elemento toma esta secuencia de comandos de dibujo a través del atributo d.
Un triángulo rectángulo
<path d="M10 10 L75 10 L75 75 Z" />
Puedes pensar en un bolígrafo virtual que se dibuja en la pantalla, y los comentarios de dibujo en el elemento de ruta simplemente controlan el bolígrafo. En el ejemplo anterior, se le indica al bolígrafo que se mueva a la posición (10, 10) (M10 10), para dibujar una línea a (75, 10) (L75 10), para dibujar un línea a (75, 75) L75 75 y luego cerrar la ruta volviendo al punto inicial (Z).
Usando otros comandos de dibujo, como arcos (A), curvas de bezier cuadráticas (Q), curvas de bezier cúbicas (C), etc., puede crear formas y gráficos mucho más complejos en SVG.
Caminos SVG y CSS
Para nuestra primera técnica, vamos a aprovechar dos atributos de SVG: stroke-dasharray y stroke-dashoffset.
Los archivos SVG se pueden animar de la misma manera que los elementos HTML, mediante el uso de fotogramas clave CSS y propiedades de animación o mediante el uso de transiciones CSS. Las animaciones más complejas generalmente tienen algún tipo de transformación aplicada: una traducción, rotación, escalado o sesgo.
El atributo stroke-dasharray controla el patrón de rayas y lagunas utilizadas para trazar el camino. Si deseas dibujar sus líneas como un grupo de guiones y espacios en lugar de un trazo continuo de tinta, este es el atributo que usaría.
Como las imágenes SVG son parte del DOM del navegador web y stroke-dasharray es un elemento de presentación, el atributo también se puede configurar mediante CSS.
Del mismo modo, el atributo stroke-dashoffset (que especifica qué tan lejos está en el patrón del tablero para comenzar el guión) también se puede controlar usando CSS.
Estos dos atributos SVG, juntos, se pueden usar para animar rutas SVG, dando al espectador la ilusión de que las rutas se están dibujando gradualmente.
Animación básica
La siguiente animación es muy simple. Lo que hace es que, al pasar el ratón por encima de la pantalla, la rueda aumente de tamaño:
 
Rueda Girando:
Primero, debes configurar los keyframes de rotación (en este caso @keyframes spin y @keyframes FadeIn). Como se trata de un gráfico giratorio, es necesario realizar una rotación completa. También se aplicará un efecto de fundido de entrada también.
A continuación, es importante crear un contenedor SVG (svg-container).
Se crearán estilos SVG generales y aquí es donde se especifica el origen de la transformación (etiqueta SVG).
 
Se usan dos reglas para asegurar la compatibilidad con los navegadores:
@keyframes rotate – Navegadores Firefox e Internet Explorer.
@-webkit-keyframes rotate – Navegadores que usan WebKit (Google Chrome, Safari)

Valores que se pueden modificar

En la propiedad "animation" se usan los siguientes valores que se pueden modificar:
3s – Intervalo en segundos de la rotación
rotate – Tipo de animación
linear – Tipo de movimiento
infinite – Duración de la animación

La sintaxis general de la propiedad transition es:
 
 
Cada parámetro es:
1.	transition-poperty: propiedad a la que se le va a aplicar el efecto de transición. Cualquier propiedad CSS es válida: width, height, color, border, etc.
2.	transition-duration: duración del efecto. Puede ser en segundos (s) o milisegundos (ms).
3.	trasition-timing-function: define la curva de velocidad a la que se produce el efecto. Puede ser:
o	ease: este es el valor por defecto. Tiene un comienzo lento, luego rápido y termina de nuevo lentamente. Es equivalente a cubic-bezier(0.25,0.1,0.25,1).
o	linear: la misma velocidad durante toda la duración de la transición. Equivalente a cubic-bezier(0,0,1,1).
o	ease-in: efecto de transición con comienzo lento. Equivalente a cubic-bezier(0.42,0,1,1).
o	ease-out: efecto de transición con comienzo rápido y final lento. Equivalente a cubic-bezier(0,0,0.58,1).
o	ease-in-out: efecto de transición con comienzo y final lento; más rápido en medio. Equivalente a cubic-bezier(0.42,0,0.58,1).
o	cubic-bezier(n,n,n,n): define tus propios valores para la curva de Bezier. Cada valor es entre 0 y 1.
o	initial: establece esta propiedad a su valor por defecto.
o	inherit: hereda esta propiedad del elemento padre.
4.	transition-delay: retraso en el comienzo de la transición. Puede ser en segundos (s) o milisegundos (ms).


Degradados:
Vamos a crear dos degradados lineales usando dos colores (inicio y fin) y a asignarles una ID única para poder identificarlos, llamarlos y aplicarlos sobre los elementos que queramos, que en nuestro caso será sobre <text> usando el atributo [fill].
 

Un degradado es una transición suave de un color a otro. Además, se pueden aplicar varias transiciones de color a un mismo elemento.
Hay dos tipos principales de degradados en SVG:
•	Lineal
•	Radial
SVG Gradiente lineal - <linearGradient>
El elemento <linearGradient> se utiliza para definir un degradado lineal.
El elemento <linearGradient> debe estar anidado dentro de una etiqueta <defs>. La etiqueta <defs> es la abreviatura de definiciones y contiene definiciones de elementos especiales (como degradados).
Los degradados lineales se pueden definir como degradados horizontales, verticales o angulares:
•	Los gradientes horizontales se crean cuando y1 e y2 son iguales y x1 y x2 difieren
•	Los gradientes verticales se crean cuando x1 y x2 son iguales y y1 e y2 difieren
•	Los gradientes angulares se crean cuando x1 y x2 difieren y y1 e y2 difieren

Ejemplo:
 
 

•	El atributo id de la etiqueta <linearGradient> define un nombre único para el degradado
•	Los atributos x1, x2, y1, y2 de la etiqueta <linearGradient> definen la posición inicial y final del degradado
•	La gama de colores de un degradado puede estar compuesta por dos o más colores. Cada color se especifica con una etiqueta <stop>. El atributo de compensación se usa para definir dónde comienza y termina el color degradado
•	El atributo de relleno vincula el elemento de elipse al degradado.


documentacion jhon fredy bernal rojas  
encargado de la seccion b del body 

1.  emmpese buscando como hacer que el titulo puediera tener una animacion con css y  obtuve un muy buen resultado ya que el titulo al recargar lapagina     se desplaza de derecha a izquierda esto lo consegui con el siguiente codigo de css 


@keyframes titulo-diplomados{/*---------asi se describen los fotogramas de la animacion----------*/
    from{/*-------fotograma donde empieza la animacion---------*/
        margin-left: 100%;
        width: 300%
    }

    to {/*------------fotograma donde termina la animacion-------------*/
        margin-left: 0%;
        width: 100%;
    }
}


2. de hay continue con la busqueda de cono hacer un medidor de minimo a maximo intente buscarlo solo con css y html  pero no logre conseguirlo  asi que      use uno que tenia funcionalidad script pero le quite la funcionalidad quedo solo como maqueta y lo consegui con el siguiente codigo 


                        <div class="wrapper">
                            <div>
                                <div class="line"></div>
                                <div class="number n0">0%</div>
                                <div class="number n25">25%</div>
                                <div class="number n90">50%</div>
                                <div class="number n75">75%</div>
                                <div class="number n180">100%</div>
                                <div class="circle2"></div>
                                <div class="circle1"></div>
                            </div>
                            <input type="number" min="0" max="100" value="0">
                        </div>
                        <div>
                            <DIV class="lista-del-medidor"> 
                                <UL class="significado-de-los-volores" >
                                    <LI class="uno">MAL</LI>
                                    <LI class="dos">REGULAR</LI>
                                    <LI class="tres">BIEN</LI>
                                    <LI class="cuatro">EXELENTE</LI>
                                </UL>
                            </DIV>
                        </div>
                        
                        
3. el siguiente paso complicado para mi fue hacer una estadistica lineal  del la asistencia promedio semanal   en ese me tomo un poco mas de tiempo encontrar como hacerlo pero afin lo consegui y lo logre con un codigo html  vasico y un css algo compejo  


body{
  background-color: #ededed;
}
.board{
    margin: auto;
    width: 55%;
    height: 450px;
    background-color: #e2e2e2;
    padding: 10px;
    box-sizing: border-box;
    overflow: hidden;
}
.titulo_grafica{
    width: 100%;
    height: 10%;
}
.titulo_grafica>h3{
    padding: 0;
    margin: 0px;
    text-align: center;
    color: #666666;
}
.sub_board{
    width: 100%;
    height: 90%;
    padding: 10px;
    margin-top: 0px;
    background-color:#f4f4f4;
    overflow: hidden;
    box-sizing: border-box;
}
.sep_board{
    width: 100%;
    height: 10%;
}
.cont_board{
    width: 100%;
    height: 80%;
}
.graf_board{
    width: 85%;
    height: 100%;
    float: right;
    margin-top: 0px;
    background-color: darkgrey;
    border-left: 2px solid #999999;
    border-bottom: 2px solid #999999;
    box-sizing: border-box;
    display: flex;
    background: -moz-linear-gradient(top, rgba(0,0,0,0) 0%, 
    rgba(0,0,0,0) 9.5%,  rgba(0,0,0,0.3) 10%, rgba(0,0,0,0) 10.5%, 
    rgba(0,0,0,0) 19.5%, rgba(0,0,0,0.3) 20%, rgba(0,0,0,0) 20.5%, 
    rgba(0,0,0,0) 29.5%, rgba(0,0,0,0.3) 30%, rgba(0,0,0,0) 30.5%, 
    rgba(0,0,0,0) 39.5%, rgba(0,0,0,0.3) 40%, rgba(0,0,0,0) 40.5%, 
    rgba(0,0,0,0) 49.5%, rgba(0,0,0,0.3) 50%, rgba(0,0,0,0) 50.5%, 
    rgba(0,0,0,0) 59.5%, rgba(0,0,0,0.3) 60%, rgba(0,0,0,0) 60.5%, 
    rgba(0,0,0,0) 69.5%, rgba(0,0,0,0.3) 70%, rgba(0,0,0,0) 70.5%, 
    rgba(0,0,0,0) 79.5%, rgba(0,0,0,0.3) 80%, rgba(0,0,0,0) 80.5%, 
    rgba(0,0,0,0) 89.5%, rgba(0,0,0,0.3) 90%, rgba(0,0,0,0) 90.5%,  
    rgba(0,0,0,0) 100%);

    background: -webkit-linear-gradient(top, rgba(0,0,0,0) 0%, 
    rgba(0,0,0,0) 9.5%,  rgba(0,0,0,0.3) 10%, rgba(0,0,0,0) 10.5%, 
    rgba(0,0,0,0) 19.5%, rgba(0,0,0,0.3) 20%, rgba(0,0,0,0) 20.5%, 
    rgba(0,0,0,0) 29.5%, rgba(0,0,0,0.3) 30%, rgba(0,0,0,0) 30.5%, 
    rgba(0,0,0,0) 39.5%, rgba(0,0,0,0.3) 40%, rgba(0,0,0,0) 40.5%, 
    rgba(0,0,0,0) 49.5%, rgba(0,0,0,0.3) 50%, rgba(0,0,0,0) 50.5%, 
    rgba(0,0,0,0) 59.5%, rgba(0,0,0,0.3) 60%, rgba(0,0,0,0) 60.5%, 
    rgba(0,0,0,0) 69.5%, rgba(0,0,0,0.3) 70%, rgba(0,0,0,0) 70.5%, 
    rgba(0,0,0,0) 79.5%, rgba(0,0,0,0.3) 80%, rgba(0,0,0,0) 80.5%, 
    rgba(0,0,0,0) 89.5%, rgba(0,0,0,0.3) 90%, rgba(0,0,0,0) 90.5%,  
    rgba(0,0,0,0) 100%);

    background: linear-gradient(to bottom, rgba(0,0,0,0) 0%,
    rgba(0,0,0,0) 9.5%,  rgba(0,0,0,0.3) 10%, rgba(0,0,0,0) 10.5%, 
    rgba(0,0,0,0) 19.5%, rgba(0,0,0,0.3) 20%, rgba(0,0,0,0) 20.5%, 
    rgba(0,0,0,0) 29.5%, rgba(0,0,0,0.3) 30%, rgba(0,0,0,0) 30.5%, 
    rgba(0,0,0,0) 39.5%, rgba(0,0,0,0.3) 40%, rgba(0,0,0,0) 40.5%, 
    rgba(0,0,0,0) 49.5%, rgba(0,0,0,0.3) 50%, rgba(0,0,0,0) 50.5%, 
    rgba(0,0,0,0) 59.5%, rgba(0,0,0,0.3) 60%, rgba(0,0,0,0) 60.5%, 
    rgba(0,0,0,0) 69.5%, rgba(0,0,0,0.3) 70%, rgba(0,0,0,0) 70.5%, 
    rgba(0,0,0,0) 79.5%, rgba(0,0,0,0.3) 80%, rgba(0,0,0,0) 80.5%, 
    rgba(0,0,0,0) 89.5%, rgba(0,0,0,0.3) 90%, rgba(0,0,0,0) 90.5%, 
    rgba(0,0,0,0) 100%);

    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00ffffff', endColorstr='#00ffffff',GradientType=0 );
}
.barra{
    width:100%;
    height: 100%;
    margin-right: 15px;
    margin-left: 15px;
    background-color: none;
    display: flex;
    flex-wrap: wrap;
    align-items: flex-end;
}
.sub_barra{
    width: 100%;
    height: 80%;
    background: #00799b;
    background: -moz-linear-gradient(top, #00799b 0%, #64d1be 100%);
    background: -webkit-linear-gradient(top, #00799b 0%,#64d1be 100%);
    background: linear-gradient(to bottom, #00799b 0%,#64d1be 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00799b', endColorstr='#64d1be',GradientType=0 );
    
    -webkit-border-radius: 3px 3px 0 0;
    border-radius: 3px 3px 0 0;
}
.tag_g{
    position: relative;
    width: 100%;
    height: 100%;
    margin-bottom: 30px;
    text-align: center;
    margin-top: -20px;
    z-index: 2;
}
.tag_leyenda{
    width: 100%;
    text-align: center;
    margin-top: 5px;
}
.tag_board{
    height: 100%;
    width: 15%;
    border-bottom: 2px solid rgba(0,0,0,0);
    box-sizing: border-box;
}
.sub_tag_board{
    height: 100%;
    width: 100%;
    display: flex;
    align-items: flex-end;
    flex-wrap: wrap;
}
.sub_tag_board>div{
    width: 100%;
    height: 10%;
    text-align: right;
    padding-right: 10px;
    box-sizing: border-box;
}
.b1{ height: 35%}
.b2{ height: 45%}
.b3{ height: 55%}
.b4{ height: 75%}
.b5{ height: 85%}
footer{
    position: absolute;
    bottom: 0px;
    width: 100%;
    text-align: center;
    font-size: 12px;
    font-family: sans-serif;
}
       
       
       
4.  en este paso ya me fue un poco mas sencillo acomodar las estructuras con displey flex  para despues unir me trabajo con el de mis compañeros        
       
                        








