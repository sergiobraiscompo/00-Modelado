# 00-entrega_modelado

## Caso básico

## Este es el caso opcional

![imagen](../Capturas/Modelado%20opcional.png)

#Lo que he tenido en cuenta
###Jerarquía
Como mucho contará con 3 niveles
- Temática > Curso >> Lección
- Ejemplo:
  Front End > React >> Testing

# Temática
- Mostrará los cursos hijos para evitar la carga de lecciones.

# Cursos
- Almacenarán al padre.
- Almacenarán las lecciones hijas para que así el usuario pueda ver todo de un vistazo.

# Lecciones
- Almacenaran los dos niveles anteriores para así facilitar la navegación por los contenidos.

# Vídeos
- Adicionalmente se añadieron a la tabla de vídeos los ancestros para así facilitar la navegación entre estos.

# Usuarios
## Campos nuevos
- SUBCRIPCIONES
  - Activa
  - Contenidos []
    - Cursos
    - Lecciones

- COMPRAS
  - Contenidos []
      - Cursos
      - Lecciones