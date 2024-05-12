# Git Blog 

| Team:             | **Summit Devs**   |
|-------------------|-------------------|
| **Workflow:**     | **Git Flow**      |

## Bitacora del Proyecto
  Desarrollamos un blog con [Astro](astro.build) y decidimos usar Git Flow como flujo de trabajo por su facilidad para comprender el flujo de las ramas y la protección que existe a la rama main para evitar llevar errores a producción.
  No se tuvieron problemas mayores, todo el equipo trabajo bien.
  Tampoco hubieron conflictos pero si se realizo un revert, lo realizo Miguel que junto dos features en un sola rama por error al tratar de hacer merge.

## Buenas y malas practicas
En general todo el equipo uso buenas practicas, no hubo ningun problema entre los que desarrollamos el trabajo, entre las buenas practicas esta el uso de un buen flujo de trabajo, commits con buena redacción, uso de pull requests para integrar los cambios, uso de hooks, etc.
  ### Cecilia (revisión por Javier)
  ### Javier (revisión por Miguel)
  ### Miguel (revisión por Cecilia)
## Git hooks o Git alias

  Se uso `simple git hooks` y `bumpp` para el manejo de hooks, usamos un hook precommit para ejecutar eslint y solucionar errores con el linter, con bumpp nos encargamos del lanzamiento de versiones.
