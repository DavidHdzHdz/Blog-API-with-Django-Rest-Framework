# Base para la API de un blog.

La Api se compone de dos partes, la parte grafica que nos permite una facil administración de nuestro blog
y la Api como tal.

### Parte grafica:
### API yservicios:

* Servicio para **obtener posts**, buscar por frases y ordenarlos:
  
  * Ruta para **listar post**:
   ```
  http://url/api/post/
  ```
    el cual devuelve un json así:
  ```json
  {
    "count": 4,
    "next": null,
    "previous": null,
    "results": 
    [
        {
            "url": "http://localhost:8000/api/posts/my-title/",
            "user": {
                "username": "abc",
                "email": "",
                "first_name": "",
                "last_name": ""
            },
            "title": "my title",
            "image": "http://localhost:8000/media/7/Screen_Shot_2016-04-26_at_1.34.15_PM.png",
            "content": "asdfasdfasd",
            "publish": "2016-04-01"
         }
     ]        
    }    
  ```
  * Para realizar busquedas en los post se agrega el parametro ?search=string_buscado,
    por ejemplo para buscar gatos sería:
    ```
    http://url/api/posts/?search=gatos
    ```
  
  

* Servicio para **subir imagenes**:

  * la rutas de las imágenes de portada para los articulos se guardan de la siguiente manera:
  ```
  http://url/media/id_media/nombre_img/
  ```
  * por ejemplo si la cover img del articulo de id 2 se llama cochorro.png se guardaría en:  
  ```
  http://url/media/2/cachorro.png/
  ```
    *nota si un post no tiene foto de portada el id_media sería id_post -1 y así ucesicvamente.*
  
  
