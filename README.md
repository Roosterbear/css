# css

Crear un proyecto en VSC, agregando un index.html con ! y tabulador.

Bajo los _meta_ agregar 2 etiquetas link con tabulador, ambos con __rel="stylesheet"__

* En el primer _link_ agregamos en el __href__ las fonts de la siguiente URL: https://fonts.googleapis.com/

  * Agregamos la carpeta __css__ + el signo de __?__ y la variable __family__ + el __signo de =__

  * Ahora agregamos el nombre de la fuente + __:__ (_Lato:_) y las medidas separadas por comas (_100,300,400,700,900_)
    _Quedando: href="https://fonts.googleapis.com/css?family=Lato:100,300,400,700,900"_

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

  __background-image__ _Para agregar una imagen ponemos la ruta, Ejm. url(../image/hero.jpg)_

  __height__  _Se recomiend usar la medida vh, que es la altura del viewport en porcentaje, Ejm. 95vh_

  __background-size__ _cover para cubrir todo_
  
  __background-position__  _Es la parte que tendra prioridad en caso de disminuir_ 
                           _Puede ser: top, center, bottom_
