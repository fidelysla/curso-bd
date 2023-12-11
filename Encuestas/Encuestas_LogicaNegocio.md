# Encuestas

## Listado de Entidades

### encuestas **(ED)**

-   encuesta_id **(PK)**
-   nombre
-   descripcion
-   imagen
-   fecha
-   n_encuestados

### preguntas **(ED)**

-   pregunta_id **(PK)**
-   encuesta_id **(FK)**
-   pregunta

### respuestas **(ED)**

-   respuesta_id **(PK)**
-   pregunta_id **(FK)**
-   respuesta
-   es_correcta

### encuestados **(ED)**

-   encuestado_id **(PK)**
-   nombre
-   apellidos
-   edad
-   email **(UQ)**

### resultado **(ED|EP)**

-   resultado_id **(PK)**
-   encuesta_id **(FK)**
-   encuestado_id **(FK)**
-   n_preguntas
-   resp_correctas

## Relaciones

-   Una **encuesta** tiene muchas **preguntas** (_1 - M_).
-   Una **pregunta** tiene **respuestas** (_1 - M_).
-   En un **resultado** hay muchas **encuestas** (_1 - M_).
-   En un **resultado** hay muchos **encuestados** (_1 - M_).

## Diagramas

### Modelo Relacional de la BD

![]()
