# Kogacat

## Miembros del grupo L3-ABS-6

1. García Cabeza, Lucía
1. Mao, Yanxi
1. Farahat, Amal
1. Gaitán Severo, Jorge

## 1. Introducción al problema

Cuando se trata de preservar historias, suele ser la fama de la propia obra la que se encarga de que no se olvide. Sin embargo, la cantidad de fanfics que pueden surgir a partir de una historia puede ser enorme, facilitando que muchos de ellos se pierdan en la abundancia de la nube. Nuestro objetivo es conservar todos y cada uno de ellos, aportando las herramientas suficientes para descubrir o encontrar justo el fanfic que uno está buscando.
Nuestros usuarios incluyen a cualquiera que disfrute con la lectura, escritura o discusión de fanfics.

**Prototipo de la Interfaz (estructura)**

<img width="700" alt="Proyecto IISSI1_page-0001" src="https://github.com/user-attachments/assets/d94e4d36-d1d6-4258-b2fb-a7035e35034a" />

Esperamos organizar los servicios ofrecidos en una barra vertical a la izquierda, con la siguiente jerarquía:

- Home: Apartado para descubrir fanfics
- Biblioteca: Espacio para visualizar los fanfics que el usuario:
  - quiere leer
  - está leyendo
  - ha terminado de leer
  - ha marcado como favoritos
- Comunidad: Contiene los espacios para acceder a:
  - Escritores
  - Fandoms
  - Hilos

<table>
  <tr>
    <th>Los fanfics que este ha escrito el usuario se guardan por separado:</th>
    <th>Interfaz esperada para la lectura de un fanfic:</th>
  </tr>
  <tr>
    <td><img width="600" alt="Proyecto IISSI1_page-0003" src="https://github.com/user-attachments/assets/fc91b561-c687-46a8-b115-68686795e44a" /></td>
    <td><img width="600" alt="Proyecto IISSI1_page-0009" src="https://github.com/user-attachments/assets/2cbfefcd-4a49-4fbb-b101-a7ffd3443f41" /></td>
  </tr>
</table>


## 2. Glosario de términos 

(Ordenados alfabéticamente)

- Comentario: Valoración u opinión sobre el capítulo de un fanfic.
- Crítico: Usuario que escribe comentarios o hilos y/o responde a ellos.
- Escritor: Usuario que publica fanfics.
- Fandom: Un tag de carácter obligatorio. Indica la comunidad de fans detrás de un fenómeno, obra, artista, serie, película, videojuego o personalidad específica.
- Fanfic (Fan-fiction): Historia ficticia escrita por fans sobre otra historia ficticia; ya sea sobre una serie, película, cómic, etc...
- Hilo: Espacio de discursión e intercambio de opiniones sobre un fanfic.
- Lector: Usuario que lee fanfics y/o publica comentarios e hilos.
- Tag: Etiqueta que identifica una característica de un fanfic.

## 3. Visión general del sistema

### 3.1. Requisitos generales

#### R.G.01. Crear y Publicar Historias

Como escritor,
quiero poder crear y publicar mis propias historias,
para que otros usuarios puedan leerlas.

#### R.G.02. Leer Historias

Como usuario,
quiero poder leer historias publicadas por otros usuarios,
para ver de diferentes tipos de contenido.

#### R.G.03. Buscar y Guardar Historias

Como lector,
quiero poder encontrar historias que me interesen y guardarlas,
para poder leerlas más tarde.

#### R.G.04. Comentar Historias

Como lector,
quiero poder comentar las historias, 
para compartir mi opinión.

### 3.2. Usuarios del sistema

Tenemos solo un tipo de usuario, el cual puede adoptar distintos roles simultáneamente, dependiendo de lo que busque del servicio en ese momento.
- Lector:
Aquellos interesados en leer obras de otros usuarios.
- Escritor:
Aquellos interesados en crear y publicar sus propias obras.
- Crítico:
Aquellos interesados en la discusión de obras y en expresar su opinión sobre ellas.

Todos estos pueden ser un mismo usuario, aunque entendemos que un crítico también debe ser un lector a la fuerza.

## 4. Catálogo de requisitos

### 4.1. Requisitos funcionales

#### R.F.01. Comentarios por capítulo

Como lector,
quiero poder escribir y leer comentarios en los capítulos de un fanfic,
para expresar mi opinión públicamente sobre cada capítulo por separado.

**Prueba de aceptación**
- Se publica un comentario en un capítulo y aparece correctamente.
- Se entra en un capítulo con comentarios y se pueden leer.
- Se intenta publicar un comentario vacío y aparece un mensaje de error.

#### R.F.02. Seguir a escritores

Como lector,
quiero poder seguir a escritores que me gusten,
para recibir recomendaciones sobre sus historias.

**Prueba de aceptación**
- Se sigue a un escritor y aparece en la lista de escritores seguidos.
- Se deja de seguir a un escritor y desaparece de la lista.
- Se intenta seguir dos veces al mismo escritor y solo aparece una vez.

#### R.F.03. Notificar novedades

Como usuario,
quiero recibir una notificación cuando alguien a quien sigo suba un fanfic nuevo o cuando se actualice un fanfic que estoy leyendo.

**Prueba de aceptación**
- Un escritor seguido publica un fanfic nuevo y el usuario recibe una notificación.
- Se actualiza un fanfic que el usuario está leyendo y recibe una notificación.
- Un escritor que no sigue el usuario publica un fanfic y no recibe una notificación.

#### R.F.04. Búsqueda avanzada

Como usuario,
quiero poder realizar búsquedas en el sistema con distintos filtros y criterios de ordenación,
para encontrar con más facilidad lo que estoy buscando.

**Prueba de aceptación**
- Se realiza una búsqueda con un filtro y aparecen únicamente los resultados que cumplen ese filtro.
- Se utilizan varios filtros y todos los resultados cumplen todos ellos.
- Se ordenan los resultados y aparecen en el orden elegido.

#### R.F.05. Recomendaciones

Como lector,
quiero recibir recomendaciones por parte del sistema, sobre fanfics, escritores, fandoms e hilos que podrían gustarme en base a mi actividad en la página,
para tener una experiencia personalizada que facilite descubrir partes de la página que me gusten.

**Prueba de aceptación**
- Se consultan varios fanfics y el sistema muestra recomendaciones relacionadas.
- Se siguen escritores y sus historias aparecen en las recomendaciones.
- Se marca un nuevo fanfic como favorito y se actualizan las recomendaciones.

#### R.F.06. Fanfics Favoritos 

Como lector,
quiero poder marcar fanfics como favoritos y acceder a ellos en su propia pestaña,
para encontrarlos más fácilmente y recibir recomendaciones en base a ellos.

**Prueba de aceptación**
- Se marca un fanfic como favorito y aparece en la pestaña de favoritos.
- Se quita un fanfic de favoritos y desaparece de la pestaña.
- Se intenta añadir dos veces el mismo fanfic a favoritos y solo aparece una vez.

#### R.F.07. Crear Hilos 

Como lector,
quiero poder abrir un hilo sobre un fanfic que he leído,
para crear un espacio en el que hablar sobre un tema de interés del fanfic.

**Prueba de aceptación**
- Se crea un hilo sobre un fanfic y aparece asociado a ese fanfic.
- Se entra en un fanfic y se pueden ver los hilos creados sobre él.
- Se intenta crear un hilo sin asociarlo a un fanfic y aparece un mensaje de error.

#### R.F.08. Guardado de Hilos 

Como usuario,
quiero poder guardar los hilos que me interesen,
para archivarlos y poder encontrarlos más tarde.

**Prueba de aceptación**
- Se guarda un hilo y aparece en la lista de hilos guardados.
- Se elimina un hilo guardado y desaparece de la lista.
- Se cierra y vuelve a abrir la sesión y los hilos guardados siguen apareciendo.

#### R.F.09. Ajustes de Notificaciones

Como usuario,
quiero poder editar la frecuencia con la que recibo notificaciones
para modificar mi experiencia en el sistema.

**Prueba de aceptación**
- Se cambia la frecuencia de las notificaciones y se guarda correctamente.
- Se desactivan las notificaciones y el usuario deja de recibirlas.
- Se vuelven a activar las notificaciones y el usuario las recibe de nuevo.

#### R.F.10. Añadir y Quitar Tags

Como escritor,
quiero poder añadir tags a los fanfics que escriba,
para que los lectores puedan encontrar mi contenido en base a búsquedas avanzadas.

**Prueba de aceptación**
- Se añaden tags a un fanfic y aparecen correctamente.
- Se busca un fanfic mediante uno de sus tags y aparece en los resultados.
- Se elimina un tag y el fanfic deja de aparecer al buscar por ese tag.

#### R.F.11. Crear Tags

Como escritor,
quiero poder crear tags que no existan actualmente,
para expandir los posibles criterios de búsqueda y filtrado de la página.

**Prueba de aceptación**
- Se intenta crear un tag que ya existe y no se permite.
- Se crea un tag y a otros escritores les aparece como un tag existente.

#### 4.1.1. Requisitos de información

##### R.I.01. Información fanfics 

Como lector, 
quiero disponer de la siguiente información sobre los fanfics:

- Título del fanfic
- Descripción
- Autor
- Fandom al que pertenece
- Tags asociados (personajes, género y tags adicionales)
- Fecha de publicación
- Estado del fanfic (en curso o finalizado)
- Número de capítulos actual
- Capítulos que contenga

**Prueba de aceptación**
- Se abre un fanfic y aparecen su título, autor, descripción, fandom y tags asociados, seguido de sus capítulos.
- Se crea un fanfic y automáticamente aparece en la lista de fanfics creados por ese usuario y en la lista de fanfics que pertenecen a su fandom asociado.
- Se añaden tags a un fanfic y el fanfic aparece en la lista de fanfics con ese tag.
- Se elimina algún tag del fanfic y este desaparece de la lista de fanfics con ese tag.
- Se comprueba que aparecen la fecha de publicación, el número de capítulos y si el fanfic está en curso o finalizado.

##### R.I.02. Información usuarios 

Como usuario, 
quiero disponer de la siguiente información relacionada con mi cuenta:

- Nombre de usuario
- Contraseña
- Fanfics publicados por mí
- Fanfics de mi biblioteca
- Por cada fanfic de mi biblioteca:
  - Si está sin leer, en proceso, o leído
  - Si está marcado como favorito o no
- Escritores seguidos
- Hilos guardados

**Prueba de aceptación**
- Se crea una cuenta y se comprueba que aparecen correctamente el nombre de usuario y la contraseña.
- Se publican y se marcan fanfics como favoritos y aparecen en la información del usuario.
- Se sigue a un escritor y se guarda un hilo, y ambos aparecen en la información del usuario.

##### R.I.03. Información capítulos de un fanfic

Como lector, 
quiero disponer de la siguiente información sobre los capítulos de un fanfic:

- Título del capítulo
- Número de capítulo
- Contenido
- Fecha de publicación
- Comentarios realizados en el capítulo

**Prueba de aceptación**
- Se crea un capítulo y aparecen su título, número, contenido y fecha de publicación.
- Se añaden comentarios a un capítulo y aparecen asociados a ese capítulo.
- Se modifican los datos de un capítulo y se comprueba que la información mostrada se actualiza correctamente.

##### R.I.04. Información de los hilos

Como lector, 
quiero disponer de la siguiente información sobre los hilos de un fanfic:

- Título del hilo
- Usuario que lo ha creado
- Fanfic relacionado
- Contenido
- Fecha de creación
- Respuestas de otros usuarios

**Prueba de aceptación**
- Se crea un hilo y aparecen su título, usuario que lo creó, fanfic relacionado, contenido y fecha.
- Se añaden respuestas a un hilo y aparecen correctamente.
- Se consulta un hilo y se comprueba que toda la información aparece asociada al fanfic correspondiente.

##### R.I.04. Información de los comentarios

Como lector,
quiero disponer de la siguiente información sobre los comentarios de un capítulo:

- Usuario que lo ha escrito
- Contenido
- Fanfic del capítulo asociado
- Si ha sido editado o no

**Prueba de aceptación**
- Se crea un comentario y aparece en la lista de comentarios escritos por ese usuario.
- Se elimina un comentario y deja de aparecer la lista de comentarios escritos por ese usuario y la lista de comentarios del capítulo.
- Se edita un comentario y aparece como editado

#### 4.1.2. Reglas de negocio

##### R.N.01. Permisos sin registrarse

Como desarrollador de la página,
quiero que un usuario que no esté registrado sólo pueda actuar como lector,
para que no se puedan publica fanfics, hilos y comentarios sin asociarlos a una cuenta.

##### R.N.02. Número de cuentas por correo

Como desarrollador de la página,
quiero que un mismo correo electrónico no pueda crear más de una cuenta.

##### R.N.03. Creación de capítulos en orden

Como desarrollador de la página,
quiero que el número de un capítulo no pueda ser mayor a la cantidad de capítulos que tiene el fanfic,
para que todos los capítulos publicados sean consecutivos.

##### R.N.04. Conservación de fanfics

Como desarrollador de la página,
quiero que un usuario sólo pueda borrar un fanfic que ha escrito si ese fanfic no se encuentra en la biblioteca de ningún otro usuario,
para evitar que los usuarios pierdan acceso a fanfics que ya conocían.

##### R.N.05. Capítulos vacíos

Como desarrollador de la página,
quiero que no se puedan publicar fanfics con capítulos vacíos, ni editar un capítulo para vaciarlo.

##### R.N.06. Requisitos para Publicar Fanfics

Como desarrollador de la página,
quiero que un fanfic no pueda publicarse sin tener un título y al menos un fandom asociado.

### 4.2. Mapa de historias de usuario (opcional)

### 4.3. Requisitos no funcionales (opcional)

**R.N.F.01. Tiempo de respuesta**

Como lector, 
quiero que la página cargue rápidamente,
para no tener que esperar demasiado al buscar o leer fanfics.

**R.N.F.02. Disponibilidad**

Como escritor, 
quiero que la página esté disponible la mayor parte del tiempo, 
para poder publicar y actualizar mis fanfics cuando quiera.

**R.N.F.03. Seguridad**

Como usuario,
quiero que mi cuenta y contraseña estén protegidas, 
para evitar que otras personas puedan acceder a mi cuenta.

**R.N.F.04. Compatibilidad**

Como lector, 
quiero poder utilizar la página desde diferentes navegadores, 
para poder leer fanfics independientemente del navegador que utilice.

-- fin entregable 1 --

## 5. Modelo conceptual

### 5.1. Diagramas de clases UML

- con restricciones.

### 5.2. Escenarios de prueba

- con descripción textual y diagrama de objetos UML.

## 6. Matrices de trazabilidad

- Matriz de trazabilidad entre los elementos del modelo conceptual y los requisitos.

|       | EntidadX   | AsociaciónX  | RestricciónX  | Entidad2 ...   | 
|:------|:-----------|:-----------|:-----------|:-----------|
| RI-1  | X          | X          | X          | X          |
| RI-2  |            | X          |            | X          |
| RF-1  |            | X          |            | X          |
| RF-2  | X          |            | X          | X          |
| RN-1  |            | X          |            |            |
| RN-2  | X          | X          | X          |            |
| ...   |            |            |            |            |

-- fin entregable 2 --

## 7. Modelo relacional en 3FN

- Relaciones obtenidas al aplicar la transformación del modelo conceptual.

### 7.1.  Justificación de la estrategia de transformación de jerarquías

- si se identificaron jerarquías en el MC.


### 8. Matriz de trazabilidad MC/SQL (opcional):

- Restricciones sobre el MC / Elementos del modelo tecnológico (SQL) (Triggers, checks, etc.)
- Incluir Reglas de negocio — Constraints/Triggers en las matrices de trazabilidad para el entregable 3

|       | EntidadX   | AsociaciónX  | RestricciónX  | Entidad2 ...   | 
|:-------|:-------|:-------|:-------|:-------|
| TABLA-1 |        |        |        |        |
| TABLA-2 |        |        |        |        |
| TABLA-3 |        |        |        |        |
| TABLA-4 |        |        |        |        |
| TRIG-1 |        |        |        |        |
| TRIG-2 | X      | X      |        | X      |
| TRIG-3 |        | X      |        | X      |
| TRIG-4 |        |        | X      |        |
| CONST-1 |        |        |        |        |
| CONST-2 | X      | X      |        | X      |
| CONST-3 |        | X      |        | X      |
| CONST-4 |        |        | X      |        |

Se consideran todo tipo de constraints declarativas (aquellas definidas durante el CREATE TABLE).
-- fin entregable 3 --

## Referencias


