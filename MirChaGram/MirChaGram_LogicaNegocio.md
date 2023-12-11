# MirChaGram

## Listado de Entidades

### posts **(ED)**

-   post_id **(PK)**
-   post_date
-   plot
-   photo
-   user **(FK)**

### user **(ED)**

-   user **(PK)**
-   user_date
-   user_name
-   email **(UQ)**
-   password
-   phone **(UQ)**
-   bio
-   web
-   avatar
-   birthdate
-   genre
-   country **(FK)**

### comments **(ED|EP)**

-   comment_id **(PK)**
-   comment_date
-   comment
-   post_id **(FK)**
-   user **(FK)**

### hearts **(ED|EP)**

-   heart_id **(PK)**
-   heart_date
-   post_id **(FK)**
-   user **(FK)**

### follows **(ED|EP)**

-   follow_id **(PK)**
-   follow_date
-   follow_user **(FK)**
-   user **(FK)**

### countries **(EC)**

-   country_id **(PK)**
-   country_name

## Relaciones

1.  Un **user** tiene muchos (publican) **posts** _(1 - M)_.
1.  Un **user** tiene **country** _(1 - M)_.
1.  Un **user** hace muchos **comments** _(1 - M)_.
1.  Un **post** tiene muchos **comments** _(1 - M)_.
1.  Un **user** da un **heart** _(1 - 1)_.
1.  Un **post** tiene muchos **heart** _(1 - M)_.
1.  Un **user** tiene muchos **follows** _(1 - M)_.
1.  Un **user** siguen a muchos **follows** _(1 - M)_.

## Diagramas

### Modelo Relacional de la BD
