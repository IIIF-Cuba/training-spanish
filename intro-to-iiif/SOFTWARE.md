# Software

La mayor parte del software de IIIF desarrollado es de código abierto y se puede encontrar mediante la lista [Awesome-IIIF](https://github.com/IIIF/awesome-iiif).

Un ciclo típico de respuesta a petición de IIIF tiene este aspecto.

![IIIF request response](images/request_response.png)

Este ciclo de respuesta a petición sigue un patrón básico, donde un cliente de IIIF quiere mostrar un objeto compuesto por `n` imágenes. El cliente solicita entonces de un servidor un [`manifest.json`](https://purl.stanford.edu/cy496ky1984/iiif/manifest.json) de la API de Presentación de IIIF. El cliente parsea entonces el manifest, y empieza a construir una vista del objeto imagen. Por cada imagen que quiere mostrar, el cliente solicita entonces una respuesta [`info.json`](https://stacks.stanford.edu/image/iiif/cy496ky1984%2Fcy496ky1984_00_0002/info.json) del servidor de IIIF. La respuesta `info.json` contiene información sobre la imagen, incluyendo dimensiones, opciones del servidor de imagenes disponibles, y niveles de mosaico disponibles.

## Software de manifest de IIIF
Los manifests de IIIF se pueden servir como contenido estático o dinámico. El manifest puede ser muy complejo, pero en su nivel básico contiene metadatos sobre el objeto imagen. Existen [varias librerías](https://github.com/IIIF/awesome-iiif#presentation-api-libraries) para crear estos manifests.

## Software de servidor de imágenes de IIIF
Hay varias [aplicaciones de software de servidor de imágenes de IIIF](https://github.com/IIIF/awesome-iiif#image-api-libraries) disponibles. Estos servidores de imágenes tienen dos funciones principales: responder peticiones de `info.json` y responder peticiones de imágenes. Más adelante en este taller vamos a instalar el [Servidor de Imágenes de IIIF Cantaloupe](https://github.com/medusa-project/cantaloupe/).

## Software de cliente de IIIF
Los clientes de IIIF son construídos para consumir servicios web de IIIF usando las especificaciones técnicas. Algunos clientes se concentran en presentar los objetos imagen mientras que otros sólo están interesados en consumir las respuestas de servidor de imágenes.
