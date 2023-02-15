# css

Crear un proyecto en VSC, agregando un index.html con ! y tabulador.

Bajo los _meta_ agregar 2 etiquetas link con tabulador, ambos con __rel="stylesheet"__

* En el primer _link_ agregamos en el __href__ las fonts de la siguiente URL: https://fonts.googleapis.com/

  * Agregamos la carpeta __css__ + el signo de __?__ y la variable __family__ + el __signo de =__

  * Ahora agregamos el nombre de la fuente + __:__ (_Lato:_) y las medidas separadas por comas (_100,300,400,700,900_)

    _Quedando algo como: href="https://fonts.googleapis.com/css?family=Lato:100,300,400,700,900"_

* En el segundo _link_ agregamos en __href__ la carpeta(s) separando con una __/__ y el nombre del archivo __.css__

En el archivo __.css__ agregamos un reset basico con el _selector universal_ como el siguiente:

```

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

```

### Cambiamos la fuente general con el selector body

  __font-family__  _Ponemos el nombre de la fuente entre comillas_
                   _Se recomienda poner fuentes mas comunes al final_
                   _Al final debemos poner el tipo mas general: sans o sans-serif_

  __font-weight__  _Puede ser bold, bolder, thin, normal, 100, 700, 400, 900_
  
  __line-height__  _Es una proporcion relativa a 1, que es el 100%. Ejm: 1.7_
  

### Creamos una etiqueta que envuelva nuestro encabezado

  __background-image__ _Para agregar una imagen ponemos la ruta_
                       _Ejm. url(../image/hero.jpg)_
  __AGREGAR GRADIENT__
  _Antes de url, agregamos la palabra_ __linear-gradient()__ _y separamos con una coma_
  _Dentro de los parentesis agregamos 2 codigos de color: el inicial y el final, Ejm. #7ED56F, 28B485_
  _Podemos manejar transparencias con codigo RGBA, Ejm. rgba(126, 213, 111, 0.8), rgba(40, 180, 131, 0.8)_
  _Siendo 0.8 el 80%_
  _Antes de los codigos de color podemos agregar el sentido a donde cambiaran los colores:_
  _top / bottom y right / left, separados de los colores por una coma. Ejm. to right bottom_
                      
  __height__  _Se recomiend usar la medida vh, que es la altura del viewport en porcentaje, Ejm. 95vh_

  __background-size__ _cover para cubrir todo_
  
  __background-position__  _Es la parte que tendra prioridad en caso de disminuir_ 
                           _Puede ser: top, center, bottom_

### Imagen de logo

_Agregamos un div con una clase llamada_ __logo-box__
_Dentro del div logo-box agregamos una imagen con la clase_ __logo__
__A la clase padre de box__ _le agregamos_ __position: relative__
__A la clase box__ _le agregamos_ __position: absolute__
__A la clase box__ _le damos un valor top y otro left donde mostrara la imagen_
__A la clase logo__ _le agregamos un height para alterar tamaño de la imagen_ 

### Texto central

_Como ya tenemos la clase padre en relative, creamos dentro una para el texto_
_Creamos un div_ __text-box__ _con posicion absoluta_
_Le ponemos un top:40% y un left: 50%_
_Comienza a poner el texto desde la esquina y no se ve centrado, por lo que agregamos:_
__transform: translate(-50%, -50%);__
_Con la finalidad de agregar 2 titulos en un solo H1 para SEO creamos una clase_ __heading-primary__
_Dentro agregamos 2 span con clases:_ __heading-primary-main__ y __heading-primary-sub__
_A la clase del H1 le agregamos el color y el_ __text-transform__ _a uppercase_
_A los headings de los span les ponemos_ __display:block__
_Le damos una fuente mas grande (60px y 20px) y un espaciado mayor (35px y 17.4)_
_Por default H1 tiene el peso de 700, asi que se lo cambiamos a 400_ __font-weight:400;__

### Animacion de texto

_Se crean con la instruccion_ __@keyframes__ _mas el nombre que deseamos poner y llaves_
__Estado inicial__
_Le ponemos un_ __0%__ _y llaves para encerrar los efectos_
_Para que aparezca iniciamos con_ __opacity:0__
_Si queremos mover de izquierda a derecha usamos_ __transform: translateX(-100)__
_Esto movera en el eje de las x 100px al iniciar_
__Estado final__
_Lo ponemos con_ __100%__ _y las llaves para encerrar los efectos_
_Si queremos efectos intermedios ponemos otro porcentaje como 30% o 70%_
__usar el efecto__
_Para usar el efecto, en la clase del texto debemos agregar:_ __animation-name:__ _+nombre de animacion_
_Ademas debemos agregarle_ __animation-duration: 5s__ _con los segundos deseados_
_Existen otras funciones como_ __animation-timing-function: ease-out__, __animation-delay: 3s__ o __animation-iteration-count: 3__






