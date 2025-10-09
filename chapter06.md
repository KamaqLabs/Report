# Capítulo VI: Product Implementation, Validation & Deployment

## 6.1 Software Configuration Management

Esta sección aborda de manera detallada la gestión de configuración del software, un componente clave en el desarrollo y mantenimiento de cualquier sistema tecnológico. Su propósito principal es asegurar la integridad y trazabilidad de todos los artefactos producidos a lo largo del ciclo de vida del software, permitiendo que el equipo de desarrollo pueda trabajar de manera coordinada y estructurada. A través de políticas claras de versionado, control de cambios, definición de entornos y procedimientos estandarizados, se garantiza que cada integrante tenga acceso a configuraciones consistentes y actualizadas. Además, se establecen mecanismos para documentar y validar las modificaciones realizadas, lo que reduce significativamente la posibilidad de errores o incompatibilidades en las etapas de integración y despliegue.

La correcta implementación de una estrategia de gestión de configuración no solo mejora la calidad del producto final, sino que también optimiza la colaboración entre equipos multidisciplinarios, agiliza la detección de problemas y fortalece la estabilidad del sistema en entornos de producción.

### 6.1.1 Software Development Environment Configuration

En esta sub-sección se describe la configuración técnica del entorno de desarrollo utilizado durante el proyecto. Se especifican las herramientas de software instaladas, sus versiones, rutas de acceso y cualquier dependencia necesaria para asegurar un entorno de trabajo homogéneo para todos los miembros del equipo. Esta documentación resulta esencial para prevenir discrepancias durante la ejecución de tareas, evitar conflictos entre versiones y facilitar la incorporación de nuevos integrantes al proyecto.

Asimismo, se detallan las configuraciones iniciales requeridas para compilar, ejecutar y probar el sistema, incluyendo ajustes en IDEs, variables de entorno, gestores de paquetes, y posibles contenedores o entornos virtualizados (como Docker). Este enfoque garantiza que el entorno de desarrollo se mantenga alineado con el entorno de producción, contribuyendo a una transición fluida entre etapas de desarrollo, pruebas y despliegue.



- **Visual Studio Code**: Editor de código utilizado para desarrollar la Landing Page. Su entorno ligero, personalizable y con soporte para múltiples lenguajes facilitó la colaboración entre desarrolladores y la implementación ágil de componentes web.

<div style="text-align: center;">
  <img src="./assets/visualstudio.png" alt="Visual Studio Code" style="width:10%;"/>
</div>

- **HTML5**: Lenguaje de marcado base para estructurar el contenido de la Landing Page. Permitió organizar la información de forma semántica y accesible, mejorando la navegación y la experiencia del usuario.

<div style="text-align: center;">
  <img src="./assets/html5.png" alt="HTML 5" style="width:10%;"/>
</div>

- **CSS3**: Utilizado para aplicar estilos visuales a la Landing Page. Ayudó a mantener una identidad gráfica coherente, responsiva y atractiva, lo cual es clave para captar la atención del usuario final.

<div style="text-align: center;">
  <img src="./assets/css3.png" alt="CSS 3" style="width:10%;"/>
</div>

- **JavaScript**: Lenguaje que permitió incorporar lógica e interactividad a la Landing Page, como animaciones, validaciones y mejoras en la experiencia dinámica del usuario.

<div style="text-align: center;">
  <img src="./assets/js.png" alt="JavaScript" style="width:10%;"/>
</div>

- **GitHub**: Plataforma de control de versiones que centralizó el código del proyecto. Facilitó el trabajo colaborativo del equipo, permitió el seguimiento de cambios y mejoró la trazabilidad del desarrollo.

<div style="text-align: center;">
  <img src="./assets/github.png" alt="Github" style="width:10%;"/>
</div>

- **LucidChart**: Herramienta usada para crear diagramas de flujo, wireflows y modelos conceptuales. Contribuyó a la claridad en el diseño funcional y ayudó a definir la lógica de interacción entre pantallas y procesos.

<div style="text-align: center;">
  <img src="./assets/lucidchart.png" alt="LucidChart" style="width:10%;"/>
</div>

- **Figma**: Plataforma de diseño colaborativo utilizada para la creación de wireframes y prototipos visuales de alta fidelidad. Permitió validar la interfaz gráfica con antelación y alinear al equipo de desarrollo con la visión de diseño.

<div style="text-align: center;">
  <img src="./assets/figma.png" alt="Figma" style="width:10%;"/>
</div>

- **Android Studio**: Entorno de desarrollo para la aplicación móvil. Proporcionó las herramientas necesarias para programar, depurar, probar y empaquetar la app en dispositivos Android.

<div style="text-align: center;">
  <img src="./assets/androidstudio.png" alt="CSS 3" style="width:10%;"/>
</div>

- **Kotlin**: Lenguaje de programación moderno utilizado para desarrollar la aplicación móvil. Su sintaxis clara y concisa mejoró la eficiencia del código y la productividad del equipo, alineándose con las mejores prácticas de desarrollo en Android.

<div style="text-align: center;">
  <img src="./assets/kotilin.png" alt="Kotlin" style="width:10%;"/>
</div>

- **Trello**: Plataforma de gestión de tareas basada en tableros y tarjetas, utilizada para organizar y hacer seguimiento del progreso del equipo durante el desarrollo del proyecto. Facilitó la planificación de sprints, la asignación de responsabilidades y la visualización del avance en tiempo real, promoviendo una colaboración efectiva y una mejor administración del tiempo.

<div style="text-align: center;">
  <img src="./assets/Trello.png" alt="Trello" style="width:10%;"/>
</div>

- **Angular**: Framework de desarrollo web basado en TypeScript, empleado para construir la interfaz del panel administrativo. Su arquitectura modular, compatibilidad con APIs REST y componentes reutilizables facilitaron el desarrollo de un entorno web responsivo, escalable y mantenible.

<div style="text-align: center;"> <img src="./assets/angular.png" alt="Angular" style="width:10%;"/> </div>

- **NestJS**: Framework progresivo de Node.js utilizado para el desarrollo del backend de la plataforma. Permite estructurar los microservicios de manera modular y escalable, integrando MQTT para la comunicación IoT, REST APIs para el consumo desde Angular y Flutter, y PostgreSQL como base de datos principal.

<div style="text-align: center;"> <img src="./assets/nestjs.png" alt="NestJS" style="width:10%;"/> </div>

- **Node.js y npm**: Entorno de ejecución de JavaScript y su gestor de paquetes, utilizados para instalar dependencias y ejecutar scripts de desarrollo y despliegue tanto del frontend (Angular) como del backend (NestJS).

<div style="text-align: center;"> <img src="./assets/nodejs.png" alt="Node.js" style="width:10%;"/> </div>

- **Postman**: Herramienta de testing de APIs utilizada para validar la comunicación entre el backend y los clientes web/móvil. Permitió automatizar peticiones HTTP, gestionar entornos y realizar pruebas de integración antes del despliegue.

<div style="text-align: center;"> <img src="./assets/postman.png" alt="Postman" style="width:10%;"/> </div>

- **Git**: Sistema de control de versiones distribuido utilizado para el seguimiento de cambios y la colaboración en el código fuente del proyecto. Permitió mantener ramas independientes por módulo (web, móvil, backend) y facilitar la integración continua.

<div style="text-align: center;"> <img src="./assets/git.png" alt="Git" style="width:10%;"/> </div>


Cada una de estas herramientas fue seleccionada estratégicamente para cumplir con los objetivos del proyecto, asegurando una solución tecnológica robusta, escalable y centrada en la experiencia del usuario.

### 6.1.2 Source Code Management

**Repositorio de la Landing Page:**  
Durante el desarrollo de la Landing Page, utilizamos un repositorio centralizado en GitHub para almacenar y gestionar el código fuente del proyecto. Esto permitió el trabajo colaborativo, el control de versiones y la trazabilidad de cambios en el desarrollo.

**Implementación de GitFlow:**  
Para nuestra estrategia de gestión de versiones con Git, nos basamos en el modelo de ramificación propuesto en el artículo _“A successful Git branching model”_ de Vincent Driessen. Adoptamos el enfoque **GitFlow**, el cual proporciona una estructura clara y organizada para el desarrollo colaborativo, facilitando la integración y el mantenimiento del código.

- **Rama Principal (`main`)**: Contiene la versión estable en producción.  
- **Rama de Desarrollo (`develop`)**: Integra los últimos avances y funcionalidades en desarrollo. Actúa como entorno de integración continua.  
- **Rama de Lanzamiento (`release`)**: Utilizada para preparar una nueva versión del producto, permitiendo ajustes finales antes de su despliegue.  
  - Deriva de: `develop`  
  - Se fusiona con: `develop` y `main`  
- **Rama de Características (`feature`)**: Destinada al desarrollo de nuevas funcionalidades específicas del producto.  
  - Deriva de: `develop`  
  - Se fusiona con: `develop`  
- **Rama de Corrección Rápida (`hotfix`)**: Diseñada para aplicar soluciones urgentes a errores críticos detectados en producción.  
  - Deriva de: `main`  
  - Se fusiona con: `develop` y `main`  
- **Rama de Alcance (`scope`)**: Rama personalizada creada para gestionar desarrollos relacionados con un módulo o funcionalidad específica de gran tamaño o impacto. Su objetivo es permitir el aislamiento de tareas que abarquen múltiples ramas `feature`, mejorando la organización y facilitando su integración progresiva.  
  - Deriva de: `develop`  
  - Puede actuar como contenedor de varias `feature`  
  - Se fusiona con: `develop` o `release`, según el caso
  
<div style="text-align: center;">
  <img src="./assets/gitflow.png" alt="Ejemplo ramas Gitflow" style="width:70%;"/>
</div>

**Conventional Commits:**  
Para mantener claridad y consistencia en los mensajes de confirmación (`commits`), adoptamos la convención **Conventional Commits**, la cual estandariza la estructura semántica de cada mensaje, permitiendo una mejor comprensión del historial de cambios y una posible automatización en la generación de changelogs.

**Tipos de mensajes utilizados:**

- `feat`: Incorporación de nuevas funcionalidades.
- `fix`: Corrección de errores o bugs.
- `docs`: Cambios relacionados con la documentación.
- `style`: Ajustes de formato sin impacto funcional.
- `refactor`: Reestructuración del código sin alterar su comportamiento.
- `test`: Adición o modificación de pruebas automatizadas.
- `chore`: Tareas de mantenimiento y configuraciones del entorno.
- `perf`: Mejoras orientadas al rendimiento del sistema.    

### 6.1.3 Source Code Style Guide & Conventions

Para garantizar un código legible, consistente y de fácil mantenimiento, se adoptaron las convenciones propuestas por Google en sus guías oficiales de estilo para HTML/CSS, JavaScript y Kotlin. La aplicación de estos lineamientos facilita el trabajo colaborativo, mejora la comprensión del código entre distintos desarrolladores y reduce significativamente la probabilidad de errores durante el desarrollo y mantenimiento del sistema.

#### Convenciones para HTML/CSS (Google HTML/CSS Style Guide)

Durante la implementación de la Landing Page, se aplicaron las siguientes buenas prácticas recomendadas:

- Declarar siempre el tipo de documento (`<!DOCTYPE html>`) al inicio.
- Usar minúsculas para los nombres de los elementos HTML (`<p>`, `<h1>`, `<section>`, etc.).
- Cerrar correctamente todos los elementos HTML (por ejemplo, `<p></p>`).
- Colocar entre comillas los valores de los atributos (por ejemplo, `<div class="container">`).
- Incluir los atributos `alt`, `width` y `height` en las imágenes para accesibilidad y rendimiento.
- Evitar líneas de código excesivamente largas para facilitar la lectura.
- No omitir el elemento `<title>` dentro del `<head>`.
- Incluir `meta tags` relevantes al inicio del documento, como codificación, viewport y descripciones.

Estas convenciones aseguran una estructura semántica clara y una mejor interpretación por parte de navegadores y motores de búsqueda, además de contribuir a una experiencia de usuario coherente.

#### Convenciones para JavaScript (Google JavaScript Style Guide)

Para el desarrollo de funcionalidades interactivas con JavaScript, se aplicaron las siguientes convenciones:

- Usar notación **camelCase** para nombrar variables y funciones (por ejemplo: `numberArray`, `calculateSum()`).
- Emplear **comillas simples** para definir cadenas de texto (`'Este es un string'`).
- Finalizar todas las sentencias con punto y coma (`;`) para evitar errores de interpretación.
- Evitar el uso de `var` para declarar variables, priorizando `let` o `const` según la necesidad de reasignación.

Estas prácticas ayudan a mantener un estilo uniforme en el código fuente y previenen errores comunes relacionados con el scope, la redeclaración de variables o la gestión de valores dinámicos.

#### Convenciones para Kotlin (Google Kotlin Style Guide)

En el desarrollo de la aplicación móvil, se utilizó **Android Studio** como entorno de desarrollo, y se siguieron las convenciones oficiales para Kotlin propuestas por Google, que permiten escribir código más limpio, expresivo y seguro. Las principales directrices aplicadas fueron:

- Usar **camelCase** para variables, funciones y nombres de métodos (`userName`, `getUserData()`).
- Declarar constantes con `val` y variables mutables con `var` solo cuando sea estrictamente necesario.
- Utilizar nombres significativos, claros y descriptivos para funciones y clases.
- Omitir el punto y coma (`;`) al final de las sentencias, dado que no es necesario en Kotlin.
- Aplicar sangrías de 4 espacios y mantener una estructura clara de bloques.
- Utilizar funciones de extensión, lambdas y expresiones funcionales donde sea apropiado, siguiendo el estilo idiomático de Kotlin.
- Dividir clases largas en archivos separados para mejorar la mantenibilidad y legibilidad del código.

Estas convenciones permitieron desarrollar una aplicación Android robusta, con código fácilmente entendible y adaptable por cualquier miembro del equipo. Además, se favoreció el uso de buenas prácticas modernas en el entorno Android, alineándose con los estándares actuales de la industria.

La aplicación sistemática de estas convenciones fortaleció la calidad del código entregado en todas las capas del proyecto, promoviendo la claridad, la eficiencia y la colaboración efectiva entre los integrantes del equipo.

### 6.1.4 Software Deployment Configuration

#### Landing Page Deplyment
La Landing Page de Dedalus está desarrollada con el framework Angular, utilizando componentes modulares y estilos en Angular Material. El código fuente se mantiene dentro del repositorio `Dedalus_Landing_Page` en la organización `KamaqLabs` (GitHub).
El despliegue se realiza mediante GitHub Actions y GitHub Pages, asegurando una publicación continua (CI/CD) cada vez que se realizan cambios en la rama `develop`.

#### Flujo de Despliegue Automatizado
El proceso automatizado de despliegue está definido dentro del archivo:
`.github/workflows/deploy.yml`
![Workflow github](./assets/workflow.png)
![deploy.yml](./assets/deploy.yml.png)
Cada vez que se realiza un push hacia la rama develop, se ejecuta el flujo con las siguientes etapas:
1. Checkout del repositorio
- El flujo obtiene el código fuente desde la rama develop.
2. Configuración del entorno Node.js
- Se instala Node.js versión 20.19.0, necesaria para ejecutar Angular CLI.
3. Instalación de dependencias
- Se ejecuta el comando npm ci para instalar todas las dependencias del proyecto sin modificar el package-lock.json.
4. Compilación del proyecto Angular
- Se genera la build optimizada para producción mediante: <br>
~~~
npm run build -- --configuration production --base-href="/Dedalus_Landing_Page/"
~~~
- El resultado se almacena en el directorio:<br>
~~~
dist/LandingPage/browser/
~~~
5. Configuración de soporte de rutas
- Se copia el archivo `index.html` como `404.html` dentro de la carpeta `browser` para asegurar el correcto enrutamiento de Angular en GitHub Pages.
6. Publicación automática
- Se usa la acción `JamesIves/github-pages-deploy-action@v4` para publicar el contenido generado en la rama gh-pages.
- La configuración de GitHub Pages en el repositorio está establecida para usar `gh-pages` como rama fuente.

![github actions](./assets/gh-pages.png)

#### Resultado del despliegue 
Una vez finalizado el flujo, GitHub Pages publica automáticamente la última versión compilada del sitio en la siguiente URL: <br>
🔗 [Enlace de landing page desplegada]: https://kamaqlabs.github.io/Dedalus_Landing_Page/
                      
Este proceso elimina la necesidad de desplegar manualmente, garantizando que cada modificación aprobada en la rama `develop` se refleje directamente en la versión pública.

![Landing page deployed](./assets/landing-page-deployed.png)


## 6.2 Landing Page, Services & Applications Implementation
En esta sección se detalla el proceso completo de implementación, pruebas, documentación y despliegue de la Landing Page, los Web Services y las Aplicaciones Móviles. Abarca desde la planificación inicial hasta la entrega final, asegurando que cada componente cumpla con los requisitos establecidos y funcione correctamente.

## 6.2.1 Sprint 1
En esta sección se registra y explica el avance en términos de producto y trabajo colaborativo para el Sprint 1. Durante este sprint, el equipo se enfocará en la implementación de la Landing  y de la web application, asegurando que cumpla con los requisitos establecidos y funcione correctamente.

### 6.2.1.1 Sprint Planning 1  
En esta sección se especifican los aspectos principales del Sprint Planning Meeting. Este encuentro es fundamental para definir los objetivos y tareas del Sprint 1, asegurando que todos los miembros del equipo estén alineados y preparados para comenzar el trabajo. A continuación, se presenta un cuadro resumen del Sprint Planning Meeting, que incluye los puntos clave discutidos y las decisiones tomadas.

| **Sprint #**                       | Sprint 1                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Sprint Planning Background**     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Date                               | 2025-09-23                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Time                               | 16:00 PM                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Location                           | Google Meet Reunion                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Prepared by                        | Valentino Cervantes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Attendees (to planning meeting)    | Valentino Cervantes, Miguel Carpio, Mathias Vasquez, Gabriel Braithuaite, Sihuar Ccotarma                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Sprint n - 1 Review  Summary       | No aplica para este Sprint 1                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Sprint n - 1 Retrospective Summary | No aplica para este Sprint 1                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Sprint Goal & User Stories**     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Sprint 1 Goal                      | Our focus is on delivering the initial web presence and management interface for the Dedalus Platform, including a responsive landing page and a functional web module for administrators to manage rooms, reservations, and IoT device data. <br> We believe it delivers visibility, credibility, and early digital interaction for potential hotel clients, while providing administrators with the first version of the digital control panel for operational management. <br> This will be confirmed when the landing page is publicly accessible and administrators can successfully log in, create rooms, and visualize basic IoT sensor data from the web application. |
| Sprint 1 Velocity                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Sum of Story Points                |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |


### 6.2.1.2 Aspect Leaders and Collaborators
En esta sección se especifican los aspectos principales del Sprint Planning Meeting. Este encuentro es fundamental para definir los objetivos y tareas del Sprint 1, asegurando que todos los miembros del equipo estén alineados y preparados para comenzar el trabajo. A continuación, se presenta un cuadro resumen del Sprint Planning Meeting, que incluye los puntos clave discutidos y las decisiones tomadas.


### 6.2.1.3 Sprint Backlog 1  
En esta sección se presenta el Sprint Backlog del Sprint 1, que incluye las tareas y actividades planificadas para el desarrollo de la Landing Page y el avance de nuestro Web Application. Cada tarea está asociada a una User Story específica, lo que permite al equipo realizar un seguimiento del progreso y asegurarse de que se cumplan los objetivos del sprint.

| **Sprint #** | Sprint 1                     |                |                                          |                                                                                                                 |                       |              |        |
|--------------|------------------------------|----------------|------------------------------------------|-----------------------------------------------------------------------------------------------------------------|-----------------------|--------------|--------|
| User Story   |                              | Work Item/Task |                                          |                                                                                                                 |                       |              |        |
| Id           | Title                        | Id             | Title                                    | Description                                                                                                     | Estimation<br>(Hours) | Assined To   | Status |
| US021        | Página inicial               | WI01           | Diseñar la estructura de la Landing Page | Crear un esquema básico de la Landing Page, incluyendo secciones principales y descripción inicial del sistema. | 1                     | Valentino    | Done   |
| US022        | Sección Proyecto             | WI02           | Diseñar la sección “¿Qué es Dedalus?”    | Incluir una descripción de las características principales del sistema.                                         | 1                     | Mathias      | Done   |
| US025        | Llamada a la acción (CTA)    | WI03           | Implementar botón de "Probar ahora"      | Crear un botón que permita a los usuarios ir hacia la aplicación web.                                           | 1                     | Gabriel      | Done   |
| US026        | Sección “About the Product”  | WI04           | Diseñar la sección "About the product"   | Incluir una descripción resumida del producto y sus beneficios.                                                 | 1                     | Sihuar       | Done   |
| US027        | Sección “About the Team”     | WI05           | Diseñar la sección "About the team"      | Incluir una breve descripción de que es Dedalus.                                                                | 1                     | Miguel       | Done   |
| US024        | Sección de planes            | WI06           | Diseñar la sección "Planes de Pago"      | Incluir dos planes de suscripción con precios y características.                                                | 1                     | Miguel       | Done   |
| US028        | Sección “Miembros del grupo” | WI07           | Diseñar la sección "Miembros del grupo"  | Incluir fotos y nombres de los miembros del equipo de desarrollo.                                               | 1                     | Valentino    | Done   |
| US023        | Sección de contacto          | WI08           | Diseñar la sección "Contacto"            | Incluir un formulario de contacto con campos para nombre, correo electrónico, teléfono y mensaje.               | 1                     | Mathias      | Done   |
| US029        | Footer                       | WI09           | Diseñar el footer                        | Incluir un aviso de derechos de autor.                                                                          | 1                     | Gabriel      | Done   |

Screenshot del Sprint Backlog del Sprint 1 en Trello: 

![Sprint Backlog 1](./assets/sprint-backlog-1.png)

Enlace al Sprint Backlog del Sprint 1 en Trello: https://trello.com/c/ecIEDWCF

### 6.2.1.4 Development Evidence for Sprint Review  
En esta sección se explican y presentan los avances en la implementación de los productos de la solución según el alcance del Sprint 1. Durante este sprint, el equipo se ha enfocado en la creación y despliegue de la Landing Page, asi como el avance de nuestra Web Application.

| Repository                          | Branch  | Commit Id | Commit Message                                                                      | Commit Message Body                                                                                                                                                            | Commited on (Date) |
|-------------------------------------|---------|-----------|-------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|
| Anx0123/Dedalus_Landing_Page        | main    | 6a185d8   | Initial commit                                                                      | Initial commit with basic project structure and dependencies.                                                                                                                  | 2025-09-03         |
| KiwiAmenazante/Dedalus_Landing_Page | main    | e9fc982   | Move HTML and CSS files to new locations                                            | Renamed index.html and main.css to new paths and updated the stylesheet link in index.html to reflect the new location. This helps organize assets under the public directory. | 2025-09-2022       | 
| LordSack/Dedalus_Landing_Page       | develop | 1ef8598   | feat: change to angular project                                                     | feat: change to angular project                                                                                                                                                | 2025-09-24         |
| Gabooo04/Dedalus_Landing_Page       | develop | f994716   | feat: update GitHub Actions workflow for deploying Angular app to GitHub Pages      | feat: update GitHub Actions workflow for deploying Angular app to GitHub Pages                                                                                                 | 2025-10-06         |
| KiwiAmenazante/Dedalus-FrontEndApp  | main    | 3e7366    | feat: add dashboard route and session storage service for improved state management | feat: add dashboard route and session storage service for improved state management                                                                                            | 2025-10-05         |
| Dedalus-FrontEndApp                 | main    | 4f6dd38   | feat: updating session storage                                                      | feat: updating session storage                                                                                                                                                 | 2025-10-06         |

Enlace al repositorio: https://github.com/KamaqLabs/Dedalus_Landing_Page

### 6.2.1.5 Testing Suite Evidence for Sprint Review  
Para este sprint, no se han realizado pruebas automatizadas. Sin embargo, se han realizado pruebas manuales para asegurar que la Landing Page y la web application funcionen correctamente y cumplan con los requisitos establecidos.
Se podrían implementar pruebas automatizadas utilizando herramientas como Selenium en futuros sprints, pero por el momento, el equipo ha optado por realizar pruebas manuales para asegurar la calidad del producto.

### 6.2.1.6 Execution Evidence for Sprint Review  
En este Sprint 1, el equipo ha desarrollado y desplegado la Landing Page y la primera version de nuestra Web Application, asegurando que cumpla con los requisitos establecidos y funcione correctamente. A continuación, se presentan las evidencias de ejecución del Sprint 1, que incluyen capturas de pantalla y descripciones de las funcionalidades implementadas.

<br>**Hero Section**: La sección principal de la Landing Page, que incluye una barra de navegación, un título
atractivo, una imagen llamativa y un botón de llamada a la acción.
<br> ![Landing Page Access](/assets/LandingPageMockup1.png)
<br>**About Section**: La sección que proporciona información sobre la aplicación y sus características principales.
Incluye un título, una descripción y una imagen representativa. Además, tiene uan sección sobre el equipo de
desarrollo.
<br> ![Landing Page About Section](/assets/LandingPageMockup2.png)
<br> ![Landing Page About Team Section](/assets/LandingPageMockup3.png)
<br>**Subscriptions Section**: La sección que muestra los diferentes planes de suscripción disponibles para los
usuarios. Incluye un título, una descripción y nuestros dos planes con precios y características.
<br> ![Landing Page Subscriptions Section](/assets/LandingPageMockup4.png)
<br>**Contact Section**: La sección que permite a los usuarios ponerse en contacto con el equipo de desarrollo.
Incluye un formulario de contacto con campos para el nombre, correo electrónico y mensaje.
<br> ![Landing Page Contact Section](/assets/LandingPageMockup5.png)
<br>**Footer Section**: La sección que incluye un aviso de derechos de autor.
<br> ![Landing Page Footer Section](/assets/LandingPageMockup6.png)


Y respecto a la Web Application aqui se puede evidenciar parte del avance que hemos realizado para esta entrega:

![Web Application Evidence](/assets/Mockup1.png)
![Web Application Evidence](/assets/Mockup2.png)
![Web Application Evidence](/assets/Mockup3.png)
![Web Application Evidence](/assets/Mockup4.png)
![Web Application Evidence](/assets/Mockup5.png)


### 6.2.1.7 Services Documentation Evidence for Sprint Review  
Este sprint 1 tuvo como enfoque principal la implementación de la Landing Page y la Web Application, por lo que no se han desarrollado Web Services. La documentación de Endpoints con OpenAPI y los detalles relacionados con Web Services serán relevantes en sprints futuros cuando se aborde la implementación y documentación de estos servicios. 

### 6.2.1.8 Software Deployment Evidence for Sprint Review  
#### Software Deployment Evidence – Landing Page
Durante este Sprint se realizó el despliegue de la Landing Page oficial de la plataforma Dedalus, la cual tiene como propósito presentar la solución al público objetivo (hoteles, resorts y hospedajes boutique) y proporcionar una primera interacción digital con la marca.
El despliegue se efectuó utilizando GitHub Pages como servicio de hosting estático y GitHub Actions como herramienta de automatización continua (CI/CD).
Este proceso permitió garantizar que cada actualización en el repositorio principal se publique automáticamente en el entorno productivo, manteniendo una entrega continua y trazable del producto.
#### Pasos del proceso de Deployment
1. **Creación y configuración del repositorio** 
   - Se creó el repositorio público Dedalus_Landing_Page en GitHub para centralizar el código fuente de la landing.
   - La rama principal (develop) fue configurada como la fuente oficial de despliegue.
   - Se añadieron los archivos esenciales del proyecto (Angular / HTML-CSS / assets / config).
   - Estructura del repositorio: ![Repo Structure](/assets/repo-structure.png)
2. **Configuración de GitHub Pages**
   - En la sección Settings → Pages, se seleccionó la rama gh-pages (generada automáticamente por la acción de despliegue) como fuente del sitio.
   - Se habilitó el dominio del proyecto, generando la URL pública: https://kamaqlabs.github.io/Dedalus_Landing_Page/
   - La visibilidad se configuró como pública para permitir el acceso de los stakeholders y usuarios de prueba.
3. **Automatización mediante GitHub Actions (CI/CD)**
   - Se creó un archivo de flujo de trabajo (.github/workflows/deploy.yml) con la siguiente función:
     - Compilar automáticamente la landing page al hacer push en la rama develop.
     - Generar la carpeta dist/ optimizada para producción.
     - Publicar el contenido en la rama gh-pages de manera automática.
     - Script configurado: ![Deploy Script](/assets/deploy-script.png)
4. **Verificación del despliegue**
   - Se validó el acceso público a la landing desde el navegador.
   - Se comprobó la correcta carga de recursos (imágenes, estilos y scripts).
   - Los resultados de validación fueron satisfactorios: el sitio se muestra correctamente y con tiempo de carga óptimo.
   - Landing Page desplegada: ![Landing Page Deployed](/assets/landing-page-deployed.png)
    
### 6.2.1.9 Team Collaboration Insights during Sprint  
Para el desarrollo de este sprint, el equipo designó a un integrante para el desarrollo de las actividades de implementación de la Landing Page.

GitHub insights del landing page y Web Application:

![insights ](/assets/TeamCollaboration%20Landing.png)
![insights ](/assets/TeamCollaboration%20WebApp.png)

## 6.4 Video About-the-Product