# FLUJOS DE TRABAJO
## Ejercicio 1
El flujo de trabajo del grupo “SUMMI DEVS” estará básicamente conformado por dos ramas principales lo que son: “Main” y “Develop”
Los integrantes del grupo dentro la rama “Develop” serán donde crearán nuevas ramas y contribuirán al proyecto con creación de otras subramas de acuerdo a las tareas asignadas. Por ejemplo, si algún integrante esta encargado de hacer el diseño de la pagina home, entonces se creara una nueva rama dentro de “develop” y la nueva rama será nombrada con el nombre del autor y nombre de la tarea, por ejemplo:
- >**$ git switch -c Javier-home**
Para la realizar la integración de los cambios del proyecto estará a cargo de Miguel Zubieta, quien será responsable de realizar el merge desde la rama “develop”. Cuando el proyecto se encuentra en la fase final y se hayan hecho todas las pruebas, entonces se realizarán el merge desde la rama “main” para integrar todos los cambios correctos y como finalización del proyecto que es la creación de un Blog.
## Ejercicio 2
Para la creación de una nueva rama se utilizarán los siguientes comandos:
- >**$ git switch develop**
- >**$ git switch -c feature-nueva**
- >**$ git add .**
- >**$ git commit -m “Adición de una nueva funcionalidad de acuerdo al ejercicio 2 del flujo de trabajo”**
- >**$ git push origin feature-nueva**

Como prueba de la realización del ejercicio se adjuntas las siguientes imágenes:
![ejercicio 2 del flujo de trabajo](/src/img/Flujo%20de%20trabajo%202.png)

Una vez que se haya subido los cambios al repositorio remoto se procede a crear un pull request para su posterior revisión.
![creacion de PR](/src/img/creacion%20PR.png)


## Ejercicio 3
Cuando se presenta un conflicto durante una fusión de ramas en el proyecto como primer paso se debe identificar dicho conflicto, al ingresar los comandos para fusionar ramas nos saltara un error, indicando el conflicto. Se debe modificar o eliminar el archivo para poder resolver el conflicto. Al corregir los errores se debe ingresar el comando de **git add** Dicho comando guardara los cambios y los archivos pasaran al área de stagging. Se debe completar el cambio con un commit describiendo con un comentario la corrección de los errores de la fusión.

Se finaliza la fusión con el comando de **git merge**, en caso de que no ocurra ningún error o existiera algún conflicto en la fusión de ramas, el proceso se completara de manera correcta. Como último paso se recomienda realizar pruebas adicionales para asegurar que la fusión no presente ningún problema en el futuro o que se haya introducido algún error.

En caso de que se fusione a otra rama que no sea el main, se debe realizar un paso extra el cual se debe fusionar desde la rama main la rama que va a fusionarse utilizando el comando de **git merge**.
