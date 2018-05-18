# Etiquetas de Imagen de HTML

La API de Imagen de IIIF expone imágenes en forma robusta. Estas imágenes se pueden usar de diversas maneras, la más simple de las cuales es una etiqueta de imagen de HTML.

<iframe width="100%" height="300" src="//jsfiddle.net/mejackreed/r3a5ayhe/2/embedded/html,result/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

Veamos esa uri de imagen, y qué está pasando. [Sintaxis de URI de Petición de Imagen de IIIF](http://iiif.io/api/image/2.1/#image-request-uri-syntax)

```javascript
https://stacks.stanford.edu/image/iiif/hg676jb4964%2F0380_796-44/1015,1460,799,824/pct:50/0/default.jpg
```

| Parte de la URI | Parámetro de IIIF |
| -- | -- |
| https | {scheme} |
| stacks.stanford.edu | {server} |
| image/iiif | {prefix} |
| hg676jb4964%2F0380_796-44 | {identifier} |
| 1015,1460,799,824 | {region} |
| pct:50 | {size} |
| 0 | {rotation} |
| default | {quality} |
| jpg | {format} |


Usando esta manipulación de parámetros es posible modificar como se muestran las imágenes en una etiqueta de imagen de HTML.

Algo que señalar aquí, es que no todos los Servidores de Imágenes de IIIF compatibles pueden manejar todos estos parámetros. Esta información se ofrece a un consumidor de IIIF a través de la respuesta `info.json` y el [nivel de compatibilidad](http://iiif.io/api/image/2.1/compliance/) del servidor de IIIF.

Las uris de imagen de IIIF también se pueden insertar en CSS u hojas de estilo. Un ejemplo de esto está en el software [Spotlight](https://github.com/projectblacklight/spotlight) donde los títulos de las muestras tienen una imagen de fondo que es servida desde un servidor de IIIF.

[![spotlight masthead](images/spotlight_masthead.png)](https://exhibits.stanford.edu/fitch)

¿Ve como hay una url de IIIF de aspecto similar en el atributo style? Vea esa imagen de título [visitándola directamente](https://exhibits.stanford.edu/images/44/0,37,1334,133/1800,180/0/default.jpg).

```html
<div class="masthead image-masthead ">
    <span class="background-container" style="background-image: url('https://exhibits.stanford.edu/images/44/0,37,1334,133/1800,180/0/default.jpg')"></span>
    <span class="background-container-gradient"></span>
  ...
</div>
```
