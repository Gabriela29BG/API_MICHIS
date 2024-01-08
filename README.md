# API_MICHIS
Este código se centra en interactuar con la API de The Cat API para mostrar imágenes de gatos de forma aleatoria, permitir a los usuarios guardar sus imágenes favoritas y visualizarlas. Aquí tienes un resumen de las funcionalidades clave:

1. **Carga de Gatos Aleatorios:**
   - Se utiliza la función `loadRandomMichis` para obtener imágenes de gatos aleatorios de la API.
   - Si la respuesta es exitosa, se actualizan las imágenes y se asignan funciones a los botones asociados.

2. **Carga de Michis Favoritos:**
   - Utiliza la función `loadFavouriteMichis` para obtener las imágenes de gatos guardadas como favoritas.
   - Se crea una sección en el documento para mostrar los michis favoritos.
   - Cada michi favorito se presenta con su imagen y un botón para eliminarlo de la lista de favoritos.

3. **Guardado de Michis Favoritos:**
   - La función `saveFavouriteMichi` permite guardar un michi como favorito.
   - Utiliza el método `POST` para enviar la solicitud a la API y actualizar la lista de favoritos.

4. **Eliminación de Michis Favoritos:**
   - La función `deleteFavouriteMichi` elimina un michi de la lista de favoritos.
   - Utiliza el método `DELETE` para enviar la solicitud correspondiente a la API.

5. **Manejo de Errores:**
   - En caso de que ocurra un error en alguna de las solicitudes a la API, se actualiza un elemento del DOM (`spanError`) con un mensaje de error.

Este proyecto utiliza fetch para realizar solicitudes a la API, gestionando así la carga de imágenes aleatorias y la manipulación de la lista de michis favoritos. Además, hace uso de eventos de clic en los botones para realizar acciones como guardar o eliminar imágenes.
