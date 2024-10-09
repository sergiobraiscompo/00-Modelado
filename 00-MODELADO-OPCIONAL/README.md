# 00-entrega_modelado

## Caso básico

## Este es el caso opcional

![imagen](../Capturas/Modelado%20opcional.png)

#Lo que he tenido en cuenta
###Jerarquía
Como mucho contará con 4 niveles
- Temática > Curso >> Lección >>> Videos
- Ejemplo:
  Front End > React >> Testing >>> video_test.mp4

# Temática
- Mostrará los cursos hijos para evitar la carga de lecciones.

# Cursos
- Almacenarán al padre.
- Almacenarán las lecciones hijas para que así el usuario pueda ver todo de un vistazo.

# Lecciones
- Almacenará tpdos sus ancestros para así facilitar la navegación por los contenidos.

# Vídeos
- Adicionalmente se añadieron a la tabla de vídeos los ancestros para así facilitar la navegación entre estos.

# Usuarios
Se han creado 2 campos nuevos para gestionar el material accesible
___SUBCRIPCIONES___
  - Activa
  - Contenidos []
    - Cursos
    - Lecciones

___COMPRAS___
  - Contenidos []
      - Cursos
      - Lecciones