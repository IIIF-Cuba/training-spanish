# Instalando un Servidor de IIIF

¡Esta es la parte del taller donde nos ensuciamos las manos con el software!

## ¿Necesito un servidor de IIIF?

¡Quizás! Una característica excelente de la API de Imagen de IIIF es que proporciona compatibilidad en múltiples niveles. Uno de estos niveles es el [nivel 0](http://iiif.io/api/image/2.1/compliance/#level-0-compliance) que soporta la capacidad de servir mosaicos estáticos a los clientes de IIIF. Así que si necesita o desea pregenerar todos sus mosaicos puede hacerlo. Software como [iiif_s3](https://github.com/cmoa/iiif_s3) o [go-iiif](https://github.com/thisisaaronland/go-iiif) para pregenerar esos mosaicos.

Por supuesto, siempre hay tradeoffs, y una razón para no hacer esto es que una gran cantidad de imágenes puede requerir demasiado espacio de almacenamiento.

## Digamos que quiere generar mosaicos al vuelo

En lugar de pregenerar todos sus mosaicos, para este taller vamos a generarlos al vuelo. Para servir nuestras imágenes, primero necesitamos instalar un servidor de IIIF. Para los propósitos de este taller, hemos decidido instalar el servidor de IIIF [Cantaloupe](https://medusa-project.github.io/cantaloupe). Hay varias razones para esto:

 - Parece ser el servidor de IIIF más "seguro para talleres" con un prerrequisito de sólo necesitar Java 8 instalado
 - La documentación es considerable
 - Es fácil de configurar
