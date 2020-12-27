# Componente de Carrusel

En este repositorio se creo un componente que cumple la función de un carrusel de imágenes usando JavaScript vanilla y evidentemente HTML y CSS. Se que este tipo de componentes no es nada novedoso pero realizando ciertas funcionalidades al encontrarme creando un sitio web me encontré con el problema de que al emplear un carrusel de imágenes que había creado hace un tiempo este actuaba como un gran componente con cada uno de los carruseles que distribuía en cada sección del sitio en vez de actuar como pequeños carruseles independientes uno del otro.  

Con este problema en frente y con algo de tiempo libre decidí optimizár el componente de carrusel que en su memento me funciono bien al ser usado una sola vez y no en multitud de ocasiones como era este el caso. He aquí el resultado, no se si sera el mejor o peor carrusel que se viera pero como proyecto de una tarde de sábado no estuvo mal.  

# Como emplear el carrusel

En primer lugar debo aclarar que el fichero **carousel.html** sencillamente es un ejemplo de como se debe estructurar el código HTML dentro de su proyecto para usar este carrusel, se puede prescindir de ese fichero al igual que de la carpeta **src/img** que solo contiene imágenes de pruebas. Los archivos realmente importantes están en las carpetas **src/js** y **src/css**, estos si son indispensables para el funcionamiento del carrusel.  

Dentro de esta carpeta **src** encontrara:  

- src
    - css
        - carousel.css
    - img
        - *'Conjunto de imágenes de prueba'*
    - js
        - carousel.js

Es libre de añadir los cambios que crea combeniente en el código CSS y JavaScript.  

Para usar el carrusel debe copiar y pegar la siguiente linea de código HTML donde quiera introducir el carrusel:  

```html
    <div class="carousel" id="carousel-2">
        <div class="carousel__ballBox">
            <a class="carousel__ballLink" href="#"><div data-id="01" class="carousel__ball carousel__ball--red"></div></a>
            <a class="carousel__ballLink" href="#"><div data-id="02" class="carousel__ball"></div></a>
        </div>
        <div class="carousel__sliders">
            <img class="carousel__slide  carousel__slide--visible" data-id="01" src="src/img/wallhaven-p8dpwp.jpg" alt="">
            <img class="carousel__slide" src="src/img/wallhaven-q6g1e5.png" data-id="02" alt="">
        </div>
    </div>
```

La única modificación que deberá agregar sera remplazar el valor de los atributos **src** de las etiquetas ``<img>`` con la ruta de las imágenes propias que desee utilizar en su carrusel.

Si quiere agregar más imágenes solo debe copiar y pegar la cantidad de etiquetas ``<img>`` tal cual como se muestra en el ejemplo, sin embargo recuerde hacer lo mismo con las etiquetas ``<a></a>`` y su contenido tantas veces como imágenes tenga agregadas en el ``<div class="carousel__sliders"></div>``.  

Ejemplo:  

```html
    <div class="carousel" id="carousel-1">
        <div class="carousel__ballBox">
            <a href="#" class="carousel__ballLink"><div class="carousel__ball carousel__ball--red" data-id="01"></div></a>
            <a href="#" class="carousel__ballLink"><div data-id="02" class="carousel__ball"></div></a>
            <a href="#" class="carousel__ballLink"><div data-id="03" class="carousel__ball"></div></a>
        </div>
        <div class="carousel__sliders">
            <img class="carousel__slide carousel__slide--visible" data_id="01" src="src/img/wallhaven-96qy3w.jpg" alt="">
            <img class="carousel__slide" data_id="02" src="src/img/wallhaven-eyl1xr.jpg" alt="">
            <img class="carousel__slide" data_id="03" src="src/img/wallhaven-p27wge.png" alt="">
        </div>
    </div>
```

Eso seria todo lo necesario para la implementación de este sencillo carrusel de imágenes. Espero lo disfruten.

# Tecnologías usadas

- ## HTML
- ## CSS
- ## JavaScript