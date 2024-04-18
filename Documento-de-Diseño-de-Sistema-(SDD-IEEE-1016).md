## 1. Introducción

### 1.1 Propósito

El propósito de este documento es proporcionar una explicación detallada de los diversos componentes que conforman la aplicación web del "D.R.E.A.M. Lab". Esto incluye una cobertura completa de sus funcionalidades, arquitectura, atributos de calidad, escalabilidad, entre otros aspectos importantes. Está dirigido a stakeholders y miembros del equipo de desarrollo de la consultoría CodeCraft Solutions. Por lo tanto, se incluye un lenguaje técnico acompañado de un diccionario aclaratorio para abreviaturas y tecnicismos.

### 1.2 Alcance

El documento proporciona una descripción exhaustiva de la aplicación "D.R.E.A.M. Lab", abarcando sus funcionalidades de reservación, sistema de voz, administración y video wall, diseñadas tanto para computadoras como para dispositivos móviles. En su versión actual, el escrito presenta la arquitectura básica del proyecto mediante un diagrama claro y conciso, mismo que viene acompañado de la descripción de los componentes y su funcionamiento; esto para proporcionar una comprensión integral del sistema.

Además, se incluyen las pantallas preliminares del mockup, las cuales han sido desarrolladas utilizando la herramienta Figma. Estas pantallas ofrecen una visualización anticipada de la interfaz de usuario y facilitan la comprensión de la experiencia que tendrán las personas al interactuar con la aplicación.

Por último, el documento aborda los atributos de calidad del sistema, que son usabilidad, seguridad y mantenibilidad. Cada uno de estos aspectos es detalladamente explicado, resaltando los criterios que serán considerados durante la fase de desarrollo del proyecto. Este enfoque garantiza que la aplicación no solo cumpla con las expectativas funcionales, sino que también sea fácil de usar, segura y mantenible a largo plazo.

### 1.3 Definiciones, Acrónimos y Abreviaturas

* **Sprint:** Periodo de tiempo definido, típicamente de 1 a 4 semanas, durante el cual se realizan un conjunto de tareas preestablecidas.
* **Backlog:** Listado de las tareas y funcionalidades a desarrollar durante el proyecto.
* **Base de datos (BD):** Espacio virtual donde se almacena, maneja y accede a información organizada de forma estructurada. 
* **Caso de prueba:** Descripción detallada de cómo comprobar el correcto funcionamiento de un proceso o característica en un desarrollo de software. * Involucra pasos, entradas, y resultados esperados. 
* **Application Programming Interface (API):** Conjunto de protocolos y reglas que permiten que diferentes aplicaciones se comuniquen entre sí. 
* **Microservicios:** Tipo de arquitectura de software que involucra el desarrollo de una aplicación como un grupo de servicios independientes que se comunican entre sí mediante APIs.
* **Cascading Style Sheets (CSS):** Lenguaje de programación enfocado a la creación de recursos visuales en páginas web (colores, diseños, fuentes).
* **Hypertext Markup Language (HTML):** Lenguaje utilizado para la creación de páginas web. Permite definir la estructura básica de un sitio mediante objetos y etiquetas.
* **JavaScript:** Lenguaje de programación de alto nivel utilizado para agregar funcionalidad e interactividad a los sitios web.


### 1.4 Referencias

Listar todos los documentos referenciados en el SDD. Incluir títulos y fechas de publicación.

### 1.5 Resumen

Ofrecer un resumen del SDD, incluyendo las principales decisiones de diseño y arquitectura que se detallarán en el documento.

## 2. Descripción General del Sistema

### 2.1 Perspectiva del Producto

Explicar cómo se integra el sistema en un entorno más amplio. Identificar los sistemas/límites de interfaz.

### 2.2 Funciones del Producto

Resumir las principales funciones que el sistema debe realizar o a las que debe contribuir.

### 2.3 Características y Restricciones del Usuario

Describir las características demográficas y las restricciones de los usuarios finales.

### 2.4 Suposiciones y Dependencias

Enumerar cualquier suposición hecha durante el diseño del sistema y cualquier dependencia externa.

## 3. Diseño de la Arquitectura

### 3.1 Representación Arquitectónica

A continuación, se muestra un diagrama que ilustra la interconexión de los distintos componentes de la aplicación web.

Diagrama de componentes

![Diagrama de la arquitectura](https://raw.githubusercontent.com/CodeCraft-Solutions-DREAM-Lab/Wiki/main/assets/DiagramaArquitectura.png)

**Descripción del diagrama:** El usuario accede a la aplicación del D.R.E.A.M. Lab desde su computadora o dispositivo móvil. Una vez dentro, puede interactuar con diversas pantallas del front-end, como la de inicio de sesión, el menú de experiencias y el sistema de reservas. Cada una de estas pantallas se comunica con el backend para procesar las solicitudes del usuario. Estas solicitudes son atendidas mediante consultas a la base de datos, permitiendo al usuario visualizar información como descripciones de los espacios disponibles y horarios. 

Además, el back-end se conecta con un componente de inteligencia artificial para abordar solicitudes especiales, como la priorización de usuarios en sus procesos de reserva, y la generación de recomendaciones personalizadas.


### 3.2 Descomposición del Sistema

Detallar la descomposición del sistema en subsistemas y componentes, incluyendo una descripción de la funcionalidad de cada uno.

### 3.3 Diseño de la Interfaz
| Vista            | Enlace                            |
|------------------|-----------------------------------|
| Alumno (PC)      | [https://n9.cl/l8bd4](https://n9.cl/l8bd4)  |
| Profesor (PC)    | [https://n9.cl/b09nl](https://n9.cl/b09nl)  |
| Administrador (PC) | [https://n9.cl/7boin](https://n9.cl/7boin)  |
| Vista móvil      | [https://n9.cl/54fvk](https://n9.cl/54fvk)  |
| Vista del video wall | [https://shorturl.at/esDZ1](https://shorturl.at/esDZ1) |

### 3.4 Diseño de Datos

Detallar el diseño de la estructura de datos, incluyendo modelos de datos, diagramas de entidad-relación y cualquier consideración de persistencia de datos.

#### 3.4.1 Modelo Entidad-Relación

![Modelo Entidad-Relacion de la base de datos](https://raw.githubusercontent.com/CodeCraft-Solutions-DREAM-Lab/Wiki/main/assets/DiagramaBDEntidadRelacion.png)

#### 3.4.1 Diagrama Relacional

![Diagrama Relacional de la base de datos](https://github.com/CodeCraft-Solutions-DREAM-Lab/Wiki/blob/main/assets/DiagramaBDRelacional.png)

## 4. Detalles del Diseño

### 4.1 Detalles de los Componentes del Sistema

Descripción de componentes:

* **Front-end:** Interfaz gráfica con la que los usuarios interactúan y realizan peticiones a la aplicación. Esta involucra aspectos visuales como son colores, animaciones, y fondos. Este está desarrollado principalmente con React debido a su estructura modular que facilita la creación y mantenimiento de componentes reutilizables. 

* **Back-end:** Aspectos lógicos que permiten que la aplicación funcione. Involucra el manejo de solicitudes, el procesamiento de información, así como la interacción con la base de datos y otros componentes. Este está basado en Node.js debido a su capacidad de manejar múltiples conexiones simultáneas de manera eficiente. 

* **Inteligencia artificial (IA):** Componente encargado de manejar el sistema de prioridad y asignación de espacios, así como la realización de recomendaciones para cada usuario, esto tanto dentro del menú de experiencias como en el módulo de asistencia con voz. El apartado de voz trabaja con el servicio de OpenAI para mejorar la interacción con el usuario y brindar una experiencia más inmersiva. 

* **Base de datos (BD):** Espacio virtual donde se almacena, maneja y accede a información de forma estructurada. Aquí se encuentran las credenciales de acceso, información de las experiencias y espacios, así como datos sobre las reservaciones y sus estados. La base de datos es de carácter relacional y está fabricada con Azure SQL.

* **Testing:** Componente para la ejecución de pruebas. Este tiene un sistema de interacción con las pantallas del front-end para examinar su correcto funcionamiento. 

### 4.2 Detalles de la Interfaz del Usuario

A continuación se presenta un diagrama con las interacciones y flujos de la aplicación:

![Diagrama de interacciones y flujos](https://raw.githubusercontent.com/CodeCraft-Solutions-DREAM-Lab/Wiki/main/assets/Interacciones%26Flujos.png)

## 5. Atributos de Calidad del Sistema

### 5.1 Usabilidad

* **Investigación de usuarios:** Se llevará a cabo una investigación exhaustiva de los usuarios potenciales de la aplicación para comprender sus necesidades, preferencias y comportamientos. Esto incluirá la realización de entrevistas, encuestas y pruebas de usabilidad para obtener información valiosa sobre cómo mejorar la experiencia del usuario.

* **Diseño centrado en el usuario:** Se seguirán los principios del diseño centrado en el usuario para garantizar que la aplicación satisfaga las necesidades y expectativas de los usuarios finales. Se desarrollarán prototipos y wireframes iterativos que se someterán a pruebas de usabilidad con usuarios reales para validar y refinar el diseño.

* **Intuitividad y simplicidad:** Se priorizará la simplicidad y la claridad en el diseño de la interfaz de usuario, asegurándose de que las funciones principales sean fácilmente accesibles y comprensibles para los usuarios sin la necesidad de instrucciones adicionales. Se evitarán la sobrecarga de información y las interfaces complicadas que puedan abrumar a los usuarios.

* **Feedback y mejora continua:** Se establecerá un sistema para recopilar y analizar el feedback de los usuarios sobre la aplicación, incluyendo comentarios, sugerencias y quejas. Este feedback se utilizará para identificar áreas de mejora y realizar ajustes en el diseño y la funcionalidad de la aplicación de manera continua.

* **Accesibilidad:** Se asegurará de que la aplicación sea accesible para todos los usuarios, incluyendo aquellos con discapacidades físicas o cognitivas. Se seguirán las pautas de accesibilidad web y se realizarán pruebas de accesibilidad para garantizar que la aplicación cumpla con los estándares de accesibilidad establecidos.

### 5.2 Seguridad

La seguridad de la aplicación se abordará con las siguientes medidas específicas:

* **Control de acceso basado en roles:** Se establecerán roles de usuario con permisos específicos para acceder a diferentes funcionalidades de la aplicación, garantizando así que solo los usuarios autorizados puedan realizar ciertas acciones.

* **Encriptación de datos:** Todos los datos sensibles, como contraseñas y datos de tarjetas de crédito, se almacenarán en la base de datos utilizando algoritmos de encriptación robustos para protegerlos contra accesos no autorizados.

### 5.3 Mantenibilidad

Para facilitar la mantenibilidad del sistema, se seguirán las siguientes prácticas:

* **Principios de diseño limpio:** Se escribirá código limpio y bien estructurado siguiendo los principios de SOLID y DRY, lo que facilitará la comprensión y modificación del código en el futuro.

* **Documentación exhaustiva:** Se documentarán todas las decisiones de diseño, así como el funcionamiento interno de los componentes del sistema, para facilitar la comprensión y el mantenimiento por parte de futuros desarrolladores.

* **Pruebas automatizadas:** Se implementarán pruebas unitarias y de integración exhaustivas para detectar y corregir errores de manera eficiente, garantizando así la estabilidad y fiabilidad del sistema a lo largo del tiempo.

### 5.4 Otras Consideraciones

Además de los atributos de calidad mencionados anteriormente, se abordarán otras consideraciones relevantes para el éxito general del proyecto:

* **Fiabilidad y Disponibilidad Continua:** Se implementará un sistema de monitoreo proactivo para detectar cualquier anomalía en el funcionamiento del sistema y tomar medidas correctivas de manera inmediata. Además, se establecerán procedimientos de respaldo y recuperación de datos para garantizar la continuidad del servicio en caso de fallas inesperadas.

* **Escalabilidad y Flexibilidad:** El diseño del sistema se enfocará en permitir su escalabilidad y adaptabilidad a medida que crezca el número de usuarios y la complejidad de las operaciones. Se utilizarán arquitecturas y tecnologías que permitan una fácil escalabilidad horizontal y vertical, así como la incorporación de nuevas funcionalidades y componentes sin interrupciones en el servicio.

## 6. Otros

### 6.1 Problemas Abiertos

Identificar y discutir cualquier problema de diseño que permanezca sin resolver o que requiera decisiones futuras.

### 6.2 Riesgos y Mitigaciones

Enumerar los riesgos identificados para el proyecto de diseño y las estrategias para mitigarlos.

### 6.3 Planes Futuros

Esbozar cualquier trabajo futuro previsto para el diseño o desarrollo del sistema.

### 6.4 Apéndices

Incluir cualquier información adicional relevante, como glosarios, índices y registros de revisiones del documento.
