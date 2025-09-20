<h1 style="text-align: center;"> Informe del TB1 </h1>
<h3 style="text-align: center;"> Universidad Peruana de Ciencias Aplicadas </h3>

<img src=https://github.com/Integradis-OpenSource/TFDocOpenSource/assets/114628079/4be29e42-94e4-4b80-85ae-3433dde891e4
style="display: block;
margin-left:auto;
margin-right: auto;
width=50%"/>

<h5 style="text-align: center"> Área: Ingeniería de Software </h5>

<h5 style="text-align: center"> Curso: Desarrollo de soluciones IOT </h5>
<h5 style="text-align: center"> Sección: 3475 </h5>

<h5 style="text-align: center"> Docente: Marco Antonio Leon Baca </h5>

<h5 style="text-align: center"> Startup: KamaqLabs </h5>

<h5 style="text-align: center"> Producto: Dedalus </h5>

## Team members:

|                  Nombre                  |   Código   |
|:----------------------------------------:|:----------:|
| Vasquez Requejo Augusto Mathias Leonardo | u20221A955 |
|  Cervantes Erequita Valentino Sebastian  | U202110140 |
|  Ccotarma Ttito, Sihuar Eduardo Eusebio  | U20211c736 |
|    Carpio Cornejo, Miguel Ángel Jesús    | u20221c360 |
|Braithuaite Toledo, Gabriel Anthony       | u20201e889 |

<h5 style="text-align: center"> Ciclo 2025-02 </h5>

# Registro de Versiones del Informe

El objetivo de esta sección es resumir las modificaciones relevantes que se realizan al informe durante el ciclo de vida del proyecto. Esta sección inicia en una página nueva y se incluye un cuadro con la siguiente estructura:

| Versión | Fecha      | Autores                     | Descripción de Modificaciones |
|---------|------------|-----------------------------|-------------------------------|
| 1era    | 19/25/2025 | |Carátula, CapítuloI, Capítulo II, Capítulo III, Capítulo IV, Capítulo V  |



## Project Report Collaboration Insights


URL del repositorio para el reporte del proyecto: https://github.com/KamaqLabs/Report





**TB1**

Para el desarrollo del informe perteneciente a la entrega TB1, se dividió la implementación de secciones de la siguiente forma para cada integrante del equipo:

| Integrante                            | Tareas Asignadas                                                                                                                           |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Vasquez Requejo Augusto Mathias Leonardo  |Chapters 01,02,03,04,05                   |
|   Cervantes Erequita Valentino Sebastian  | Chapters 01,02,03,04,05|
|   Ccotarma Ttito, Sihuar Eduardo Eusebio   | Chapters 01,02,03,04,05  |
| Carpio Cornejo, Miguel Ángel Jesús | Chapters 01,02,03,04,05|
|Braithuaite Toledo, Gabriel Anthony  | Chapters 01,02,03,04,05|


Los integrantes son:

- Vasquez Requejo Augusto Mathias Leonardo | (Mathifa519)
- Braithuaite Toledo Gabriel Anthony | (Gaboo04)
- Cervantes Erequita Valentino Sebastian |(KiwiAmenazante)
- Ccotarma Ttito, Sihuar Eduardo Eusebio | (Anx0123)
- Carpio Cornejo, Miguel Ángel Jesús | (MiguelCarpioC)
## Contenido
## Índice

- [Capítulo I: Introducción](/docs/Chapter-01.md)
    - [1.1. StartUp Profile](/docs/Chapter-01.md#11-startup-profile)
        - [1.1.1. Descripción de la StartUp](/docs/Chapter-01.md#111-descripción-de-la-startup)
        - [1.1.2. Perfiles de Integrantes del equipo](/docs/Chapter-01.md#112-perfiles-de-integrantes-del-equipo)
    - [1.2. Solution Profile](/docs/Chapter-01.md#12-solution-profile)
        - [1.2.1. Antecedentes y Problemática](/docs/Chapter-01.md#121-antecedentes-y-problemática)
        - [1.2.2. Lean UX Process](/docs/Chapter-01.md#122-lean-ux-process)
            - [1.2.2.1. Lean UX Problem Statements](/docs/Chapter-01.md#1221-lean-ux-problem-statements)
            - [1.2.2.2. Lean UX Assumptions](/docs/Chapter-01.md#1222-lean-ux-assumptions)
            - [1.2.2.3. Lean UX Hyphotesis Statements](/docs/Chapter-01.md#1223-lean-ux-hyphotesis-statements)
            - [1.2.2.4. Lean UX Canvas](/docs/Chapter-01.md#1224-lean-ux-canvas)
    - [1.3. Segmentos objetivo](/docs/Chapter-01.md#13-segmentos-objetivo)

- [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
    - [2.1. Competidores](#21-competidores)
        - [2.1.1 Análisis competitivo](#211-análisis-competitivo)
        - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
    - [2.2. Entrevistas](#22-entrevistas)
        - [2.2.1 Diseño de entrevistas](#221-diseño-de-entrevistas)
        - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
        - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
    - [2.3. Needfinding](#23-needfinding)
        - [2.3.1. User Persona](#231-user-persona)
        - [2.3.2. User Task Matrix](#232-user-task-matrix)
        - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
        - [2.3.4. Empathy Mapping](#234-empathy-mapping)
        - [2.4. Big Picture EventStorming](#236-big-picture-eventstorming)
        - [2.5. Ubiquitous Language](#237-ubiquitous-language)

- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
    - [3.1. User Stories](#31-user-stories)
    - [3.2. Impact Mapping](#32-impact-mapping)
    - [3.3. Product Backlog](#33-product-backlog)

- [Capítulo IV: Solution Software Design](#capítulo-iv-product-design)
    - [4.1. Strategic-Level Domain-Driven Design](#41-style-guidelines)
        - [4.1.1. Design-Level EventStorming](#411-general-style-guidelines)
            - [4.1.1.1. Candidate Context Discovery](#412-web-style-guidelines)
            - [4.1.1.1. Domain Message Flows Modeling](#412-web-style-guidelines)
            - [4.1.1.1. Bounded Context Canvases](#412-web-style-guidelines)
        - [4.1.2. Context Mapping](#42-information-architecture)
        - [4.1.3. Software Architecture](#421-organization-systems)
            - [4.1.3.1. Software Architecture System Landscape Diagram](#421-system-landscape-diagram)
            - [4.1.3.2 Software Architecture Context Level Diagrams](#422-labeling-systems)
            - [4.1.3.3. Software Architecture Container Level Diagrams](#423-searching-systems)
            - [4.1.3.4 Software Architecture Deployment Diagrams](#424-labeling-systems)
    - [4.2. Tactical-Level Domain-Driven Design](#41-style-guidelines)
        - [4.2.1. Bounded Context](#424-searching-systems)
            - [4.2.1.1 Domain Layer](#425-navigation-systems)
            - [4.2.1.2 Interface Layer](#425-navigation-systems)
            - [4.2.1.3 Application Layer](#425-navigation-systems)
            - [4.2.1.4 Infrastructure Layer](#425-navigation-systems)
            - [4.2.1.5 Bounded Context Software Architecture Component Level Diagrams](#425-navigation-systems)
            - [4.2.1.6 Bounded Context Software Architecture Code Level Diagrams](#425-navigation-systems)
                - [4.2.1.6.1 Bounded Context Domain Layer Class Diagrams](#425-navigation-systems)
                - [4.2.1.6.2 Bounded Context Database Design Diagram](#425-navigation-systems)

- [Conclusiones](#conclusiones)
    - [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)
    - [Video About-the-Team](#video-about-the-team)

- [Bibliografía](#bibliografía)
- [Anexos](#anexos)

# Student Outcome
**ABET – EAC - Student Outcome 5**  
Criterio: La capacidad de funcionar efectivamente en un equipo cuyos miembros juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo, establecen objetivos, planifican tareas y cumplen objetivos.  

| Criterio Específico                                                                            | Acciones Realizadas | Conclusiones |
|------------------------------------------------------------------------------------------------|--------------------|---------------------|
| Trabaja en equipo para proporcionar liderazgo en forma conjunta                                | **Vasquez Requejo Augusto Mathias Leonardo** <br> TB1: Contribuyó al desarrollo de los capítulos iniciales del informe, organizando los apartados de introducción y propuesta de solución, lo que permitió orientar al equipo sobre la estructura general del documento. <br><br> **Cervantes Erequita Valentino Sebastian** <br> TB1: Aportó en la redacción y consolidación de las secciones relacionadas con la problemática y entrevistas, coordinando con el equipo para definir las ideas clave. <br><br> **Ccotarma Ttito Sihuar Eduardo Eusebio** <br> TB1: Se enfocó en el análisis de competidores y necesidades de usuario, planteando lineamientos para guiar las decisiones del equipo. <br><br> **Carpio Cornejo Miguel Ángel Jesús** <br> TB1: Colaboró en la organización del índice y los entregables de especificación de requerimientos, brindando soporte en la redacción y alineación de criterios comunes. <br><br> **Gabriel Braithuaite** <br> TB1: Trabajó con el equipo de manera conjunta decidiendo los objetivos de la primera entrega. | Se logró consolidar el liderazgo compartido entre los integrantes, distribuyendo funciones claves que guiaron la elaboración del documento TB1. |
| Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos | **Vasquez Requejo Augusto Mathias Leonardo** <br> TB1: Facilitó la coordinación inicial del trabajo, definiendo los primeros objetivos y estableciendo un plan de redacción conjunta. <br><br> **Cervantes Erequita Valentino Sebastian** <br> TB1: Apoyó en la revisión cruzada de capítulos y promovió un ambiente inclusivo, asegurando que todas las ideas fueran consideradas. <br><br> **Ccotarma Ttito Sihuar Eduardo Eusebio** <br> TB1: Aseguró la integración de los aportes del equipo en las secciones de análisis de usuarios, cumpliendo plazos acordados. <br><br> **Carpio Cornejo Miguel Ángel Jesús** <br> TB1: Coordinó la elaboración de diagramas y apartados técnicos, fomentando la colaboración entre todos los integrantes. <br><br> **Gabriel Braithuaite** <br> TB1: En base a los objetivos de la primera entrega, planificó las tareas que debía cumplir para aportar al equipo trabajando de manera colaborativa. | El equipo trabajó de manera organizada y colaborativa, estableciendo metas claras y cumpliendo las tareas asignadas dentro de los plazos establecidos, lo que fortaleció el trabajo conjunto. |
