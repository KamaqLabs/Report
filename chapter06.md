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



### 6.2.1.2 Aspect Leaders and Collaborators
En esta sección se especifican los aspectos principales del Sprint Planning Meeting. Este encuentro es fundamental para definir los objetivos y tareas del Sprint 1, asegurando que todos los miembros del equipo estén alineados y preparados para comenzar el trabajo. A continuación, se presenta un cuadro resumen del Sprint Planning Meeting, que incluye los puntos clave discutidos y las decisiones tomadas.


### 6.2.1.3 Sprint Backlog 1  
En esta sección se presenta el Sprint Backlog del Sprint 1, que incluye las tareas y actividades planificadas para el desarrollo de la Landing Page. Cada tarea está asociada a una User Story específica, lo que permite al equipo realizar un seguimiento del progreso y asegurarse de que se cumplan los objetivos del sprint.

Screenshot del Sprint Backlog del Sprint 1 en Trello: 


### 6.2.1.4 Development Evidence for Sprint Review  
En esta sección se explican y presentan los avances en la implementación de los productos de la solución según el alcance del Sprint 1. Durante este sprint, el equipo se ha enfocado en la creación y despliegue de la Landing Page

| Repository             | Branch | Commit Id | Commit Message       | Commit Message Body                                                     | Commited on (Date) |
|------------------------|--------|-----------|----------------------|-------------------------------------------------------------------------|--------------------|

Enlace al repositorio: 
### 6.2.1.5 Testing Suite Evidence for Sprint Review  
Para este sprint, no se han realizado pruebas automatizadas, ya que el equipo ha decidido enfocarse en la implementación de la Landing Page y no se han desarrollado pruebas unitarias o de integración. Sin embargo, se han realizado pruebas manuales para asegurar que la Landing Page funcione correctamente y cumpla con los requisitos establecidos.
Se podrían implementar pruebas automatizadas utilizando herramientas como Selenium en futuros sprints, pero por el momento, el equipo ha optado por realizar pruebas manuales para asegurar la calidad del producto.

### 6.2.1.6 Execution Evidence for Sprint Review  
En este Sprint 1, el equipo ha desarrollado y desplegado la Landing Page, asegurando que cumpla con los requisitos establecidos y funcione correctamente. A continuación, se presentan las evidencias de ejecución del Sprint 1, que incluyen capturas de pantalla y descripciones de las funcionalidades implementadas.

<br>**Hero Section**: La sección principal de la Landing Page, que incluye una barra de navegación, un título
atractivo, una imagen llamativa y un botón de llamada a la acción.
<br> ![Landing Page Access](./assets/landing_page_access.png)
<br>**About Section**: La sección que proporciona información sobre la aplicación y sus características principales.
Incluye un título, una descripción y una imagen representativa. Además, tiene uan sección sobre el equipo de
desarrollo.
<br> ![Landing Page About Section](./assets/landing_page_about_section.png)
<br> ![Landing Page About Team Section](./assets/landing_page_about_team_section.png)
<br>**Subscriptions Section**: La sección que muestra los diferentes planes de suscripción disponibles para los
usuarios. Incluye un título, una descripción y nuestros dos planes con precios y características.
<br> ![Landing Page Subscriptions Section](./assets/landing_page_subscriptions_section.png)
<br>**Customers Section**: La sección que muestra los clientes actuales de la aplicación. Incluye un título y una
descripción de nuestros dos segmentos objetivos.
<br> ![Landing Page Customers Section](./assets/landing_page_customers_section.png)
<br>**Contact Section**: La sección que permite a los usuarios ponerse en contacto con el equipo de desarrollo.
Incluye un formulario de contacto con campos para el nombre, correo electrónico y mensaje.
<br> ![Landing Page Contact Section](./assets/landing_page_contact_section.png)
<br>**Footer Section**: La sección que incluye un aviso de derechos de autor.
<br> ![Landing Page Footer Section](./assets/landing_page_footer_section.png)

### 6.2.1.7 Services Documentation Evidence for Sprint Review  
Este sprint 1 tuvo como enfoque principal la implementación de la Landing Page, por lo que no se han desarrollado Web Services. La documentación de Endpoints con OpenAPI y los detalles relacionados con Web Services serán relevantes en sprints futuros cuando se aborde la implementación y documentación de estos servicios. 

### 6.2.1.8 Software Deployment Evidence for Sprint Review  
En este Sprint 1, el equipo ha desplegado la Landing Page utilizando github pages. A continuación, se presentan las evidencias de despliegue del Sprint 1, que incluyen capturas de pantalla y pasos detallados del proceso de despliegue.
1. **Creación del Repositorio**: Se creó un repositorio en GitHub para alojar el código de la Landing Page. El repositorio se llama "LandingPage" y está disponible en la cuenta de GitHub del equipo.

url del repositorio: https://github.com/KamaqLabs/Dedalus_Landing_Page

2. **Configuración de GitHub Pages**: Se habilitó la opción de GitHub Pages en la configuración del repositorio. Esto permite que el contenido del repositorio se publique como una página web estática.
<br>
3. **Despliegue de la Landing Page**: Se subió el código HTML, CSS y JavaScript de la Landing Page al repositorio. GitHub Pages generó automáticamente una URL para acceder a la página.
<br>

4. **Acceso a la Landing Page**: La Landing Page se puede acceder a través de la URL proporcionada por GitHub Pages. Esta URL es pública y permite que cualquier persona acceda a la página.
<br> url de la landing page: https://kamaqlabs.github.io/Dedalus_Landing_Page/
5. **Evidencia del Despliegue**: Se realizó una captura de pantalla de la Landing Page desplegada para mostrar su apariencia y funcionalidad.


### 6.2.1.9 Team Collaboration Insights during Sprint  
Para el desarrollo de este sprint, el equipo designó a un integrante para el desarrollo de las actividades de implementación de la Landing Page.

GitHub insights del landing page:

![insights 4](./assets/insights%204.png)

## 6.3 Validation Interviews  
### 6.3.1 Diseño de Entrevistas  
#### 6.3.1.1 Preguntas para Gestores de Empresas Hoteleras
#### 6.3.1.2 Información Demográfica
#### 6.3.1.3 Evaluación del Landing Page y Aplicaciones
### 6.3.2 Preguntas para Huéspedes
#### 6.3.2.1 Información Demográfica
#### 6.3.2.2 Evaluación del Landing Page y Aplicaciones
#### 6.3.2.3  Conclusión de la Entrevista
### 6.3.3 Registro de Entrevistas  
### 6.3.3 Evaluacion segun heuristicas.
## 6.4 Video About-the-Product