# 00-entrega_modelado

## Caso básico

## Este es el caso básico

![imagen](../Capturas/Modelado%20básico.png)

#Lo que he tenido en cuenta
###Categorías
- En principio serán 4 pero se esperan añadir más
  - Front End
  - Devops
  - Backend
  - Otros
- ESCRITURA
  - Cuando se cree una nueva categoría
- LECTURA
  - Carga fuerte
##Entidades
### Cursos
- En principio serán 10, ampliables a futuro hasta 1000
- Cada curso contendrá:
    - Autores: 1 ó + autores creada como un array de strings
    - Lecciones será un objeto array compuesto por:
      - Nombre de la lección
        - Videos: De 1 a 20 links a los vídeos por lo tanto la crearé como una arrray de strings
        - Ficha de la lección
        - Autores:
          - Será un objeto que contendrá el id y el nombre del autor, así queda más ordenado y será más cómodo a la hora de hacer las queries.
ESCRITURAS
    - Se creará 1 curso al día
###Autores
- ESCRITURAS
  - Se añadirá 1 al día
###Videos de los cursos
- Escritura
  - Se añadirán 1 ó 2 vídeos al día
  - Carga fuerte

##*usuario*
- id
- activo
- Cursos
  - Array de los cursos a los que está suscrito, si tiene subscreipción automáticamente estará suscrito a todos
- ¿Se podrá definir desde la aplicación si un usuario está suscrito o compre el curso?

##Página principal
ULTIMOS 5 VIDEOS POR TEMATICA
  - ¿Hay que crear un campo temática o la aplicación los puede filtrar desde la tabla de cursos?
  - Puede ser que una categoría aun no tenga 5 videos