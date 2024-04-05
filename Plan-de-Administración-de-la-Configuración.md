# Plan de Administración de la Configuración

## Elementos, herramientas y fuentes de información

A continuación, se presenta un listado de los elementos que integrarán la gestión de la configuración del proyecto "D.R.E.A.M. Lab", cada uno con su respectiva fuente de información, es decir, los sitios y documentos donde se puede encontrar la información correspondiente.

| Elementos de configuración (CIs) | Fuente de información |
| --- | --- |
| Código y librerías | [Repositorio (Git/GitHub)](https://github.com/CodeCraft-Solutions-DREAM-Lab/) |
| Documentación de la arquitectura y datos del diseño |[ Repositorio (Git/GitHub)](https://github.com/CodeCraft-Solutions-DREAM-Lab/Arquitectura) <br/> [Documento de arquitectura (GitHub)](https://github.com/CodeCraft-Solutions-DREAM-Lab/Wiki/blob/main/Documento-de-Dise%C3%B1o-de-Sistema-(SDD-IEEE-1016).md) |
| Historias de usuario | [Kanban en Notion](https://crimson-silverfish-4d1.notion.site/7ae7440495934b6fb9645943b3cc1efa?v=4b76e9385fae4bc5999616a4ebfc8568&pvs=4) |
| Ficheros de datos del producto | [Documento de Drive](https://docs.google.com/document/d/1NCXz10_kXLcwqjc1Ox1b_gTT3FTa8ONJIeBkBpCTjMI/edit?usp=sharing) |
| Requisitos | [Documento de requerimientos](https://docs.google.com/document/d/1Dzuzjha6ntMMHUa1TVPihW1_7_nco0bM6V8CRBCyTm8/edit?usp=sharing) |
| Herramientas de pruebas y scripts de pruebas | [Repositorio (Git/GitHub)](https://github.com/CodeCraft-Solutions-DREAM-Lab/) |

## Política de gestión de ramas

Se decidió tomar una política de gestión de ramas basada en historias de usuario, colocando para cada rama el “id” de su historia de usuario seguido de un nombre descriptivo corto. Por ejemplo: `HU10_ResultadosBusquedaPorVoz`

Una vez que las ramas anteriores hayan sido completadas en su totalidad, se fusionarán con los siguientes apartados:

| Rama | Descripción |
| --- | --- |
| Main | Rama principal estable. Solo se unen aquí los cambios completados y aprobados de la rama Dev al terminar un sprint, garantizando la estabilidad y la entrega de versiones funcionales. |
| Dev | Rama de desarrollo. Solo los cambios ya terminados de otras ramas se pueden unir a esta. |

## Proceso de auditoría

1. Identificación de cambios relevantes:

     a) Los miembros del equipo identifican los cambios necesarios en el proyecto y crean issues correspondientes en la sección de Issues del repositorio.

2. Desarrollo en branches:

    a) Cada miembro del equipo trabaja en una branch correspondiente a una historia de usuario para realizar los cambios propuestos.

3. Contribución y commits:

    a) Se realizan commits que siguen una estructura específica: <TIPO>: (<ALCANCE>) <MENSAJE>, donde se describen claramente los cambios efectuados.
   
    b) Se utilizan tipos de commits estándar (feat, fix, build, chore, docs, perf, revert, style, test) para categorizar los cambios

4. Creación de Pull Requests (PR):

    a) Los miembros del equipo crean Pull Requests para integrar sus cambios en la branch de desarrollo dev.

    b) En el PR se incluye una descripción detallada de los cambios realizados, utilizando un formato de viñetas.

    c) Se referencia el issue correspondiente, enlazando el número de issue (#) para un seguimiento más preciso.

5. Revisión y aprobación:

    a) Otros miembros del equipo revisan los Pull Requests y proporcionan comentarios o sugerencias para mejorarlos.

    b) Los miembros del equipo revisan y aprueban los Pull Requests antes de ser integrados a la branch de desarrollo dev.

6. Pruebas y verificación:

    a) Se realizan pruebas correspondientes para verificar que los cambios no generen errores y cumplan con los requisitos especificados.

    b) Se marca una lista de verificación en el Pull Request para asegurar que se hayan realizado todas las acciones necesarias (revisión del código, pruebas, comentarios, etc.).

7. Integración a la branch general 'main':

    a) Una vez que los cambios en la branch dev han sido probados y revisados satisfactoriamente, se realiza el merge a la branch general main.

    b) Este merge debe contar con la aprobación de la mayoría de los miembros del equipo.

8. Seguimiento y documentación:

    a) Se lleva un seguimiento de los cambios realizados en el proyecto mediante el registro de issues, Pull Requests y commits.

    b) Se documentan los cambios significativos en la sección de documentación del proyecto.
