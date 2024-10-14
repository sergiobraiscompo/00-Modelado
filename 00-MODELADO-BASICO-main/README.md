# 00-entrega_modelado

## Caso básico
## Este es el caso básico
![imagen](../Capturas/Modelado%20básico.png)

# Curso
---

## ESCRITURAS
- Se espera que no se suba más de uno o dos cursos / video al día.

- Se espera que un autor se cree como mucho una vez al día.

## LECTURAS
- Se espera una carga fuerte de lectura en página principal, lecciones y video.

## Notas extra
- En principio serán 10, ampliables a futuro hasta 1000

## Campos
### ID del curso
### Nombre del curso
### Ficha del curso

### Lecciones
- Orden
- Título de la lección
- Videos de los cursos
  - De 1 a 20 links a los vídeos por lo tanto la crearé como una arrray de strings
  - autor del vídeo
  - Ficha de la lección

- Escritura
  - Se añadirán 1 ó 2 vídeos al día

### Temáticas
Según se añada un curso se creará una temática
  - id
  - nombre temática

### Autores
Sólo recibirá los siguientes campos de la tabla autor
  - id
  - nombre del autor


# Autores
---
 Se usará el _archive pattern_ ya que rara vez se hará una visita a la página de un autor y como a futuro se esperan llegar a subir 1000 cursos seguramente el documento de autores aumente mucho de tamaño.


# Usuario
---
- id
- activo
- Cursos
  - Array de los cursos a los que está suscrito, si tiene subscreipción automáticamente estará suscrito a todos
- ¿Se podrá definir desde la aplicación si un usuario está suscrito o compre el curso?


# Página principal
---
Mostrará los últimos cursos creados en la útima semana

## ÚLTIMOS CURSOS
- Curso
  - ID curso
  - Nombre curso
  - Descripción curso