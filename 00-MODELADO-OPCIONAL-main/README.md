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

## Cursos
Almacenarán a la temática madre y a las lecciones hijas para que así el usuario pueda ver todo de un vistazo.
En las horas de menos actividad 
- temática
- lecciones
- visualizaciones
---

## Lecciones
Almacenaran los dos niveles anteriores para así facilitar la navegación por los contenidos

### Campos nuevos
Almacena las suscripciones a las que está vinculada
- tipo_subscripcion
---

## Vídeos
Adicionalmente se añadieron a la tabla de vídeos los ancestros para así facilitar la navegación entre los contenidos superiores.

### Campos nuevos
Cada vez que un usuario termine de ver un vídeo se contabilizará una visualización más en un contador de la aplicación.

Cada 12 horas se lanzará un script para calcular las visualizaciones totales
<br>
- Visualizaciones

---

### Usuarios
- Contará con unos campos con los IDs de los cursos a los que el usuario tiene acceso, se harán las comprobaciones y gestiones de las suscripciones desde la aplicación.
<br>
- Por defecto los usuarios contarán con una suscripción llamada _pública_.

---
### Campos nuevos
##### SUBSCRIPCIONES
- Subscripciones
  - Nombre
  - Fecha suscripción

#### COMPRAS
- Cursos
---