# **Personajes Dragon Ball**

## **Listado de Entidades**

### personajes **(ED)**

-   personaje_id **(PK)**
-   nombre
-   apellido
-   fecha de nacimiento
-   sexo **(FK)**
-   ocupacion **(FK)**
-   idioma **(FK)**
-   origen **(FK)**
-   especie **(FK)**
-   nivel_poder **(FK)**

### sexos **(EC)**

-   sexos_id **(PK)**
-   nombre **(UQ)**

### ocupaciones **(EC)**

-   ocupacion_id **(PK)**
-   nombre **(UQ)**

### origenes **(EP)**

-   origen_id **(PK)**
-   planeta **(FK)**
-   universo **(FK)**

### idiomas **(EC)**

-   idioma_id **(PK)**
-   nombre **(UQ)**

### planetas **(EC)**

-   planeta_id **(PK)**
-   nombre **(UQ)**
-   descripcion

### universo **(EC)**

-   universo_id **(PK)**
-   nombre **(UQ)**

### especies **(EC)**

-   especie_id **(PK)**
-   nombre **(UQ)**

### niveles_poder **(EC)**

-   nivel_poder_id **(PK)**
-   nombre **(UQ)**

## **Relaciones**

1. Un **personaje** _tiene_ un solo **sexo** (_1 a 1_).
1. Un **personaje** _tiene_ un **origen** (_1 a 1_).
1. Un **personaje** puede _tener_ muchos **idiomas** (_1 a M_).
1. Un **personaje** _tiene_ un **origen** (_1 a 1_).
1. Un **personaje** _pertenece_ a una **especie** (_1 a 1_).
1. Un **personaje** _tiene_ un **nivel_poder** (_1 a 1_).
1. Un **personaje** _tiene_ una **ocupacion** (_1 a 1_).

## **Diagrama**

### Modelo Relacional de la BD

![Prueba](/personajesDB/PersonajesModeloRelacionalDB.jpg)
_Modelo Relacional sujeto a errores_

## **Reglas de Negocio**

### personajes

1. Crear el registro de un personaje
1. Leer el registro de un(os) personaje(s) dada una condición en particular.
1. Leer todos los registros de la entidad personajes.
1. Actualizar los datos de un personaje dada una condición en particular.
1. Eliminar los datos de un personaje dada una condición en particular.

### sexos

1. Crear el registro de un sexo, solo deberán ser Masculino o Femenino
1. Leer el registro de un(os) sexo(s) dada una condición en particular.
1. Leer todos los registros de la entidad sexos.
1. Actualizar el dato de un sexo dada una condición en particular.
1. Eliminar los datos de un sexo dada una condición en particular.

### ocupaciones

1. Crear el registro de una ocupación
1. Leer el registro de una(s) ocupacion(es) dada una condición en particular.
1. Leer todos los registros de la entidad ocupaciones.
1. Actualizar los datos de una carrera dada una condición en particular.
1. Eliminar los datos de una carrera dada una condición en particular.

### origenes

### idiomas

### planetas

### universo

### especies

### niveles_poder
