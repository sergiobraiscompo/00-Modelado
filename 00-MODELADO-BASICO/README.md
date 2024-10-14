# 00-entrega_modelado

## Caso básico
## Este es el caso básico
![imagen](../Capturas/Modelado%20básico.png)

# Curso
---

## ESCRITURAS
- Se espera que no se suba más de uno o dos cursos / video al día
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
Será un objeto con la explicación de la lección y un array de vídeos
Los autores de la lección vendrán de los autores de los vídeos
Se actualizarán cada vez que se suba un vídeo
- Orden
- Título de la lección
- Autores
- Videos de los cursos
  - De 1 a 20 links a los vídeos por lo tanto la crearé como una arrray de strings
  - autor del vídeo

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
 contará con un array de cursos obtenido de la tabla homónima
 Los enlaces serán un array de objetos conun link y un nombre para el recurso
- id
- nombre
- biografia
- cursos
- enlaces extra
  - link
  - recurso
 


# Usuario
---
- id
- activo
- nombre
- correo


# Página principal
---
Mostrará los últimos cursos creados en la útima semana agrupados por temática
Se usará un _bucket pattern_ para almacenar los últimos cursos usando el campo de fecha

## Novedades
- Curso
  - ID curso
  - Nombre curso
  - Descripción curso