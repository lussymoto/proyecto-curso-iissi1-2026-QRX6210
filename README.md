# Título Proyecto

## Miembros del grupo L3-ABS-6

1. García Cabeza, Lucía
1. Mao, Yanxi
1. Farahat, Amal
1. Gaitán Severo, Jorge

## 1. Introducción al problema

- Descripción del problema para poner en contexto el proyecto, incluyendo información sobre los clientes y usuarios, la situación actual, problemas, expectativas, etc. Se valorará la presencia de información multimedia (fotos, gráficos, documentos escaneados, etc.).

## 2. Glosario de términos

- Términos específicos del dominio del problema, ordenados alfabéticamente. Se valorará la presencia de información multimedia.
  - Fanfic (Fan-fiction): Historia ficticia escrita por fans sobre otra historia ficticia; ya sea sobre una serie, película, cómic, etc...
  - Escritor: Usuario que publica fanfics.
  - Lector: Usuario que lee fanfics y/o publica comentarios e hilos.
  - Fandom: La comunidad de fans detrás de un fenómeno, obra, artista, serie, película, videojuego o personalidad específica.
  - Tag: Etiqueta que identifica una característica de un fanfic.
  - Hilo: Espacio de discursión e intercambio de opiniones sobre un fanfic.

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

#### R.G.04. Valorar Historias

Como lector,
quiero poder comentar las historias, 
para compartir mi opinión.

### 3.2. Usuarios del sistema

Tenemos solo un tipo de usuario. Éste puede escribir y/o leer fanfics.

## 4. Catálogo de requisitos

### 4.1. Requisitos funcionales

#### R.F.01. Comentarios por capítulo

Como lector,
quiero poder escribir y leer comentarios en los capítulos de un fanfic,
para expresar mi opinión públicamente sobre cada capítulo por separado.

#### R.F.02. Seguir a escritores

Como lector,
quiero poder seguir a escritores que me gusten,
para recibir recomendaciones sobre sus historias.

#### R.F.03. Notificar novedades

Como usuario,
quiero recibir una notificación cuando alguien a quien sigo suba un fanfic nueva o cuando se actualice un fanfic que estoy leyendo.

#### R.F.04. Búsqueda avanzada

Como usuario,
quiero poder realizar búsquedas en el sistema con distintos filtros y criterios de ordenación,
para encontrar con más facilidad lo que estoy buscando.

#### R.F.05. Recomendaciones

Como lector,
quiero recibir recomendaciones por el sistema de fanfics, escritores, fandoms e hilos que podrían gustarme en base a mi actividad en la página,
para tener una experiencia personalizada que facilite descubrir partes de la página que me gusten.

#### R.F.06. Fanfics Favoritos 

Como lector,
quiero poder marcar fanfics como favoritos y acceder a ellos en su propia pestaña,
para encontrarlos más fácilmente y recibir recomendaciones en base a ellos.

#### R.F.07. Crear Hilos 

Como lector,
quiero poder abrir un hilo sobre un fanfic que he leído,
para crear un espacio en el que hablar sobre un tema de interés del fanfic.

#### R.F.08. Guardar Hilos 

Como usuario,
quiero poder guardar los hilos que me interesen,
para archivarlos y poder encontrarlos más tarde.

#### R.F.09. Ajustes de Notificaciones

Como usuario,
quiero poder editar la frecuencia con la que recibo notificaciones
para modificar mi experiencia en el sistema.

#### R.F.10. Tags

Como escritor,
quiero poder añadir tags a los fanfics que escriba,
para que los lectores puedan encontrar mi contenido en base a búsquedas avanzadas.


**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- Se debe aplicar la regla de negocio R.N.XX.
- ...

**R.F.01. Comentarios por capítulo**

-Se publica un comentario en un capítulo y aparece correctamente.

-Se entra en un capítulo con comentarios y se pueden leer.

-Se intenta publicar un comentario vacío y aparece un mensaje de error.

**R.F.02. Seguir a escritores**

-Se sigue a un escritor y aparece en la lista de escritores seguidos.

-Se deja de seguir a un escritor y desaparece de la lista.

-Se intenta seguir dos veces al mismo escritor y solo aparece una vez.

**R.F.03. Notificar novedades**

-Un escritor seguido publica un fanfic nuevo y el usuario recibe una notificación.

-Se actualiza un fanfic que el usuario está leyendo y recibe una notificación.

-Un escritor que no sigue el usuario publica un fanfic y no recibe una notificación.

**R.F.04. Búsqueda avanzada**

-Se realiza una búsqueda con un filtro y aparecen los resultados que cumplen ese filtro.

-Se utilizan varios filtros y los resultados cumplen todos ellos.

-Se ordenan los resultados y aparecen en el orden elegido.

**R.F.05. Recomendaciones**

-Se consultan varios fanfics y el sistema muestra recomendaciones relacionadas.

-Se siguen escritores y sus historias aparecen en las recomendaciones.

-Se marcan fanfics como favoritos y se tienen en cuenta para las recomendaciones.

**R.F.06. Fanfics favoritos**

-Se marca un fanfic como favorito y aparece en la pestaña de favoritos.

-Se quita un fanfic de favoritos y desaparece de la pestaña.

-Se intenta añadir dos veces el mismo fanfic a favoritos y solo aparece una vez.

**R.F.07. Crear hilos**

-Se crea un hilo sobre un fanfic y aparece asociado a ese fanfic.

-Se entra en un fanfic y se pueden ver los hilos creados sobre él.

-Se intenta crear un hilo sin rellenar los datos necesarios y aparece un mensaje de error.

**R.F.08. Guardar hilos**

-Se guarda un hilo y aparece en la lista de hilos guardados.

-Se elimina un hilo guardado y desaparece de la lista.

-Se cierra y vuelve a abrir la sesión y los hilos guardados siguen apareciendo.

**R.F.09. Ajustes de notificaciones**

-Se cambia la frecuencia de las notificaciones y se guarda correctamente.

-Se desactivan las notificaciones y el usuario deja de recibirlas.

-Se vuelven a activar las notificaciones y el usuario las recibe de nuevo.

**R.F.10. Tags**

-Se añaden tags a un fanfic y aparecen correctamente.

-Se busca un fanfic mediante uno de sus tags y aparece en los resultados.

-Se elimina un tag y el fanfic deja de aparecer al buscar por ese tag.

#### 4.1.1. Requisitos de información

##### R.I. Título requisito de información

Como [tipo de usuario]
quiero [servicio]
para [razón]

#### R.I.01. Información de los fanfics 

Como lector, 
quiero disponer de la siguiente información sobre los fanfics:

-Título del fanfic

-Descripción

-Autor

-Fandom al que pertenece

-Tags asociados

-Fecha de publicación

-Número de capítulos

-Estado del fanfic (en curso o finalizado)

#### R.I.02. Información de los usuarios 

Como usuario, 
quiero disponer de la siguiente información relacionada con mi cuenta:

-Nombre de usuario

-Contraseña

-Fanfics publicados

-Fanfics favoritos

-Escritores seguidos

-Hilos guardados

#### R.I.03. Información de los capítulos

Como lector, 
quiero disponer de la siguiente información sobre los capítulos de un fanfic:

-Título del capítulo

-Número de capítulo

-Contenido

-Fecha de publicación

-Comentarios realizados en el capítulo

#### R.I.04. Información de los hilos

Como lector, 
quiero disponer de la siguiente información sobre los hilos:

-Título del hilo

-Usuario que lo ha creado

-Fanfic relacionado

-Contenido

-Fecha de creación

-Respuestas de otros usuarios

**Prueba de aceptación**
- Descripción de la primera comprobación a realizar
- Descripción de la segunda comprobación a realizar
- ...

**R.I.01. Información de los fanfics**
-Se crea un fanfic y se comprueba que aparecen su título, descripción, autor y fandom.

-Se añaden tags a un fanfic y aparecen correctamente.

-Se comprueba que aparecen la fecha de publicación, el número de capítulos y si el fanfic está en curso o finalizado.

**R.I.02. Información de los usuarios**

-Se crea una cuenta y se comprueba que aparecen correctamente el nombre de usuario y la contraseña.

-Se publican y se marcan fanfics como favoritos y aparecen en la información del usuario.

-Se sigue a un escritor y se guarda un hilo, y ambos aparecen en la información del usuario.

**R.I.03. Información de los capítulos**

-Se crea un capítulo y aparecen su título, número, contenido y fecha de publicación.

-Se añaden comentarios a un capítulo y aparecen asociados a ese capítulo.

-Se modifican los datos de un capítulo y se comprueba que la información mostrada se actualiza correctamente.

**R.I.04. Información de los hilos**

-Se crea un hilo y aparecen su título, usuario que lo creó, fanfic relacionado, contenido y fecha.

-Se añaden respuestas a un hilo y aparecen correctamente.

-Se consulta un hilo y se comprueba que toda la información aparece asociada al fanfic correspondiente.

#### 4.1.2. Reglas de negocio

##### R.N.01. Permisos sin registrarse

Un usuario debe estar registrado con una cuenta para poder publicar fanfics, hilos y comentarios. Sin una cuenta, sólo se les permite leerlos.

##### R.N.02. Número de cuentas por correo

Un mismo correo electrónico tiene derecho a crear una única cuenta. 

##### R.N.03. Número de fanfics por usuario

Un usuario puede crear publicar distintos fanfics, pero un fanfic no puede tener más de un autor.

##### R.N.04. Conservación de fanfics

Si un usuario borra su cuenta, los fanfics que ha creado no son borrados.

##### R.N.05. Capítulos vacíos

Un capítulo no puede publicarse si está vacío, en cuyo caso, el fanfic sólo acualizará el resto de cambios realizados.


### 4.2. Mapa de historias de usuario (opcional)

### 4.3. Requisitos no funcionales (opcional)

**R.N.F. Título requisito no funcional**
Como [tipo de usuario]
quiero [servicio]
para [razón]

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


