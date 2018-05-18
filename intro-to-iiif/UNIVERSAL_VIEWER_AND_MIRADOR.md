# Universal Viewer y Mirador
Hasta ahora nos hemos confinado principalmente a la API de Imagen de IIIF. Herramientas como OpenSeadragon y Leaflet se sitúan sobre la API de Imagen para ofrecer comportamiento de zoom, pero ¿y si quisiéramos toda la riqueza de navegar colecciones estructuradas: proporcionar información y metadatos a los usuarios, tablas de contenidos, y anotaciones?

La API de Presentación ofrece las herramientas para modelar esas características de su contenido, y Universal Viewer y Mirador son "visores IIIF-completos" en el sentido de que manifiestan este contenido para el usuario.
### Universal Viewer
[UV](http://universalviewer.io/examples/#?c=0&m=0&s=0&cv=0&xywh=-1377%2C-197%2C5321%2C3936) ha sido desarrollado como una herramienta de código abierto por la firma británica Digirati para usar en el entorno IIIF de la British Library. Toma un manifest o colección y ofrece una ventana a su contenido donde puede ver sus metadatos y navegarlo de varias maneras.
Está disponible en `npm` y tiene muchos ejemplos en el enlace anterior.
### Mirador
Mirador nació de las necesidades de los estudiosos de Historia del Arte y Manuscritos de la Universidad de Stanford y ha crecido mediante una colaboración multi-institucional con la Universidad de Harvard y un par de docenas de contribuyentes de todo el mundo. Además de visualización, proporciona configuraciones para guardar estado, crear anotaciones mediante el backend, y comparar múltiples objetos de diferentes instituciones en un espacio de trabajo de ventanas.

Para información general del proyecto y demos, vea [ProjectMirador.org](http://projectmirador.org/).
Para comenzar, visite la [documentación](http://projectmirador.org/docs/docs/getting-started.html)

Mirador está disponible como una distribución pre-construída, a través de `npm`, o la reciente [gem Mirador-rails](https://github.com/sul-dlss/mirador_rails).

### ¿De Dónde Vienen Los Manifests?
Cuando tenga un servidor de imágenes en ejecución, puede crear "manifests" de la API de Presentación que apunten a esos recursos y proporcionen estructura enriquecida e información presentacional a visores como Mirador y UV. Muchas instituciones generan sus manifests de presentación a partir de metadatos institucionales existentes para mostrar a sus usuarios. Otras los crean a mano.

Esta es una muy sencilla, pero completa, respuesta de manifest tomada de las especificaciones: [http://iiif.io/api/presentation/2.1/#c-example-manifest-response](http://iiif.io/api/presentation/2.1/#c-example-manifest-response)

Y estos son algunos más complejos:
[https://purl.stanford.edu/qm670kv1873/iiif/manifest.json](https://purl.stanford.edu/qm670kv1873/iiif/manifest.json)
[http://iiif.harvardartmuseums.org/manifests/object/320567](http://iiif.harvardartmuseums.org/manifests/object/320567)
[http://iiif.bodleian.ox.ac.uk/iiif/manifest/51a65464-6408-4a78-9fd1-93e1fa995b9c.json](http://iiif.bodleian.ox.ac.uk/iiif/manifest/51a65464-6408-4a78-9fd1-93e1fa995b9c.json)
[http://media.nga.gov/public/manifests/nga_highlights.json](http://media.nga.gov/public/manifests/nga_highlights.json)
