# Leaflet-IIIF

[Leaflet-IIIF](https://github.com/mejackreed/Leaflet-IIIF) es una librería de JavaScript para crear vistas zoomables de imágenes de IIIF. Es un plugin para la popular librería [LeafletJS](http://leafletjs.com/).

Veamos un ejemplo:

<iframe src="https://mejackreed.github.io/Leaflet-IIIF/examples/example.html" frameborder="0" width="100%" height="500px"></iframe>

Leaflet-IIIF permite usar la expresividad de Leaflet y su ecosistema de plugins simultáneamente para mostrar imágenes de IIIF.

Veamos esa instancia de Leaflet-IIIF y como funciona.


<iframe width="100%" height="300" src="//jsfiddle.net/mejackreed/r4gucLb8/embedded/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

El tilelayer de Leaflet-IIIF es una subclase de [L.Tilelayer](http://leafletjs.com/reference.html#tilelayer) y por tanto hereda muchas de las propiedades de esta clase, incluyendo opciones de instanciación, métodos y eventos. No todas son relevantes (o funcionan :))

Algunas de las razones para usar Leaflet-IIIF:

 - Es ligera (por mucho, la más ligera librería de la API de Imagen de IIIF)
 - Funciona muy bien en los móviles
 - Orientada a la accesibilidad
 - Una enorme [comunidad de plugins](http://leafletjs.com/plugins) con los cuales integrar

Una desventaja del plugin, es que alguna funcionalidad no está implementada aún. Pero en general maneja el 95% casos de uso.

[Más ejemplos de cosas divertidas que puede hacer con Leaflet-IIIF](https://bl.ocks.org/mejackreed).
