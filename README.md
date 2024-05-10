# SUMMIT DEVS

## Índice

1. [Introducción](#introducción)
2. [Herramientas Utilizadas](#herramientas-utilizadas)
3. [Comandos](#comandos)
4. [Flujos de Trabajo](#flujos-de-trabajo)
5. [Buenas Prácticas en Git](#buenas-prácticas-en-git)
6. [Deshacer Cambios](#deshacer-cambios)
7. [Truquitos Pros en Git](#truquitos-pros-en-git)

## Introducción
Bienvenidos al repositorio del proyecto de blog de Summit Devs. Este proyecto es una plataforma web estática desarrollada usando el framework Astro, destinada a compartir conocimientos y experiencias a través de contenidos educativos enfocados en tecnología. El blog cuenta con varias secciones incluyendo Home, About —que detalla quiénes somos y nuestros objetivos—, y un Blog, donde lanzamos posts sobre temas como la historia de Linux, historia de Git y buenas prácticas en Git.

[Tutorial blog ASTRO](https://docs.astro.build/es/basics/project-structure/)


## Herramientas Utilizadas

🚀 Para el desarrollo de este proyecto, estamos utilizando varias herramientas clave que facilitan la creación y mantenimiento del blog:


**Astro:** Un framework moderno para construir sitios web estáticos de alto rendimiento.

**Visual Studio Code:** Nuestro editor de código recomendado, optimizado para Astro con una extensión oficial que mejora la experiencia de desarrollo.

**Node.js:** Utilizamos Node.js para manejar diversas dependencias y scripts necesarios para el proyecto. Las versiones compatibles son 18.17.1 y 20.3.0 o superior, excluyendo la versión 19 que no es soportada.


## Comandos

🧞 Todos los comandos deben ejecutarse desde la raíz del proyecto, desde una terminal:

| Comando                   | Acción                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Instala las dependencias                         |
| `npm run dev`             | Inicia el servidor local de desarrollo en `localhost:4321` |
| `npm run preview`         | Previsualiza tu construcción localmente, antes de desplegarla |
| `npm run astro -- --help` | Obtén ayuda sobre cómo usar la CLI de Astro      |

## Flujos de Trabajo
## Buenas Prácticas en Git

Trabajar con Git en un proyecto colaborativo implica seguir ciertas buenas prácticas para mantener el repositorio organizado y facilitar la colaboración entre los miembros del equipo.

**1. Nombres descriptivos y consistentes para las ramas:**

Utilizar nombres de ramas que reflejen claramente el propósito de los cambios es importnte.

Ejemplo: <pre>**feature/nombre-del-feature**
feature/about
feature/home
feature/oliver-posts
</pre>
**2. Mensajes de commit claros y concisos:**

 Cada commit debe tener un mensaje que explique claramente qué cambios se han realizado y por qué. Los mensajes de commit deben comenzar con una línea resumen breve (idealmente menos de 50 caracteres), seguida de una descripción más detallada si es necesario. Esto facilita la revisión de la historia del proyecto y la búsqueda de cambios específicos.

Ejemplo:<pre>
 * Commit Inicial, iniciando proyecto con astro
 * Add: carpeta img y change[about]:En la introduccion
 * fix[about]: Resolviendo error de la dirección de la imagen
 * Change[README]:Add introduccion, herramientas utilizadas
 * fix[posts]: Quitando comentarios para usar el post layout
 </pre>

**3. Integración frecuente de cambios:**

 Es importante integrar tus cambios regularmente con la rama principal o de desarrollo para evitar conflictos masivos y difíciles de resolver. La integración continua también permite que el equipo detecte problemas temprano y asegure que las características se integren de manera efectiva y cohesiva en el producto final.

**4. Uso de pull requests y merges planificados:**

 Utiliza pull requests para fusionar cambios en las ramas principales. Esto permite discutir los cambios propuestos en un contexto claramente definido y realizar modificaciones antes de que los cambios sean parte de la rama principal. Además, es recomendable que las fusiones sean realizadas después de que al menos una o más personas revisen y aprueben los cambios.

 ### ¿Qué es .gitignore?

 El archivo **.gitignore** es una lista que le dice a Git cuáles archivos del proyecto no debe guardar en el historial de versiones. Esto es útil para mantener fuera del repositorio archivos que no necesitas compartir, como configuraciones personales, contraseñas o archivos temporales que tu computadora crea automáticamente. Al usar .gitignore, puedes ayudar a que tu proyecto sea más limpio y seguro, asegurándote de que solo los archivos importantes sean rastreados y compartidos con otros.

### ¿Cómo crear y configurar un archivo .gitignore
 * **Crear el archivo .gitignore**
 * **Especificar patrones de archivos para ignorar**
 * **Guardar y cerrar el archivo:**

    Una vez que hayas terminado de añadir las reglas, guarda y cierra el archivo.
* **Añadir .gitignore al repositorio:**

    Es importante que el archivo .gitignore mismo sea parte del repositorio, para que las mismas reglas se apliquen en todos los entornos de trabajo. Añádelo a tu repositorio con:
    <pre>git add .gitignore
git commit -m "Add .gitignore"
git push</pre>

### Implementación de la Gestión de Versiones Semántica (SemVer) en un Proyecto Git con Astro
**Cómo etiquetar versiones en Git:**
* Asegúrarse de que todos los cambios estén confirmados y que el repositorio esté limpio.
* Utilizar el comando de Git para crear una etiqueta:<pre> git tag -a v1.0.0 -m "Release version 1.0.0"
</pre>
*Aquí, v1.0.0 es la versión que estás publicando y el mensaje después de -m debe ser descriptivo de los cambios realizados.*
* Empujar la etiqueta a tu repositorio remoto:
  <pre>git push origin v1.0.0</pre>

Al implementar SemVer junto con buenas prácticas de control de versiones y despliegue continuo, se puede mejorar significativamente la gestión y la predictibilidad de los lanzamientos en el proyecto de blog Astro, asegurandonos que las actualizaciones sean siempre claras y controladas.

## Deshacer Cambios
## Truquitos Pros en Git