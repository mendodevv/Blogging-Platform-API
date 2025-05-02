# roadmap-project
Template for a roadmap-project


> [!NOTE]
> Este proyecto es obtenido de la página de <a href="https://roadmap.sh/projects/blogging-platform-api">roadmap.sh</a>

## Soluciones hechas por la comunidad
|Usuario|Repositorio| Documentación |
|-------|-----------|---------|
| <a href="https://github.com/EGAMAGZ">EGAMAGZ</a> |<a href="https://github.com/EGAMAGZ/Blogging-Platform-API">Repositorio</a> | N/A |

# Mi solución
En este proyecto, se creó una API REST que nos permite realizar operaciones CRUD (Create, Read, Update, Delete) para una plataforma de blogging.
Los requerimientos fueron los siguientes:
- Crear una nueva publicación de blog
- Actualizar una publicación de blog existente
- Eliminar una publicación de blog existente
- Obtener una sola publicación de blog
- Obtener todas las publicaciones de blog
- Filtrar publicaciones de blog por un término de búsqueda

## Tecnologías utilizadas:
- Java 21
- Springboot 3.4.5
- MySQL 8.0
- IntelliJ IDEA 2024.2.3
- Maven
- Spring Data JPA
- Spring Validation
- Spring Web
- Jakarta Validation
- Flyaway
- Lombok
- SpringDoc OpenAPI
- Insomnia

## Base de Datos
Para la base de datos, se crearon dos tablas, la primera es la de los post, la cuál contiene
- Título del post
- Contenido del post
- Categoría del post
- Fecha de creación
- Fecha de actualización
El usuario solo ingresará los primeros 3 campos, ya que la fecha de creación y actualización del post es manejada enteramente por el Backend de la aplicación.

La segunda es la tabla de los tags, la cual contiene:
- Nombre del tag
- ID del post/posts a los que está asociado el tag

## Funcionamiento de la aplicación
## Como hacer funcionar la aplicación?
Para poder correr esta aplicación, deberás contar con un IDE para Java (De preferencia IntelliJ) y Java 21 instalado.
1. Clona el repositorio en tu PC
2. Crear una base de datos en MySql (El nombre queda a tu elección)
3. Configura las credenciales de la base de datos en el archivo ```application.properties```
     - En IntelliJ, ve a Run -> Edit Configurations -> Environment Variables
     - Ya ahí, agrega las variables del ```application.properties``` (DB_NAME, DB_USERNAME y DB_URL) y para su valor, pon los de tu base de datos
4. Una vez agregadas las variables de entorno, corre la aplicación
5. Para poder probar los endpoints, entra a ```http://localhost:8080/swagger-ui/index.html#/```
