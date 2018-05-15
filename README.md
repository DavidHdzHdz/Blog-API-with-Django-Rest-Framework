# Base para la API de un blog.

La Api se compone de dos partes, la parte grafica que nos permite una facil administración de nuestro blog
y la Api como tal.

### Parte grafica:
### API yservicios:

* Servicio para **obtener posts**, buscar por frases y ordenarlos:

  

* Servicio para **subir imagenes**:

  la rutas de las imágenes de portada para los articulos se guardan de la siguiente manera:
  ```
  http://url/media/id_post/nombre_img
  ```
  por ejemplo si la cover img del articulo de id 2 se llama cochorro.png se guardaría en:  
  ```
  http://url/media/2/cachorro.png
  ```
