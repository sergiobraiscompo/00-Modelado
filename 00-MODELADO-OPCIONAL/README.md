# 00-entrega_modelado

## Caso básico

## Este es el caso opcional

![imagen](../Capturas/Modelado%20opcional.png)

# Jerarquía
Como mucho contará con 3 niveles
- Temática > Curso >> Lección
- Ejemplo:
  Front End > React >> Testing

---

## Temática
Contendrá a los cursos hijos
- Cursos
---

## Curso
Almacenarán a la _temática madre_ y los nombres de las _lecciones hijas_ para que así el usuario pueda ver todo de un vistazo.

Se usará el _computed pattern_ para contabilziar las visualizaciones de los videos del curso
Cada dia de madrugada se lanzará un script que recoge las visualizaciones de todos los videos del curso.

Habrá un campo que almacene las suscricpiones que dan acceso al curso por defecto tendrán una con id _0_ que sería de acceso público

### Campos nuevos
- parent
- children
- lecciones
- vistas_videos
- suscripciones
---

## Lecciones
Almacenarán los dos niveles superiores de la jerarquía para así facilitar la navegación por los contenidos

Almacenará las suscripciones a las que está vinculada dan acceso al curso por defecto tendrán una con id _0_ que sería de acceso público

### Campos nuevos
- ancestors
- children
- suscripciones
---

## Vídeos
Cada vez que un usuario termine de ver un vídeo se contabilizará una visualización más en un contador de la aplicación.
Cada 12 horas se lanzará un script para sumar y escribir las visualizaciones totales

### Campos nuevos
- vistas

---

### Usuarios
Se harán las comprobaciones y gestiones de las suscripciones desde la aplicación.
Por defecto los usuarios contarán con una suscripción con id _0_ que sería de acceso público

### Campos nuevos
##### SUBSCRIPCIONES
- Subscripciones
  - id
  - Fecha_alta

#### COMPRAS
- Cursos

#### Datos bancarios
- numero_tarjeta
- fecha de caducidad
- nombre del titular
---