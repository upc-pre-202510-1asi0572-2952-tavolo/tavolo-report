<div align="center">
    <h3>Universidad Peruana de Ciencias Aplicadas</h3>
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png"></img><br>
    <strong>Ingeniería de Software - 7mo Ciclo</strong><br>
    <strong>Desarrollo de Soluciones IOT</strong><br>
    <strong>1ASI0572</strong><br>
    <strong>Profesor: Marco Antonio León Baca</strong><br>
    <br><strong>Report</strong><br>
    <br><strong>Tavolo</strong><br>
    <!--<strong>name startup</strong>-->
</div>

<h3> Team Members: </h3>

<div align="center">

| Member                              |    Code    |
| :---------------------------------- | :--------: |
| Baldeon Fabian, Aldo Alberto        | u202122633 |
| Cama Salvatierra, Jimena Tamara     | u202210778 |
| Castillo Castillo, Jair Alexander   | u202211390 |
| La Torre Valle, Franz Jair          | u202012378 |
| Quezada Portalatino, Barbara Susana | u202211800 |

</div>

<h3 align="center">Abril, 2025</h3>

<br><br>

<div align="justify">




## Registro de Versiones del Informe

El objetivo de esta sección es resumir las modificaciones relevantes que se realizan al informe durante el ciclo de vida del proyecto. Esta sección inicia en una página nueva e incluye un cuadro con la siguiente estructura:

<table>
  <thead>
    <tr>
      <th>Versión</th>
      <th>Fecha</th>
      <th>Autor</th>
      <th>Descripción de modificación</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0.1</td>
      <td>-</td>
      <td>-</td>
      <td>-</td>
    </tr>
    
  </tbody>
</table>

## Project Report Collaboration Insights

Para desarrollar el proyecto, se empleó GitHub como herramienta para gestionar versiones y facilitar la colaboración en tiempo real. A continuación, se proporciona el enlace al repositorio del proyecto:

| **Descripción**            | **Enlace**                                                                 |
| :-------------------------: | :------------------------------------------------------------------------: |
| Repositorio del Proyecto    | https://github.com/IoT-Solutions-SW71-Grupo-4/HidroBots-Report.git         |
| Link de la Organización     | https://github.com/upc-pre-202510-1asi0572-2952-tavolo                    |

**TB1:**

Para el TB1, se asignaron responsabilidades específicas a cada integrante, las cuales se detallan a continuación:

| Miembro del Equipo | Tarea Asignada |
|       :---:        |      :---:     |
| Aldo Baldeon       |        -       |
| Barbara Quezada    |        -       |
| Franz La Torre     |        -       |
| Jimena Cama        |        -       |
| Jair Castillo      |        -       |

Cabe destacar que, durante la creación del informe, se realizaron commits específicos para cada tarea asignada, lo que permitió garantizar un control de versiones y una colaboración efectiva en tiempo real.

Miembros

- Aldo Baldeon    (CodAress)
- Barbara Quezada (BarbaraQP15)
- Franz La Torre  (FranzJairLTV)
- Jimena Cama     (AkSoon-ie)
- Jair Castillo   (U202211390)
  
El uso de GitHub ha permitido gestionar versiones y fomentar la colaboración en tiempo real, facilitando que los integrantes del equipo trabajen tanto de forma asincrónica como sincrónica en el proyecto. Asimismo, la metodología Gitflow ha posibilitado la creación de diversas ramas para el desarrollo de las tareas asignadas, promoviendo un trabajo autónomo y colaborativo entre los miembros.

La rama "develop" se utilizó como un entorno para integrar las tareas de cada miembro de manera estructurada y organizada, mientras que la rama "main" se destinó a la entrega de la versión final del proyecto.

# Contenido

## Tabla de Contenidos

### [Registro de Versiones del Informe](#registro-de-versiones-del-informe)

### [Project Report Collaboration Insights](#project-report-collaboration-insights)

### [Contenido](#contenido)

### [Student Outcomes](#student-outcome)

### [Capítulo I: Introducción](#capítulo-i-introducción)

- [Contenido](#contenido)
  - [Tabla de Contenidos](#tabla-de-contenidos)
    - [Registro de Versiones del Informe](#registro-de-versiones-del-informe-1)
    - [Project Report Collaboration Insights](#project-report-collaboration-insights-1)
    - [Contenido](#contenido-1)
    - [Student Outcomes](#student-outcomes)
    - [Capítulo I: Introducción](#capítulo-i-introducción)
    - [Capítulo II: Requirements Elicitation \& Analysis](#capítulo-ii-requirements-elicitation--analysis)
    - [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
    - [Capítulo IV: Solution Software Design](#capítulo-iv-solution-software-design)
    - [Capítulo V: Solution UI/UX Design](#capítulo-v-solution-uiux-design)
    - [Capítulo VI: Product Implementation, Validation \& Deployment](#capítulo-vi-product-implementation-validation--deployment)
    - [Conclusiones](#conclusiones)
    - [Bibliografía](#bibliografía)
    - [Anexos](#anexos)
- [Student Outcome](#student-outcome)
- [Capítulo I: Introducción](#capítulo-i-introducción-1)
  - [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
  - [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1. Antecedentes y problemática](#121-antecedentes-y-problemática)
    - [1.2.2. Lean UX Process](#122-lean-ux-process)
      - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
      - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
          - [**Business Outcomes:**](#business-outcomes)
          - [**Users:**](#users)
          - [**User Outcomes \& Benefits:**](#user-outcomes--benefits)
          - [**Feature Assumptions:**](#feature-assumptions)
          - [**Business Assumptions:**](#business-assumptions)
          - [**User Assumptions:**](#user-assumptions)
      - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
      - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
  - [1.3. Segmentos objetivo](#13-segmentos-objetivo)
  - [4.2. Tactical-Level Domain-Driven-Design](#42-tactical-level-domain-driven-design)
    - [4.2.1 Bounded Context: IAM Bounded Context](#421-bounded-context-iam-bounded-context)
      - [4.2.1.1. Domain Layer](#4211-domain-layer)
        - [**Aggregates**](#aggregates)
        - [**Entities**](#entities)
        - [**Value Objects**:](#value-objects)
      - [4.2.1.2. Interface Layer](#4212-interface-layer)
      - [**Controllers**](#controllers)
      - [**Resources**](#resources)
      - [**Transformers**](#transformers)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes)
      - [4.2.1.3 Application Layer](#4213-application-layer)
      - [**Command Services**](#command-services)
      - [**Query Services**](#query-services)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-1)
      - [4.2.1.4. Infrastructure Layer](#4214-infrastructure-layer)
      - [**Persistencia (JPA Repositories)**](#persistencia-jpa-repositories)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-2)
      - [4.2.1.5. Bounded Context Software Architecture Component Level Diagrams](#4215-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.1.6. Bounded Context Software Architecture Code Level Diagrams](#4216-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.1.6.1. Bounded Context Domain Layer Class Diagrams](#42161-bounded-context-domain-layer-class-diagrams)
        - [4.2.1.6.2. Bounded Context Database Design Diagram.](#42162-bounded-context-database-design-diagram)
    - [4.2.3 Bounded Context: Branching Bounded Context](#423-bounded-context-branching-bounded-context)
      - [4.2.3.1. Domain Layer](#4231-domain-layer)
        - [**Aggregates**](#aggregates-1)
        - [**Entities**](#entities-1)
        - [**Value Objects**](#value-objects-1)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-3)
      - [4.2.3.2. Interface Layer](#4232-interface-layer)
      - [**Access Control Layer (ACL)**](#access-control-layer-acl)
      - [**Controllers**](#controllers-1)
      - [**Resources**](#resources-1)
      - [**Transformers**](#transformers-1)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-4)
      - [4.2.3.4. Infrastructure Layer](#4234-infrastructure-layer)
      - [**Persistencia (JPA Repositories)**](#persistencia-jpa-repositories-1)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-5)
      - [4.2.3.5. Bounded Context Software Architecture Component Level Diagrams](#4235-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.3.6. Bounded Context Software Architecture Code Level Diagrams](#4236-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.3.6.1. Bounded Context Domain Layer Class Diagrams](#42361-bounded-context-domain-layer-class-diagrams)
        - [4.2.3.6.2. Bounded Context Database Design Diagram.](#42362-bounded-context-database-design-diagram)
    - [4.2.4 Bounded Context: Booking Bounded Context](#424-bounded-context-booking-bounded-context)
      - [4.2.4.1. Domain Layer](#4241-domain-layer)
      - [**Aggregates**](#aggregates-2)
      - [**Entities**](#entities-2)
      - [**Value Objects**](#value-objects-2)
      - [**Commands**](#commands)
      - [**Queries**](#queries)
      - [**Events**](#events)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-6)
      - [4.2.4.2. Interface Layer](#4242-interface-layer)
      - [**Controllers**](#controllers-2)
      - [**Resources**](#resources-2)
      - [**Transformers**](#transformers-2)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-7)
      - [4.2.4.3. Application Layer](#4243-application-layer)
      - [**Command Services**](#command-services-1)
      - [**Query Services**](#query-services-1)
      - [**Event Handlers**](#event-handlers)
      - [**Outbound Services (ACL)**](#outbound-services-acl)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-8)
      - [4.2.4.4. Infrastructure Layer](#4244-infrastructure-layer)
      - [**Persistencia (JPA Repositories)**](#persistencia-jpa-repositories-2)
      - [**Relaciones entre componentes**](#relaciones-entre-componentes-9)
      - [4.2.4.5. Bounded Context Software Architecture Component Level Diagrams](#4245-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.4.6. Bounded Context Software Architecture Code Level Diagrams](#4246-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.4.6.1. Bounded Context Domain Layer Class Diagrams](#42461-bounded-context-domain-layer-class-diagrams)
        - [4.2.4.6.2. Bounded Context Database Design Diagram.](#42462-bounded-context-database-design-diagram)

### [Capítulo II: Requirements Elicitation & Analysis](#capc3adtulo-ii-requirements-elicitation--analysis-1)

- [2.1. Competidores](#21-competidores)
  - [2.1.1. Análisis competitivo](#211-análisis-competitivo)
  - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
- [2.2. Entrevistas](#22-entrevistas)
  - [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)
  - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
  - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
- [2.3. Needfinding](#23-needfinding)
  - [2.3.1. User Personas](#231-user-personas)
  - [2.3.2. User Task Matrix](#232-user-task-matrix)
  - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
  - [2.3.4. Empathy Mapping](#234-empathy-mapping)
  - [2.3.5. As-is Scenario Mapping](#235-as-is-scenario-mapping)
- [2.4. Ubiquitous Language](#24-ubiquitous-language)

### [Capítulo III: Requirements Specification](#capc3adtulo-iii-requirements-specification)

- [3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)
- [3.2. User Stories](#32-user-stories)
- [3.3. Impact Mapping](#33-impact-mapping)
- [3.4. Product Backlog](#34-product-backlog)

### [Capítulo IV: Solution Software Design](#capc3adtulo-iv-solution-software-design)

- [4.1. Strategic-Level Domain-Driven Design](#41-strategic-level-domain-driven-design)
  - [4.1.1. Event Storming](#411-event-storming)
    - [4.1.1.1 Candidate Context Discovery](#4111-candidate-context-discovery)
    - [4.1.1.2 Domain Message Flows Modeling](#4112-domain-message-flows-modeling)
    - [4.1.1.3 Bounded Context Canvases](#4113-bounded-context-canvases)
  - [4.1.2. Context Mapping](#412-context-mapping)
  - [4.1.3. Software Architecture](#413-software-architecture)
    - [4.1.3.1. Software Architecture System Landscape Diagram](#4131-software-architecture-system-landscape-diagram)
    - [4.1.3.2. Software Architecture Context Level Diagrams](#4132-software-architecture-context-level-diagrams)
    - [4.1.3.3. Software Architecture Deployment Diagrams](#4133-software-architecture-deployment-diagrams)
- [4.2. Tactical-Level Domain-Driven Design](#42-tactical-level-domain-driven-design)
  - [4.2.X. Bounded Context: Bounded Context Name](#42x-bounded-context-bounded-context-name)
    - [4.2.X.1. Domain Layer](#42x1-domain-layer)
    - [4.2.X.2. Interface Layer](#42x2-interface-layer)
    - [4.2.X.3. Application Layer](#42x3-application-layer)
    - [4.2.X.4. Infrastructure Layer](#42x4-infrastructure-layer)
    - [4.2.X.6. Bounded Context Software Architecture Component Level Diagrams](#42x6-bounded-context-software-architecture-component-level-diagrams)
    - [4.2.X.7. Bounded Context Software Architecture Code Level Diagrams](#42x7-bounded-context-software-architecture-code-level-diagrams)
      - [4.2.X.7.1. Bounded Context Domain Layer Class Diagrams](#42x71-bounded-context-domain-layer-class-diagrams)
      - [4.2.X.7.2. Bounded Context Database Design Diagram](#42x72-bounded-context-database-design-diagram)

### [Capítulo V: Solution UI/UX Design](#capc3adtulo-v-solution-uiux-design)
- [5.1. Style Guidelines](#51-style-guidelines)
  - [5.1.1. General Style Guidelines](#511-general-style-guidelines)
  - [5.1.2. Web, Mobile and IoT Style Guidelines](#512-web-mobile-and-iot-style-guidelines)
- [5.2. Information Architecture](#52-information-architecture)
  - [5.2.1. Organization Systems](#521-organization-systems)
  - [5.2.2. Labeling Systems](#522-labeling-systems)
  - [5.2.3. SEO Tags and Meta Tags](#523-seo-tags-and-meta-tags)
  - [5.2.4. Searching Systems](#524-searching-systems)
  - [5.2.5. Navigation Systems](#525-navigation-systems)
- [5.3. Landing Page UI Design](#53-landing-page-ui-design)
  - [5.3.1. Landing Page Wireframe](#531-landing-page-wireframe)
  - [5.3.2. Landing Page Mock-up](#532-landing-page-mock-up)
- [5.4. Applications UX/UI Design](#54-applications-uxui-design)
  - [5.4.1. Applications Wireframes](#541-applications-wireframes)
  - [5.4.2. Applications Wireflow Diagrams](#542-applications-wireflow-diagrams)
  - [5.4.3. Applications Mock-ups](#543-applications-mock-ups)
  - [5.4.4. Applications User Flow Diagrams](#544-applications-user-flow-diagrams)
- [5.5. Applications Prototyping](#55-applications-prototyping)

### [Capítulo VI: Product Implementation, Validation & Deployment](#capitulo-vi-product-implementation-validation-deployment)
- [6.1. Software Configuration Management](#61-software-configuration-management)
  - [6.1.1. Software Development Environment Configuration](#611-software-development-environment-configuration)
  - [6.1.2. Source Code Management](#612-source-code-management)
  - [6.1.3. Source Code Style Guide & Conventions](#613-source-code-style-guide-conventions)
  - [6.1.4. Software Deployment Configuration](#614-software-deployment-configuration)
- [6.2. Landing Page, Services & Applications Implementation](#62-landing-page-services--applications-implementation)
- [6.3. Validation Interviews](#63-validation-interviews)
- [6.3.1. Diseño de Entrevistas](#631-diseño-de-entrevistas)
- [6.3.2. Registro de Entrevistas](#632-registro-de-entrevistass)
- [6.3.3. Evaluaciones según heurísticas](#633-evaluaciones-según-heurísticas)
- [6.4. Video About-the-Product](#64-video-about-the-product)


### [Conclusiones](#conclusiones)

- [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)

### [Bibliografía](#bibliografía)

### [Anexos](#anexos)

# Student Outcome

El curso contribuye al cumplimiento del Student Outcome ABET:
**ABET – EAC - Student Outcome 5**
**Criterio:** La capacidad de funcionar efectivamente en un equipo cuyos miembros
juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo,
establecen objetivos, planifican tareas y cumplen objetivos.
En el siguiente cuadro se describe las acciones realizadas y enunciados de
conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 5.

<!-- Cambiamos el rowspan="1" por rowspan="n" cuando agregamos más de una acción realizada por criterio específico. (TB1, TP1, TB2, TF1)-->

<table>
    <tr>
        <th><b>Criterio específico</b></th>
        <th><b>Acciones realizadas</b></th>
        <th><b>Conclusiones</b></th>
    </tr>
    <tr>
        <td rowspan="1"><b>Trabaja en equipo para proporcionar liderazgo en forma conjunta</b></td>
        <td>TB1<br><br>
            <b>Baldeon Fabian, Aldo Alberto</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br> 
            <b>Cama Salvatierra, Jimena Tamara</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
            <b>Castillo Castillo, Jair Alexander</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
            <b>La Torre Valle, Franz Jair</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
            <b>Quezada Portalatino, Barbara Susana</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
        </td>
        <td>TB1<br><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
        </td>
    </tr>
    <tr>
        <td rowspan="1"><b>Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos.</b></td>
        <td>TB1<br><br>
            <b>Baldeon Fabian, Aldo Alberto</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br> 
            <b>Cama Salvatierra, Jimena Tamara</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
            <b>Castillo Castillo, Jair Alexander</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
            <b>La Torre Valle, Franz Jair</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
            <b>Quezada Portalatino, Barbara Susana</b><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
            <br><br>
        </td>
        <td>TB1<br><br>
            - Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi.
        </td>
    </tr>
</table>

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup 

**Nombre startup** es una empresa dedicada a la implementación de soluciones IoT para la gestión inteligente del aforo de restaurantes, cafeterías y otros establecimientos de hostelería. Nuestro sistema permitirá a los establecimientos monitorizar en tiempo real la ocupación de mesas y ofrecer a los clientes información actualizada a través de una aplicación móvil y web, mejorando la experiencia del usuario y la eficiencia operativa. 

**Mision:**<br>
Brindar una solución IoT innovadora que permita a restaurantes, cafeterías y locales similares gestionar su foro de forma eficiente y segura, ofreciendo una experiencia de usuario intuitiva y facilitando la toma de decisiones operativas en tiempo real.

**Visión:**<br>
Ser la plataforma líder en gestión inteligente de aforo para el sector de la hostelería en el Perú, reconocida por la innovación, la eficiencia operativa y el impacto positivo en la experiencia del cliente.


### 1.1.2. Perfiles de integrantes del equipo  

<table>
  <tr align="center">
    <td rowspan="4">
      <img src="./images/profile_images/aldo_profile.jpg" alt="Aldo's profile image" min-width="400" max-width="900"/>
    </td>
    <td align="left">
      <b>Nombre y Apellido:</b>
      <br>            
      Aldo Alberto Baldeon Fabian
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Código:</b>
    <br>
    U202122633
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Carrera:</b>
    <br>
    Ingeniería de Software
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Acerca de:</b>
    <br>
    Soy Aldo Alberto Baldeon Fabian, estudio la carrera de Ingeniería de Software en la UPC. Escogí esta carrera porque me interesó el desarrollo de aplicaciones. Soy responsable y me gusta trabajar en equipo. Poseo conocimientos básicos en C#, java, JavaScript, HTML y CSS. También, poseo conocimientos intermedios en C + +, SQL y MongoDB, además de contar con experiencia en Git y GitHub.
    </td>
  </tr>
  </tr>

  <tr align="center">
    <td rowspan="4">
      <img src="./images/profile_images/barbara_profile.jpg" alt="Barbara's profile image" min-width="400" max-width="900"/>
    </td>
    <td align="left">
      <b>Nombre y Apellido:</b>
      <br>            
      Barbara Susana Quezada Portalatino
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Código:</b>
    <br>
    U202211800
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Carrera:</b>
    <br>
    Ingeniería de Software
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Acerca de:</b>
    <br>
    Barbara Susana Quezada Portalatino, cursando el séptimo ciclo de la carrera de software, trabajo mayormente bajo un rol de líder que me ayuda a poder organizar no solo la ideas de mi grupo sino que las ideas aterricen en la ejecución. Soy una persona muy disciplinada y detallista.
    </td>
  </tr>
  </tr>
   <tr align="center">
    <td rowspan="4">
      <img src="./images/profile_images/jimena_profile.jpg" alt="Jimena's profile image" min-width="400" max-width="900"/>
    </td>
    <td align="left">
      <b>Nombre y Apellido:</b>
      <br>            
      Jimena Tamara Cama Salvatierra
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Código:</b>
    <br>
    U2022210778
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Carrera:</b>
    <br>
    Ingeniería de Software
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Acerca de:</b>
    <br>
     Soy estudiante de la carrera de Ingeniería de Software en la UPC y actualmente estoy cursando el 7mo ciclo. Me considero una persona curiosa, determinada y organizada. Con la experiencia en proyectos de startup y trabajos en equipo, trabajaré junto a mis compañeros para lograr un óptimo resultado del proyecto.
    </td>
  </tr>
  </tr>

<tr align="center">
    <td rowspan="4">
      <img src="./images/profile_images/jair_profile.jpg" alt="Jair's profile image" min-width="400" max-width="900"/>
    </td>
    <td align="left">
      <b>Nombre y Apellido:</b>
      <br>            
      Jair Alexander Castillo Castillo
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Código:</b>
    <br>
    U202211390
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Carrera:</b>
    <br>
    Ingeniería de Software
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Acerca de:</b>
    <br>
    Soy estudiante de la carrera de Ingeniería de Software en la UPC y me encuentro en el 7to ciclo. Me considero una persona dedicada, comprensiva y metódica. Con mis habilidades de liderazgo y mi capacidad para trabajar en equipo en un ambiente de respeto, estoy segura de que podré dirigir la implementación de la startup de nuestro proyecto de manera exitosa.
    </td>
  </tr>
  </tr>
  
<tr align="center">
    <td rowspan="4">
      <img src="./images/profile_images/franz_profile.jpg" alt="Franz's profile image" min-width="400" max-width="900"/>
    </td>
    <td align="left">
      <b>Nombre y Apellido:</b>
      <br>            
      Franz Jair La Torre Valle
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Código:</b>
    <br>
    U202012378
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Carrera:</b>
    <br>
    Ingeniería de Software
    </td>
  </tr>
  <tr>
    <td align="left">
    <b>Acerca de:</b>
    <br>
    Soy estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Mi compromiso con el equipo se basa en mantener una participación activa en todas las actividades, estar siempre disponible para resolver dudas y contribuir de manera significativa al desarrollo del proyecto. Busco aportar con soluciones innovadoras, apoyo constante y un aprendizaje continuo para alcanzar los objetivos propuestos.
    </td>
  </tr>

</table>


## 1.2. Solution Profile

Nuestra propuesta consiste en el desarrollo de una solución IoT que permita la automatización en el control de aforo de establecimientos mediante la detección de ocupación de mesas a través de sensores de peso. La solución se integra con aplicaciones móviles y web, facilitando a los clientes conocer la disponibilidad de mesas y a los administradores del local gestionar el flujo de personas.

### 1.2.1. Antecedentes y problemática  

El sector gastronómico peruano consolida su posición como motor clave de la economía, registrando un crecimiento sostenido en los últimos años. Según datos del INEI (citados por la Oficina General de Evaluación de Impacto y Estudios Económicos, 2025), Lima concentró el 41.6% del gasto anual en restaurantes durante 2024, evidenciando su liderazgo en el consumo nacional. Sin embargo, este dinamismo enfrenta desafíos críticos: la ocupación en establecimientos varía según temporada y tipo de negocio, mientras que los tiempos de espera prolongados impactan directamente en la satisfacción del cliente y la rentabilidad.

En este contexto, la tecnología emerge como aliada estratégica. López-Chau et al. (2022) destacan en su estudio publicado en Estudios Gerenciales que herramientas como el software de gestión de mesas mitigan estos problemas, optimizando el flujo de clientes. Avanzando en esta línea, soluciones innovadoras como sensores IoT integrados en mesas representan el siguiente paso: no solo reducirían tiempos de espera, sino que mejorarían la experiencia mediante datos en tiempo real, potenciando la competitividad del sector.

**What? - ¿Qué?** <br>
La problemática actual en muchos restaurantes y cafeterías es la falta de un sistema en tiempo real que permita conocer el estado de ocupación de sus mesas. La ausencia de esta tecnología dificulta la gestión del aforo, especialmente en horas pico o durante eventos especiales, lo cual puede afectar la experiencia del cliente.

**When? - ¿Cuándo?**<br>
El problema se vuelve crítico en momentos de alta afluencia, como durante almuerzos, cenas, fines de semana o eventos especiales, en los cuales la ocupación irregular de las mesas puede generar aglomeraciones y una mala experiencia para los clientes.

**Where? - ¿Dónde?**<br>
El desafío se presenta en restaurantes, cafeterías y otros establecimientos de hostelería, tanto en grandes ciudades como en zonas turísticas, donde la demanda y el flujo de clientes varían constantemente.

**Who? - ¿Quién?** <br>
Los principales afectados son los propietarios y administradores de locales de hostelería, así como los clientes que buscan una experiencia cómoda y segura. Además, las autoridades sanitarias y de seguridad pueden verse beneficiadas al contar con datos en tiempo real para el control de aforo.

**Why? - ¿Por qué?** <br>
La falta de información precisa sobre la ocupación de mesas puede generar problemas de sobreaforo, dificultades en la atención al cliente y riesgos en el cumplimiento de protocolos de seguridad. La integración de tecnologías IoT permite automatizar y optimizar estos procesos, reduciendo errores humanos y mejorando la eficiencia operativa.

**How? - ¿Cómo?** <br>
La solución se implementará instalando sensores de peso en cada mesa, conectados a una red IoT que transmite datos en tiempo real a una plataforma centralizada. A través de una aplicación móvil y web, los usuarios podrán visualizar la disponibilidad de mesas y, a su vez, el personal del establecimiento podrá gestionar la ocupación de manera óptima y recibir alertas en caso de anomalías.

**How much? - ¿Cuánto?** <br>
_¿Cuánto afecta este problema?_ <br>
La falta de control de aforo puede traducirse en pérdidas económicas para los establecimientos debido a la ineficiencia en la asignación de mesas, así como en sanciones por incumplimiento de normativas de seguridad.

_¿Cuánto costará resolver este problema?_ <br>
El costo de implementación dependerá del número de mesas y la infraestructura necesaria para la conexión y mantenimiento de los sensores, así como del desarrollo de la plataforma digital. Se estima que la inversión inicial se recuperará rápidamente mediante la optimización del uso del espacio y el incremento en la satisfacción del cliente.

_¿Cuántas personas se beneficiarán?_ <br>
Esta solución beneficiará directamente a los clientes y al personal de los establecimientos, con un impacto indirecto en el sector de la hostelería en general. Se estima que, en establecimientos de tamaño mediano, la adopción de la tecnología podría mejorar la eficiencia operativa en un 30-40%, beneficiando a cientos de usuarios diarios.

**Conclusiones de 5W's y 2H's:** <br>
La implementación de la solución IoT para el control de aforo permite identificar y abordar de manera efectiva los problemas relacionados con la ocupación ineficiente de mesas. Al automatizar la detección y gestión del aforo, se optimiza el uso del espacio en los establecimientos, se mejora la experiencia del cliente y se aseguran protocolos de seguridad que contribuyen a la sostenibilidad operativa.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements 

En **nombre startup** sabemos que el sector de la hostelería en Perú es vital para la economía nacional y que la experiencia del cliente es fundamental para el éxito de cada establecimiento. Sin embargo, muchos restaurantes, cafeterías y locales de hostelería enfrentan un reto crítico: la ausencia de un sistema en tiempo real que permita conocer la ocupación exacta de sus mesas. <br>

**Problema:** La falta de información precisa y actualizada sobre la disponibilidad de mesas provoca una gestión ineficiente del aforo. Esto se traduce en aglomeraciones durante las horas pico, tiempos de espera prolongados para los clientes y, en algunos casos, incumplimiento de protocolos de seguridad que pueden acarrear sanciones. <br>

**Impacto:** Esta problemática afecta directamente la rentabilidad y la imagen del establecimiento, generando pérdidas económicas y deteriorando la experiencia del cliente. Al implementar una solución IoT basada en sensores de peso integrados en las mesas y conectados a una plataforma digital, los locales podrán optimizar la asignación de asientos, reducir los tiempos de espera y mejorar tanto la eficiencia operativa como la satisfacción del usuario, permitiendo así transformar un desafío en una ventaja competitiva. <br>

#### 1.2.2.2. Lean UX Assumptions  

###### **Business Outcomes:**

- Aumento del 25% en la eficiencia operativa de los establecimientos que adopten la solución.
- Reducción del 30% en incidencias por sobreaforo y problemas de asignación de mesas.
- Incremento del 20% en la satisfacción de los clientes, medido a través de encuestas de experiencia.
- Incremento del 15% en el flujo de clientes al evitar tiempos de espera prolongados.
- Mejora en el cumplimiento de protocolos de seguridad y normativas vigentes.

###### **Users:**

Los usuarios primarios son:
- Propietarios y administradores de restaurantes y cafeterías: Interesados en optimizar el uso del espacio y garantizar la seguridad en el establecimiento. <br>
  
- Clientes: Usuarios que buscan información en tiempo real sobre la disponibilidad de mesas para planificar su visita de manera eficiente. <br>

###### **User Outcomes & Benefits:**

- Propietarios/Administradores:
  - Control en tiempo real del aforo y asignación de mesas.
  - Reducción de errores manuales en la gestión de espacios.
  - Acceso a estadísticas e informes que faciliten la toma de decisiones.

- Clientes:
  - Información precisa sobre la disponibilidad de mesas.
  - Reducción de tiempos de espera al llegar al local.
  - Mejora en la experiencia y comodidad al planificar su visita.

###### **Feature Assumptions:**

- Detección en tiempo real: Uso de sensores de peso para determinar la ocupación de cada mesa.

- Aplicación móvil y web: Interfaz intuitiva que permita a los usuarios conocer la disponibilidad en tiempo real.

- Alertas y notificaciones: Envío de notificaciones al personal del local en caso de ocupación irregular o sobreaforo.

- Reportes y análisis: Generación de informes históricos y en tiempo real para facilitar la toma de decisiones y mejorar la gestión operativa.


###### **Business Assumptions:**

1.  **Creemos que nuestros usuarios necesitan** un sistema automatizado y en tiempo real que facilite la gestión del aforo en establecimientos de hostelería.

2. **Estas necesidades se pueden satisfacer** mediante la implementación de sensores IoT y el desarrollo de una plataforma digital accesible desde dispositivos móviles y computadoras.

3. **Nuestros clientes serán** restaurantes, cafeterías y otros locales de hostelería que buscan mejorar la eficiencia en la gestión de sus espacios y la experiencia de sus clientes.

4. **El valor más importante que un cliente quiere de nuestros servicios es** la capacidad de optimizar la ocupación de mesas en tiempo real, garantizando tanto la seguridad como la eficiencia operativa.

5. **El cliente también va obtener** beneficios adicionales como la recopilación de datos para análisis futuros.

6. **Vamos a obtener la mayoría de nuestros clientes mediante** estrategias de marketing digital, participación en ferias de tecnología y colaboraciones con asociaciones del sector de hostelería.

7. **Vamos a obtener ingresos mediante** la venta de la solución IoT como hardware y software.

8. **Nuestra competencia principal** son los sistemas tradicionales de control de aforo y soluciones de monitoreo manual.

9. **Vamos a tener ventaja frente a nuestra competencia debido a** la automatización en tiempo real, la facilidad de uso y la capacidad de integración con otras plataformas, lo que mejora significativamente la eficiencia operativa.

10. **El mayor riesgo del servicio es** la posible resistencia de los establecimientos a la adopción de nuevas tecnologías y la integración con sistemas ya existentes.

11. **Lo resolveremos mediante** demostraciones prácticas, pruebas piloto y estrategias de capacitación para asegurar una transición suave y una rápida adopción de la tecnología.

###### **User Assumptions:**

**¿Quién es el usuario?** <br>
Los usuarios son propietarios, administradores y clientes de restaurantes, cafeterías y otros locales de hostelería, que buscan una solución tecnológica para gestionar de manera eficiente la ocupación de mesas.<br>

**¿Qué problemas tiene nuestro producto? ¿Resolver?** <br>
El principal problema es la falta de información en tiempo real sobre la disponibilidad de mesas, lo que genera tiempos de espera, errores en la asignación de asientos y riesgos en el cumplimiento de normativas de seguridad. Nuestra solución automatiza este proceso, reduciendo la incertidumbre y mejorando la experiencia del usuario. <br>

**¿Qué características son importantes?** <br>
- Monitoreo en tiempo real de la ocupación mediante sensores de peso.
- Interfaz intuitiva y amigable en la aplicación móvil y web.
- Alertas y notificaciones automáticas para el personal del local.
- Reportes históricos y en tiempo real para el análisis del uso del espacio.
- Integración con otros sistemas de gestión interna del establecimiento.
<br>

**¿Dónde encaja nuestro producto en su trabajo o vida?** <br>
La solución se integra en la operación diaria de los establecimientos de hostelería, facilitando tanto la gestión interna (para administradores) como la experiencia del cliente al planificar su visita. <br>

**¿Cuándo y cómo es nuestro producto? ¿Usado?** <br>
El producto es utilizado en tiempo real, especialmente durante horas pico y en momentos de alta afluencia, permitiendo a los establecimientos gestionar el aforo de forma continua y los clientes verificar la disponibilidad antes de llegar. <br>

**¿Cómo debe verse nuestro productoo y cómo debe comportarse?** <br>
La interfaz visual debe ser moderna, limpia e intuitiva, con gráficos y datos en tiempo real que faciliten la rápida comprensión del estado de ocupación. Además, el sistema debe ser ágil, confiable y accesible desde múltiples dispositivos, garantizando una experiencia fluida y sin complicaciones. <br>

#### 1.2.2.3. Lean UX Hypothesis Statements  

A continuación, se detallan las hipótesis formuladas para abordar la problemática mediante las funcionalidades incluidas en nuestra propuesta de solución IoT. Cada hipótesis está diseñada para ser clara, cuantificable y permitir una evaluación objetiva de su éxito.

- **Hypothesis Statement 1:** <br>
    **Creemos que** los propietarios y administradores de restaurantes y cafeterías necesitan una herramienta en tiempo real que les permita monitorear la ocupación de mesas de forma automatizada. 
    <br>

    **Sabremos** que hemos tenido éxito. 
    <br>

    **Cuando** al menos el 75% de estos usuarios informen una mejora en la eficiencia operativa y una reducción del 30% en incidencias por sobreaforo.
    <br>

- **Hypothesis Statement 2:** <br>
    **Creemos que** los clientes valorarán disponer de información actualizada sobre la disponibilidad de mesas a través de una aplicación móvil y web. 
    <br>

    **Sabremos** que hemos tenido éxito. 
    <br>

    **Cuando** el 80% de los clientes reporten una experiencia mejorada y una disminución notable en los tiempos de espera al llegar al establecimiento.
    <br>

- **Hypothesis Statement 3:** <br>
    **Creemos que** la implementación de sensores IoT integrados en las mesas, que transmitan datos en tiempo real a una plataforma centralizada, facilitará la gestión del aforo y optimizará el flujo de clientes. 
    <br>

    **Sabremos** que hemos tenido éxito. 
    <br>

    **Cuando** los establecimientos vean un incremento del 25% en la eficiencia en la asignación de mesas y una recuperación de la inversión en menos de 12 meses. 
    <br>

- **Hypothesis Statement 4:** <br>
    **Creemos que** una interfaz intuitiva y amigable en la aplicación digital fomentará la adopción tanto por parte de administradores como de clientes, simplificando el proceso de toma de decisiones y la planificación de visitas. 
    <br>
    **Sabremos** que hemos tenido éxito. 
    <br>

    **Cuando** el 80% de los usuarios completen tareas básicas en la aplicación sin necesidad de asistencia y se mantenga un alto nivel de satisfacción en encuestas posteriores a su experiencia. 
    <br>

#### 1.2.2.4. Lean UX Canvas

<img src="./images/lean_ux_canvas/LEAN_UX_CANVAS.svg" alt="Lean UX Canvas"/>


## 1.3. Segmentos objetivo

Nuestros segmentos objetivo se centran en aquellos actores que se beneficiarán directamente del control automatizado del aforo y la optimización del flujo de clientes:

- **Propietarios y Administradores de Restaurantes y Cafeterías:** <br>
 Este segmento es clave, ya que busca herramientas que faciliten la gestión en tiempo real de la ocupación de mesas, reduzcan errores manuales y optimicen la operación del negocio. Son usuarios que valoran la eficiencia operativa y la posibilidad de obtener estadísticas precisas para la toma de decisiones. 
 <br>

- **Clientes de Establecimientos de Hostelería** <br>
Los clientes se benefician al contar con información actualizada sobre la disponibilidad de mesas, lo que les permite planificar su visita de manera eficiente, evitar largos tiempos de espera y disfrutar de una experiencia más cómoda y agradable.



## 4.2. Tactical-Level Domain-Driven-Design

### 4.2.1 Bounded Context: IAM Bounded Context

El **IAM (Identity and Access Management) Bounded Context** es responsable de gestionar la autenticación y la creación de usuarios en el sistema. Este contexto asegura que los usuarios puedan registrarse, iniciar sesión y gestionar sus credenciales de manera segura, cumpliendo con los estándares de seguridad y privacidad.

#### 4.2.1.1. Domain Layer

La **Domain Layer** del IAM Bounded Context encapsula la lógica de negocio relacionada con la autenticación y la gestión de usuarios. En esta capa, se definen los elementos principales del dominio, como agregados, entidades y objetos de valor, que representan los conceptos clave del sistema.

##### **Aggregates**
1. **User**
   - **Propósito**: El agregado principal es el usuario (`User`), que encapsula la lógica de negocio relacionada con la autenticación y la gestión de roles.
   - **Atributos**:
     - `username`: Identificador único del usuario, validado para cumplir con restricciones de longitud y unicidad.
     - `password`: Contraseña del usuario, almacenada de forma segura.
     - `roles`: Conjunto de roles asociados al usuario, representados como una relación `ManyToMany` con la entidad `Role`.
   - **Métodos**:
     - `addRole(Role role)`: Agrega un rol al usuario.
     - `addRoles(List<Role> roles)`: Agrega múltiples roles al usuario, validando que sean roles válidos.
   - **Características**:
     - Extiende `AuditableAbstractAggregateRoot`, lo que permite auditar cambios en los usuarios.
     - Gestiona la relación entre usuarios y roles, asegurando consistencia y validación.

##### **Entities**
1. **Role**
   - **Propósito**: La entidad `Role` representa los roles que pueden ser asignados a los usuarios.
   - **Atributos**:
     - `id`: Identificador único del rol.
     - `name`: Nombre del rol, representado como un valor enumerado (`Roles`).
   - **Métodos**:
     - `getDefaultRole()`: Devuelve el rol predeterminado (`ROLE_USER`).
     - `toRoleFromName(String name)`: Convierte un nombre de rol en una instancia de `Role`.
     - `validateRoleSet(List<Role> roles)`: Valida un conjunto de roles, asignando un rol predeterminado si el conjunto está vacío o es nulo.
   - **Características**:
     - Define una relación única entre los nombres de roles y sus representaciones en la base de datos.
     - Facilita la validación y asignación de roles a los usuarios.

##### **Value Objects**: 
1. **Roles**
   - **Propósito**: El objeto de valor `Roles` es una enumeración que define los roles disponibles en el sistema.
   - **Valores**:
     - `ROLE_ADMIN`: Rol de administrador.
     - `ROLE_SUPERVISOR`: Rol de supervisor.
     - `ROLE_USER`: Rol de usuario estándar.
   - **Características**:
     - Representa roles como valores inmutables, asegurando consistencia en su uso dentro del dominio.


En conjunto, estos elementos permiten modelar de manera robusta y segura la lógica de negocio relacionada con la autenticación y la gestión de usuarios, asegurando que las reglas del dominio se cumplan de manera consistente.

#### 4.2.1.2. Interface Layer

La **Interface Layer** del IAM Bounded Context expone los puntos de entrada al sistema a través de controladores REST. Estos controladores permiten la interacción con las entidades del dominio mediante solicitudes HTTP, facilitando la comunicación entre los clientes y el sistema. Además, esta capa incluye recursos y transformadores que aseguran una representación adecuada de los datos y su conversión entre las capas de la aplicación.

#### **Controllers**

Los controladores son responsables de manejar las solicitudes HTTP y delegar la lógica de negocio a los servicios correspondientes. A continuación, se describen los principales controladores:

1. **UsersController**
   - **Propósito**: Gestiona las operaciones relacionadas con los usuarios.
   - **Endpoints**:
     - `GET /api/v1/users`: Obtiene la lista de todos los usuarios.
     - `GET /api/v1/users/{userId}`: Obtiene los detalles de un usuario específico por su ID.
   - **Dependencias**:
     - `UserQueryService`: Servicio encargado de manejar las consultas relacionadas con los usuarios.

2. **RolesController**
   - **Propósito**: Gestiona las operaciones relacionadas con los roles.
   - **Endpoints**:
     - `GET /api/v1/roles`: Obtiene la lista de todos los roles disponibles.
   - **Dependencias**:
     - `RoleQueryService`: Servicio encargado de manejar las consultas relacionadas con los roles.

3. **AuthenticationController**
   - **Propósito**: Gestiona las operaciones de autenticación y registro de usuarios.
   - **Endpoints**:
     - `POST /api/v1/authentication/sign-up`: Registra un nuevo usuario en el sistema.
     - `POST /api/v1/authentication/sign-in`: Autentica a un usuario y genera un token de acceso.
   - **Dependencias**:
     - `UserCommandService`: Servicio encargado de manejar los comandos relacionados con los usuarios.

#### **Resources**

Los recursos representan los datos que se exponen a través de la API REST. Estos recursos son utilizados para estructurar las respuestas de los controladores y asegurar una representación clara y consistente de los datos. A continuación, se describen los principales recursos:

1. **UserResource**
   Representa un usuario en el sistema.
   - **Atributos**:
     - `id`: Identificador único del usuario.
     - `username`: Nombre de usuario.
     - `roles`: Lista de roles asociados al usuario.

1. **RoleResource**
   Representa un rol en el sistema.
   - **Atributos**:
     - `id`: Identificador único del rol.
     - `name`: Nombre del rol.

2. **AuthenticatedUserResource**
   Representa un usuario autenticado junto con su token de acceso.
   - **Atributos**:
     - `id`: Identificador único del usuario.
     - `username`: Nombre de usuario.
     - `token`: Token de acceso generado.

3. **SignUpResource**
   Representa los datos necesarios para registrar un nuevo usuario.
   - **Atributos**:
     - `username`: Nombre de usuario.
     - `password`: Contraseña.
     - `roles`: Lista de roles asignados al usuario.

4. **SignInResource**
   Representa los datos necesarios para autenticar a un usuario.
   - **Atributos**:
     - `username`: Nombre de usuario.
     - `password`: Contraseña.

#### **Transformers**

Los transformadores son responsables de convertir las entidades del dominio en recursos y viceversa. Esto asegura que los datos expuestos a través de la API REST sean consistentes y estén en el formato esperado. A continuación, se describen los principales transformadores:

1. **UserResourceFromEntityAssembler**
   Convierte una entidad `User` en un recurso `UserResource`.
   - **Método principal**:
     - `toResourceFromEntity(User entity)`: Transforma un usuario del dominio en un recurso.

1. **RoleResourceFromEntityAssembler**
   Convierte una entidad `Role` en un recurso `RoleResource`.
   - **Método principal**:
     - `toResourceFromEntity(Role entity)`: Transforma un rol del dominio en un recurso.

1. **AuthenticatedUserResourceFromEntityAssembler**
   Convierte una entidad `User` y un token en un recurso `AuthenticatedUserResource`.
   - **Método principal**:
     - `toResourceFromEntity(User entity, String token)`: Transforma un usuario autenticado en un recurso.

1. **SignUpCommandFromResourceAssembler**
   Convierte un recurso `SignUpResource` en un comando `SignUpCommand`.
   - **Método principal**:
     - `toCommandFromResource(SignUpResource resource)`: Transforma los datos de registro en un comando.

1. **SignInCommandFromResourceAssembler**
   Convierte un recurso `SignInResource` en un comando `SignInCommand`.
   - **Método principal**:
     - `toCommandFromResource(SignInResource resource)`: Transforma los datos de inicio de sesión en un comando.

#### **Relaciones entre componentes**

- Los controladores utilizan los servicios de consulta (`UserQueryService`, `RoleQueryService`) y de comandos (`UserCommandService`) para delegar la lógica de negocio.
- Los transformadores convierten las entidades del dominio en recursos para las respuestas HTTP y viceversa para las solicitudes entrantes.
- Los recursos estructuran los datos expuestos a los clientes, asegurando una representación clara y consistente.

Esta estructura asegura que la **Interface Layer** sea modular, reutilizable y fácil de mantener, facilitando la interacción entre los clientes y el sistema.

#### 4.2.1.3 Application Layer

La **Application Layer** del IAM Bounded Context actúa como un intermediario entre la **Domain Layer** y las capas externas, como la **Interface Layer** y la **Infrastructure Layer**. Su propósito principal es coordinar las operaciones de negocio, manejar comandos y consultas, y orquestar la lógica de aplicación sin exponer directamente los detalles del dominio.

#### **Command Services**
Los servicios de comandos son responsables de ejecutar operaciones que modifican el estado del sistema. A continuación, se describen los principales servicios de comandos:

1. **RoleCommandServiceImpl**
   - **Propósito**: Gestiona las operaciones relacionadas con los roles, como la creación inicial de roles en el sistema.
   - **Métodos principales**:
     - `handle(SeedRolesCommand command)`: Verifica si los roles predefinidos existen en el sistema y los crea si no están presentes.
   - **Dependencias**:
     - `RoleRepository`: Interactúa con la base de datos para verificar y guardar roles.

2. **UserCommandServiceImpl**
   - **Propósito**: Gestiona las operaciones relacionadas con los usuarios, como el registro y la autenticación.
   - **Métodos principales**:
     - `handle(SignUpCommand command)`: Registra un nuevo usuario en el sistema, asignándole roles y almacenando su contraseña de forma segura.
     - `handle(SignInCommand command)`: Autentica a un usuario verificando sus credenciales y generando un token de acceso.
   - **Dependencias**:
     - `UserRepository`: Interactúa con la base de datos para guardar y recuperar usuarios.
     - `HashingService`: Codifica y verifica contraseñas.
     - `TokenService`: Genera y valida tokens de acceso.
     - `RoleRepository`: Recupera roles asignados a los usuarios.

#### **Query Services**
Los servicios de consultas son responsables de recuperar información del sistema sin modificar su estado. A continuación, se describen los principales servicios de consultas:

1. **RoleQueryServiceImpl**
   - **Propósito**: Gestiona las consultas relacionadas con los roles.
   - **Métodos principales**:
     - `handle(GetAllRolesQuery query)`: Recupera todos los roles disponibles en el sistema.
     - `handle(GetRoleByNameQuery query)`: Recupera un rol específico por su nombre.
   - **Dependencias**:
     - `RoleRepository`: Interactúa con la base de datos para recuperar roles.

2. **UserQueryServiceImpl**
   - **Propósito**: Gestiona las consultas relacionadas con los usuarios.
   - **Métodos principales**:
     - `handle(GetAllUsersQuery query)`: Recupera todos los usuarios registrados en el sistema.
     - `handle(GetUserByIdQuery query)`: Recupera un usuario específico por su ID.
     - `handle(GetUserByUsernameQuery query)`: Recupera un usuario específico por su nombre de usuario.
   - **Dependencias**:
     - `UserRepository`: Interactúa con la base de datos para recuperar usuarios.

#### **Relaciones entre componentes**
- Los **Command Services** interactúan con los repositorios para modificar el estado del sistema y con los servicios externos para operaciones auxiliares, como el hashing de contraseñas y la generación de tokens.
- Los **Query Services** interactúan únicamente con los repositorios para recuperar información del sistema.

Esta estructura asegura que la **Application Layer** sea modular, reutilizable y fácil de mantener, permitiendo una separación clara de responsabilidades y facilitando la evolución del sistema.

#### 4.2.1.4. Infrastructure Layer 
La **Infrastructure Layer** del IAM Bounded Context proporciona las implementaciones técnicas necesarias para soportar las operaciones del sistema. Esta capa incluye configuraciones de seguridad, servicios de hashing, manejo de tokens, repositorios para la persistencia de datos y componentes relacionados con la autorización y autenticación. Su objetivo principal es conectar la lógica de negocio con los recursos externos, como bases de datos, servicios de seguridad y APIs externas.

#### **Persistencia (JPA Repositories)**

1. **RoleRepository**
   - **Propósito**: Proporciona métodos para interactuar con la base de datos de roles.
   - **Métodos principales**:
     - `findByName`: Busca un rol por su nombre.
     - `existsByName`: Verifica si un rol existe en la base de datos.

2. **UserRepository**
   - **Propósito**: Proporciona métodos para interactuar con la base de datos de usuarios.
   - **Métodos principales**:
     - `findByUsername`: Busca un usuario por su nombre de usuario.
     - `existsByUsername`: Verifica si un usuario existe en la base de datos.

#### **Relaciones entre componentes**
   - **Persistencia**: Los repositorios (`RoleRepository`, `UserRepository`) proporcionan acceso a los datos almacenados en la base de datos, permitiendo a las capas superiores interactuar con las entidades del dominio.

Esta estructura asegura que la **Infrastructure Layer** sea modular, reutilizable y fácil de mantener, facilitando la integración con otros sistemas y servicios externos.

#### 4.2.1.5. Bounded Context Software Architecture Component Level Diagrams

En esta sección se presenta el diagrama de componentes del **IAM Bounded Context**, el cual detalla los principales módulos y sus interacciones dentro del contexto delimitado. Este diagrama sigue el enfoque del C4 Model para representar los componentes clave, como servicios de aplicación, controladores, repositorios y servicios externos, junto con sus relaciones.

El propósito de este diagrama es proporcionar una visión clara y estructurada de cómo se organizan los componentes dentro del contexto, facilitando la comprensión de su arquitectura y permitiendo identificar puntos de integración y responsabilidades.

El **IAM Bounded Context** está compuesto por los siguientes módulos principales:

1. **Application Layer**:
   - Coordina las operaciones de negocio relacionadas con la autenticación y la gestión de usuarios.
   - Incluye servicios de comandos y consultas que interactúan con la **Domain Layer** y la **Infrastructure Layer**.
   - Maneja eventos relacionados con el registro de usuarios, la asignación de roles y la autenticación.

2. **Interface Layer**:
   - Expone los puntos de entrada al sistema a través de controladores REST.
   - Incluye recursos y transformadores que aseguran una representación adecuada de los datos y su conversión entre las capas de la aplicación.
   - Proporciona endpoints para operaciones como el registro de usuarios, la autenticación y la consulta de roles.

3. **Domain Layer**:
   - Encapsula la lógica de negocio relacionada con la autenticación y la gestión de usuarios.
   - Define los agregados, entidades y objetos de valor que representan los conceptos clave del dominio, como usuarios, roles y permisos.
   - Asegura que las reglas de negocio, como la validación de contraseñas y la asignación de roles, se cumplan de manera consistente.

4. **Infrastructure Layer**:
   - Proporciona las implementaciones técnicas necesarias para soportar las operaciones del sistema.
   - Incluye repositorios para la persistencia de datos y componentes que conectan la lógica de negocio con los recursos externos, como bases de datos y servicios de seguridad.
   - Implementa servicios auxiliares como el hashing de contraseñas y la generación de tokens de autenticación.

<img src="./images/c4-model/bc-component-diagram/IOT-IAM-BC-Component-Diagram.svg" alt="IAM BC Component Diagram"/><br>


#### 4.2.1.6. Bounded Context Software Architecture Code Level Diagrams

En este apartado se presentan los diagramas que ofrecen un mayor nivel de detalle sobre la implementación de los componentes del **IAM Bounded Context**. Estos diagramas están diseñados para ilustrar cómo se estructuran las clases, interfaces y relaciones dentro de las capas del contexto, proporcionando una visión técnica que facilita el desarrollo, mantenimiento y evolución del sistema.

##### 4.2.1.6.1. Bounded Context Domain Layer Class Diagrams

El diagrama de clases correspondiente a la **Domain Layer** del **IAM Bounded Context** incluye las clases principales, como agregados, entidades y objetos de valor, así como las interfaces y enumeraciones que definen el comportamiento del dominio. También se destacan las relaciones entre estos elementos, como asociaciones, composiciones y dependencias.

**Elementos principales del diagrama:**

1. **Aggregates**:
   - `User`: Agregado principal que encapsula la lógica de negocio relacionada con la autenticación y la gestión de usuarios. Incluye atributos como `username`, `password` y `roles`.
     - **Atributos**:
       - `username`: Identificador único del usuario.
       - `password`: Contraseña almacenada de forma segura.
       - `roles`: Lista de roles asignados al usuario.
     - **Métodos**:
       - `addRole(Role role)`: Agrega un rol al usuario.
       - `addRoles(List<Role> roles)`: Agrega múltiples roles al usuario, validando que sean válidos.

2. **Entities**:
   - `Role`: Representa los roles que pueden ser asignados a los usuarios.
     - **Atributos**:
       - `id`: Identificador único del rol.
       - `name`: Nombre del rol.
     - **Métodos**:
       - `getDefaultRole()`: Devuelve el rol predeterminado (`ROLE_USER`).
       - `validateRoleSet(List<Role> roles)`: Valida un conjunto de roles asignados.

3. **Value Objects**:
   - `Roles`: Enumeración que define los roles disponibles en el sistema (`ROLE_ADMIN`, `ROLE_SUPERVISOR`, `ROLE_USER`).
   - `Password`: Representa la contraseña del usuario, asegurando que cumpla con las políticas de seguridad.
   - `Token`: Representa un token de autenticación generado para un usuario.

**Relaciones destacadas:**
- El agregado `User` gestiona las relaciones con la entidad `Role`, asegurando que los usuarios tengan roles válidos asignados.
- Los objetos de valor encapsulan datos inmutables y validaciones específicas, como la seguridad de contraseñas y la unicidad de roles.
- La entidad `Role` define los permisos y responsabilidades que pueden ser asignados a los usuarios.

<img src="./images/c4-model/class-diagram/IAM_domain_class_diagram.webp" alt="IAM BC Domain Layer Class Diagram"/><br>

##### 4.2.1.6.2. Bounded Context Database Design Diagram.


### 4.2.3 Bounded Context: Branching Bounded Context

El **Branching Bounded Context** es responsable de gestionar la información de las sedes (headquarters) del sistema Tavolo. Este contexto asegura que las sedes puedan ser registradas, actualizadas y gestionadas de manera eficiente, incluyendo detalles como horarios de atención, ubicación geográfica, información de contacto y dirección. Este contexto es clave para garantizar que las operaciones relacionadas con las sedes sean consistentes y cumplan con los estándares de calidad y precisión requeridos.

#### 4.2.3.1. Domain Layer

La **Domain Layer** del Branching Bounded Context encapsula la lógica de negocio relacionada con la gestión de sedes. En esta capa, se definen los elementos principales del dominio, como agregados, entidades y objetos de valor, que representan los conceptos clave del sistema.

La **Domain Layer** del Branching Bounded Context encapsula la lógica de negocio relacionada con la gestión de sedes. En esta capa, se definen los elementos principales del dominio, como agregados, entidades y objetos de valor, que representan los conceptos clave del sistema.

##### **Aggregates**
1. **Headquarter**
   - **Propósito**: El agregado principal es la sede (`Headquarter`), que encapsula la lógica de negocio relacionada con la gestión de información de las sedes.
   - **Atributos**:
     - `name`: Nombre de la sede, representado como un objeto de valor `NameHeadquarter`.
     - `contactNumbers`: Números de contacto de la sede, representados como un objeto de valor `ContactNumbers`.
     - `coordinates`: Coordenadas geográficas de la sede, representadas como un objeto de valor `Coordinates`.
     - `schedule`: Horarios de atención de la sede, representados como una entidad `Schedule`.
     - `address`: Dirección de la sede, representada como un objeto de valor `StreetAddress`.
   - **Métodos**:
     - `getOpeningTime()`: Devuelve la hora de apertura de la sede.
     - `getClosingTime()`: Devuelve la hora de cierre de la sede.
     - `getIntervalMinutes()`: Devuelve el intervalo de tiempo en minutos entre reservas.
   - **Características**:
     - Extiende `AuditableAbstractAggregateRoot`, lo que permite auditar cambios en las sedes.
     - Gestiona la relación entre los horarios, la dirección y los datos de contacto de la sede, asegurando consistencia y validación.

##### **Entities**
1. **Schedule**
   - **Propósito**: Representa los horarios de atención de una sede.
   - **Atributos**:
     - `businessHours`: Horarios de apertura y cierre, representados como un objeto de valor `BusinessHours`.
     - `intervalMinutes`: Intervalo de tiempo en minutos entre reservas.
   - **Características**:
     - Permite definir y validar los horarios de atención de la sede.
     - Incluye validaciones para garantizar que los horarios sean consistentes (por ejemplo, la hora de apertura no puede ser posterior a la hora de cierre).

##### **Value Objects**
1. **BusinessHours**
   - **Propósito**: Representa los horarios de apertura y cierre de una sede.
   - **Atributos**:
     - `openingTime`: Hora de apertura.
     - `closingTime`: Hora de cierre.
   - **Validaciones**:
     - La hora de apertura no puede ser nula.
     - La hora de cierre no puede ser nula.
     - La hora de apertura no puede ser posterior a la hora de cierre.

2. **ContactNumbers**
   - **Propósito**: Representa los números de contacto de una sede.
   - **Atributos**:
     - `landlinePhone`: Número de teléfono fijo.
     - `mobilePhone`: Número de teléfono móvil.
   - **Validaciones**:
     - Ambos números deben ser válidos y no nulos.

3. **Coordinates**
   - **Propósito**: Representa las coordenadas geográficas de una sede.
   - **Atributos**:
     - `latitude`: Latitud de la sede.
     - `longitude`: Longitud de la sede.
   - **Validaciones**:
     - La latitud y la longitud no pueden ser nulas.

4. **NameHeadquarter**
   - **Propósito**: Representa el nombre de una sede.
   - **Atributos**:
     - `name`: Nombre de la sede.
   - **Validaciones**:
     - El nombre no puede ser nulo ni vacío.
     - El nombre debe cumplir con un formato válido (solo letras y espacios).

5. **StreetAddress**
   - **Propósito**: Representa la dirección de una sede.
   - **Atributos**:
     - `street`: Calle.
     - `number`: Número de la dirección.
     - `city`: Ciudad.
     - `postalCode`: Código postal.
     - `country`: País.
   - **Validaciones**:
     - Los campos `street`, `city`, `postalCode` y `country` no pueden ser nulos ni vacíos.
     - La calle debe cumplir con un formato válido (solo letras, espacios y puntos).


#### **Relaciones entre componentes**
- El agregado `Headquarter` actúa como el núcleo del dominio, gestionando las relaciones con los objetos de valor (`NameHeadquarter`, `ContactNumbers`, `Coordinates`, `StreetAddress`) y la entidad `Schedule`.
- Los objetos de valor encapsulan datos inmutables y validaciones específicas, asegurando consistencia en el dominio.
- La entidad `Schedule` permite modelar horarios complejos, incluyendo intervalos de tiempo entre reservas.

Esta estructura asegura que la lógica de negocio relacionada con la gestión de sedes sea robusta, consistente y fácil de mantener, cumpliendo con los requisitos del sistema.

#### 4.2.3.2. Interface Layer

La **Interface Layer** del Branching Bounded Context expone los puntos de entrada al sistema a través de controladores REST y una ACL (Access Control Layer). Esta capa permite la interacción con las entidades del dominio mediante solicitudes HTTP, facilitando la comunicación entre los clientes y el sistema. Además, incluye recursos y transformadores que aseguran una representación adecuada de los datos y su conversión entre las capas de la aplicación.

#### **Access Control Layer (ACL)**

1. **HeadquarterContextFacade**
   - **Propósito**: Proporciona una interfaz simplificada para interactuar con el dominio del Branching Bounded Context desde otros contextos. Permite consultar información clave de las sedes, como horarios de apertura y cierre, intervalos de servicio y existencia de una sede.
   - **Métodos principales**:
     - `getOpeningTime(Long headquarterId)`: Devuelve la hora de apertura de una sede.
     - `getClosingTime(Long headquarterId)`: Devuelve la hora de cierre de una sede.
     - `getIntervalMinutes(Long headquarterId)`: Devuelve el intervalo de servicio en minutos de una sede.
     - `existsHeadquarter(Long headquarterId)`: Verifica si una sede existe en el sistema.
   - **Dependencias**:
     - `HeadquarterQueryService`: Servicio encargado de manejar las consultas relacionadas con las sedes.


#### **Controllers**

Los controladores son responsables de manejar las solicitudes HTTP y delegar la lógica de negocio a los servicios correspondientes. A continuación, se describen los principales controladores:

1. **HeadquarterController**
   - **Propósito**: Gestiona las operaciones relacionadas con las sedes.
   - **Endpoints**:
     - `POST /api/v1/headquarters`: Crea una nueva sede.
     - `GET /api/v1/headquarters/{headquarterId}`: Obtiene los detalles de una sede específica por su ID.
     - `GET /api/v1/headquarters`: Obtiene la lista de todas las sedes.
   - **Dependencias**:
     - `HeadquarterCommandService`: Servicio encargado de manejar los comandos relacionados con las sedes.
     - `HeadquarterQueryService`: Servicio encargado de manejar las consultas relacionadas con las sedes.


#### **Resources**

Los recursos representan los datos que se exponen a través de la API REST. Estos recursos son utilizados para estructurar las respuestas de los controladores y asegurar una representación clara y consistente de los datos. A continuación, se describen los principales recursos:

1. **CreateHeadquarterResource**
   - **Propósito**: Representa los datos necesarios para crear una nueva sede.
   - **Atributos**:
     - `name`: Nombre de la sede.
     - `landlinePhone`: Número de teléfono fijo.
     - `mobilePhone`: Número de teléfono móvil.
     - `latitude`: Latitud de la sede.
     - `longitude`: Longitud de la sede.
     - `street`: Calle de la dirección.
     - `number`: Número de la dirección.
     - `city`: Ciudad.
     - `postalCode`: Código postal.
     - `country`: País.
     - `openingTime`: Hora de apertura.
     - `closingTime`: Hora de cierre.
     - `intervalMinutes`: Intervalo de servicio en minutos.

2. **HeadquarterResource**
   - **Propósito**: Representa una sede en el sistema.
   - **Atributos**:
     - `id`: Identificador único de la sede.
     - `name`: Nombre de la sede.
     - `landlinePhone`: Número de teléfono fijo.
     - `mobilePhone`: Número de teléfono móvil.
     - `latitude`: Latitud de la sede.
     - `longitude`: Longitud de la sede.
     - `streetAddress`: Dirección completa de la sede.
     - `openingTime`: Hora de apertura.
     - `closingTime`: Hora de cierre.
     - `intervalMinutes`: Intervalo de servicio en minutos.

#### **Transformers**

Los transformadores son responsables de convertir las entidades del dominio en recursos y viceversa. Esto asegura que los datos expuestos a través de la API REST sean consistentes y estén en el formato esperado. A continuación, se describen los principales transformadores:

1. **CreateHeadquarterCommandFromResourceAssembler**
   - **Propósito**: Convierte un recurso `CreateHeadquarterResource` en un comando `CreateHeadquarterCommand`.
   - **Método principal**:
     - `toCommandFromResource(CreateHeadquarterResource resource)`: Transforma los datos de creación de una sede en un comando.

2. **HeadquarterResourceFromEntityAssembler**
   - **Propósito**: Convierte una entidad `Headquarter` en un recurso `HeadquarterResource`.
   - **Método principal**:
     - `toResourceFromEntity(Headquarter entity)`: Transforma una sede del dominio en un recurso.

#### **Relaciones entre componentes**

- El **HeadquarterController** utiliza los servicios de comandos (`HeadquarterCommandService`) y consultas (`HeadquarterQueryService`) para delegar la lógica de negocio.
- La **ACL (HeadquarterContextFacade)** proporciona una interfaz simplificada para consultar información clave de las sedes desde otros contextos.
- Los transformadores convierten las entidades del dominio en recursos para las respuestas HTTP y viceversa para las solicitudes entrantes.
- Los recursos estructuran los datos expuestos a los clientes, asegurando una representación clara y consistente.

Esta estructura asegura que la **Interface Layer** sea modular, reutilizable y fácil de mantener, facilitando la interacción entre los clientes y el sistema.

#### 4.2.3.4. Infrastructure Layer

La **Infrastructure Layer** del Branching Bounded Context proporciona las implementaciones técnicas necesarias para soportar las operaciones del sistema relacionadas con la gestión de sedes. Esta capa incluye repositorios para la persistencia de datos y componentes que conectan la lógica de negocio con los recursos externos, como bases de datos. Su objetivo principal es garantizar que las operaciones de almacenamiento y recuperación de información sean eficientes, consistentes y seguras.

#### **Persistencia (JPA Repositories)**

1. **HeadquarterRepository**
   - **Propósito**: Proporciona métodos para interactuar con la base de datos de sedes.
   - **Métodos principales**:
     - `existsByName(NameHeadquarter name)`: Verifica si existe una sede con un nombre específico.
     - `existsByCoordinates(Coordinates coordinates)`: Verifica si existe una sede en una ubicación geográfica específica.
   - **Características**:
     - Extiende `JpaRepository`, lo que permite realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre las entidades `Headquarter`.
     - Facilita la validación de unicidad para nombres y coordenadas de sedes, asegurando que no haya duplicados en el sistema.


#### **Relaciones entre componentes**

- **Persistencia**: El repositorio `HeadquarterRepository` proporciona acceso a los datos almacenados en la base de datos, permitiendo a las capas superiores (como la **Application Layer**) interactuar con las entidades del dominio.
- **Validación**: Los métodos `existsByName` y `existsByCoordinates` son utilizados para validar la unicidad de las sedes durante las operaciones de creación o actualización, asegurando la consistencia de los datos.


La **Infrastructure Layer** del Branching Bounded Context asegura que las operaciones relacionadas con la persistencia de datos sean robustas y confiables. Al proporcionar un repositorio especializado para las sedes, esta capa facilita la integración con la base de datos y garantiza que las reglas de negocio, como la unicidad de nombres y ubicaciones, se cumplan de manera eficiente. Esta estructura modular y reutilizable permite que el sistema sea escalable y fácil de mantener.

#### 4.2.3.5. Bounded Context Software Architecture Component Level Diagrams

En esta sección se presenta el diagrama de componentes del **Branching Bounded Context**, el cual detalla los principales módulos y sus interacciones dentro del contexto delimitado. Este diagrama sigue el enfoque del C4 Model para representar los componentes clave, como servicios de aplicación, controladores, repositorios y servicios externos, junto con sus relaciones.

El propósito de este diagrama es proporcionar una visión clara y estructurada de cómo se organizan los componentes dentro del contexto, facilitando la comprensión de su arquitectura y permitiendo identificar puntos de integración y responsabilidades. 

El **Branching Bounded Context** está compuesto por los siguientes módulos principales:

1. **Application Layer**:
   - Coordina las operaciones de negocio relacionadas con la gestión de sedes.
   - Incluye servicios de comandos y consultas que interactúan con la **Domain Layer** y la **Infrastructure Layer**.
   - Maneja eventos relacionados con la creación y actualización de sedes.

2. **Interface Layer**:
   - Expone los puntos de entrada al sistema a través de controladores REST.
   - Incluye recursos y transformadores que aseguran una representación adecuada de los datos y su conversión entre las capas de la aplicación.

3. **Domain Layer**:
   - Encapsula la lógica de negocio relacionada con la gestión de sedes.
   - Define los agregados, entidades y objetos de valor que representan los conceptos clave del dominio.

4. **Infrastructure Layer**:
   - Proporciona las implementaciones técnicas necesarias para soportar las operaciones del sistema.
   - Incluye repositorios para la persistencia de datos y componentes que conectan la lógica de negocio con los recursos externos, como bases de datos.

<img src="./images/c4-model/bc-component-diagram/IOT-Braching-BC-Component-Diagram.svg" alt="Branching BC Component Diagram"/><br>

#### 4.2.3.6. Bounded Context Software Architecture Code Level Diagrams

En este apartado se presentan los diagramas que ofrecen un mayor nivel de detalle sobre la implementación de los componentes del **Branching Bounded Context**. Estos diagramas están diseñados para ilustrar cómo se estructuran las clases, interfaces y relaciones dentro de las capas del contexto, proporcionando una visión técnica que facilita el desarrollo, mantenimiento y evolución del sistema.

##### 4.2.3.6.1. Bounded Context Domain Layer Class Diagrams

El diagrama de clases correspondiente a la **Domain Layer** del **Branching Bounded Context** incluye las clases principales, como agregados, entidades y objetos de valor, así como las interfaces y enumeraciones que definen el comportamiento del dominio. También se destacan las relaciones entre estos elementos, como asociaciones, composiciones y dependencias.

El objetivo de este diagrama es proporcionar una representación detallada de la lógica de negocio encapsulada en la capa del dominio, asegurando que las reglas del negocio estén claramente definidas y alineadas con los requisitos del sistema.

**Elementos principales del diagrama:**

1. **Aggregates**:
   - `Headquarter`: Agregado principal que encapsula la lógica de negocio relacionada con la gestión de sedes. Incluye atributos como `name`, `contactNumbers`, `coordinates`, `schedule` y `address`.

2. **Entities**:
   - `Schedule`: Representa los horarios de atención de una sede, incluyendo atributos como `businessHours` e `intervalMinutes`.

3. **Value Objects**:
   - `NameHeadquarter`: Representa el nombre de una sede.
   - `ContactNumbers`: Representa los números de contacto de una sede.
   - `Coordinates`: Representa las coordenadas geográficas de una sede.
   - `StreetAddress`: Representa la dirección de una sede.
   - `BusinessHours`: Representa los horarios de apertura y cierre de una sede.

**Relaciones destacadas:**
- El agregado `Headquarter` actúa como el núcleo del dominio, gestionando las relaciones con los objetos de valor (`NameHeadquarter`, `ContactNumbers`, `Coordinates`, `StreetAddress`) y la entidad `Schedule`.
- Los objetos de valor encapsulan datos inmutables y validaciones específicas, asegurando consistencia en el dominio.
- La entidad `Schedule` permite modelar horarios complejos, incluyendo intervalos de tiempo entre reservas.

<img src="./images/c4-model/class-diagram/branching_domain_class_diagram.webp" alt="Branching BC Domain Layer Class Diagram"/><br>

##### 4.2.3.6.2. Bounded Context Database Design Diagram.


### 4.2.4 Bounded Context: Booking Bounded Context

El **Booking Bounded Context** es responsable de gestionar las reservas de mesas en el sistema Tavolo. Este contexto asegura que los usuarios puedan realizar reservas de manera eficiente, gestionando la disponibilidad de mesas, horarios y slots de tiempo. Además, permite a los administradores supervisar y gestionar las reservas activas, asegurando que las operaciones relacionadas con las reservas sean consistentes y cumplan con los estándares de calidad y precisión requeridos.

#### 4.2.4.1. Domain Layer

La **Domain Layer** del Booking Bounded Context encapsula la lógica de negocio relacionada con la gestión de reservas. En esta capa, se definen los elementos principales del dominio, como agregados, entidades, objetos de valor, comandos, consultas y eventos, que representan los conceptos clave del sistema.

#### **Aggregates**

1. **Booking**
   - **Propósito**: Representa una reserva realizada por un cliente para una mesa específica en una fecha y horario determinado.
   - **Atributos**:
     - `userId`: Identificador del cliente que realiza la reserva, representado como un objeto de valor `UserId`.
     - `tableId`: Mesa reservada, representada como una referencia a la entidad `Table`.
     - `bookingDate`: Fecha de la reserva.
     - `bookingSlots`: Conjunto de intervalos de tiempo reservados, representados como una colección de entidades `BookingSlot`.
   - **Características**:
     - Extiende `AuditableAbstractAggregateRoot`, lo que permite auditar cambios en las reservas.
     - Gestiona la relación entre el cliente, la mesa y los slots reservados, asegurando consistencia y validación.

2. **Table**
   - **Propósito**: Representa una mesa en una sede específica, incluyendo su disponibilidad y detalles.
   - **Atributos**:
     - `tableDetails`: Detalles de la mesa, como número de mesa y cantidad de asientos, representados como un objeto de valor `TableDetails`.
     - `headquarterId`: Identificador de la sede a la que pertenece la mesa, representado como un objeto de valor `HeadquarterId`.
     - `status`: Estado actual de la mesa (`AVAILABLE`, `RESERVED`, `OCCUPIED`), representado como un objeto de valor `TableStatus`.
     - `availabilitySlots`: Conjunto de slots de disponibilidad generados para la mesa, representados como una colección de entidades `AvailabilitySlot`.
   - **Características**:
     - Extiende `AuditableAbstractAggregateRoot`, lo que permite auditar cambios en las mesas.
     - Gestiona la generación y actualización de slots de disponibilidad.

#### **Entities**

1. **AvailabilitySlot**
   - **Propósito**: Representa un intervalo de tiempo disponible para una mesa en una fecha específica.
   - **Atributos**:
     - `dateOfSlot`: Fecha del slot.
     - `timeInterval`: Intervalo de tiempo del slot, representado como un objeto de valor `TimeSlot`.
     - `status`: Estado del slot (`AVAILABLE`, `RESERVED`), representado como un objeto de valor `ScheduleSlotStatus`.
   - **Métodos**:
     - `updateStatus(ScheduleSlotStatus status)`: Actualiza el estado del slot.

2. **BookingSlot**
   - **Propósito**: Representa un intervalo de tiempo reservado por un cliente.
   - **Atributos**:
     - `timeInterval`: Intervalo de tiempo reservado, representado como un objeto de valor `TimeSlot`.

#### **Value Objects**

1. **UserId**
   - **Propósito**: Representa el identificador único de un cliente.
   - **Validaciones**:
     - El identificador no puede ser negativo.

2. **HeadquarterId**
   - **Propósito**: Representa el identificador único de una sede.
   - **Validaciones**:
     - El identificador no puede ser nulo ni negativo.

3. **TableDetails**
   - **Propósito**: Representa los detalles de una mesa, como su número y cantidad de asientos.
   - **Validaciones**:
     - El número de mesa no puede ser negativo.
     - La cantidad de asientos debe ser mayor a cero.

4. **TableStatus**
   - **Propósito**: Enumera los estados posibles de una mesa (`AVAILABLE`, `RESERVED`, `OCCUPIED`).

5. **TimeSlot**
   - **Propósito**: Representa un intervalo de tiempo con una hora de inicio y una hora de fin.
   - **Validaciones**:
     - La hora de inicio y la hora de fin no pueden ser nulas.
     - La hora de inicio debe ser anterior a la hora de fin.

6. **ScheduleSlotStatus**
   - **Propósito**: Enumera los estados posibles de un slot de disponibilidad (`AVAILABLE`, `RESERVED`).

7. **MaximumDuration**
   - **Propósito**: Representa la duración máxima permitida para una reserva.
   - **Validaciones**:
     - La duración debe ser un número positivo.
     - La duración no puede exceder las 5 horas.

#### **Commands**

1. **CreateBookingCommand**
   - **Propósito**: Representa la solicitud para crear una nueva reserva.
   - **Atributos**:
     - `clientId`: Identificador del cliente.
     - `tableId`: Identificador de la mesa.
     - `bookingDate`: Fecha de la reserva.
     - `slotIds`: Lista de identificadores de slots reservados.

2. **CreateTableCommand**
   - **Propósito**: Representa la solicitud para crear una nueva mesa.
   - **Atributos**:
     - `tableNumber`: Número de la mesa.
     - `seats`: Cantidad de asientos.
     - `headquartersId`: Identificador de la sede.

3. **CreateTableScheduleCommand**
   - **Propósito**: Representa la solicitud para generar los slots de disponibilidad de una mesa.
   - **Atributos**:
     - `tableId`: Identificador de la mesa.

#### **Queries**

1. **GetAllBookingsQuery**
   - **Propósito**: Recupera todas las reservas registradas en el sistema.

2. **GetAllTablesQuery**
   - **Propósito**: Recupera todas las mesas registradas en el sistema.

3. **GetBookingByIdQuery**
   - **Propósito**: Recupera una reserva específica por su identificador.

4. **GetTableByIdQuery**
   - **Propósito**: Recupera una mesa específica por su identificador.

5. **GetTableScheduleByIdAndDateQuery**
   - **Propósito**: Recupera los slots de disponibilidad de una mesa para una fecha específica.

#### **Events**

1. **SingleTableAvailabilitySlotsGeneratedEvent**
   - **Propósito**: Evento que se dispara cuando se generan los slots de disponibilidad para una mesa.
   - **Atributos**:
     - `tableId`: Identificador de la mesa.

#### **Relaciones entre componentes**

- El agregado `Booking` actúa como el núcleo del dominio, gestionando las relaciones con las entidades `BookingSlot` y `Table`.
- El agregado `Table` gestiona la generación y actualización de los slots de disponibilidad (`AvailabilitySlot`).
- Los objetos de valor encapsulan datos inmutables y validaciones específicas, asegurando consistencia en el dominio.
- Los comandos y consultas permiten interactuar con el sistema de manera estructurada, facilitando la creación de reservas y la recuperación de información.
- Los eventos aseguran que las operaciones críticas, como la generación de slots de disponibilidad, sean comunicadas de manera eficiente a otros componentes del sistema.

Esta estructura asegura que la lógica de negocio relacionada con la gestión de reservas sea robusta, consistente y fácil de mantener, cumpliendo con los requisitos del sistema.

#### 4.2.4.2. Interface Layer

La **Interface Layer** del Booking Bounded Context expone los puntos de entrada al sistema a través de controladores REST. Esta capa permite la interacción con las entidades del dominio mediante solicitudes HTTP, facilitando la comunicación entre los clientes y el sistema. Además, incluye recursos y transformadores que aseguran una representación adecuada de los datos y su conversión entre las capas de la aplicación.

#### **Controllers**

Los controladores son responsables de manejar las solicitudes HTTP y delegar la lógica de negocio a los servicios correspondientes. A continuación, se describen los principales controladores:

1. **BookingController**
   - **Propósito**: Gestiona las operaciones relacionadas con las reservas.
   - **Endpoints**:
     - `POST /api/v1/bookings`: Crea una nueva reserva.
     - `GET /api/v1/bookings/{id}`: Obtiene los detalles de una reserva específica por su ID.
     - `GET /api/v1/bookings`: Obtiene la lista de todas las reservas.
   - **Dependencias**:
     - `BookingCommandService`: Servicio encargado de manejar los comandos relacionados con las reservas.
     - `BookingQueryService`: Servicio encargado de manejar las consultas relacionadas con las reservas.

2. **TableController**
   - **Propósito**: Gestiona las operaciones relacionadas con las mesas.
   - **Endpoints**:
     - `POST /api/v1/tables`: Crea una nueva mesa.
     - `GET /api/v1/tables/{tableId}`: Obtiene los detalles de una mesa específica por su ID.
     - `GET /api/v1/tables`: Obtiene la lista de todas las mesas.
     - `GET /api/v1/tables/{tableId}/schedule`: Obtiene los slots de disponibilidad de una mesa para una fecha específica.
   - **Dependencias**:
     - `TableCommandService`: Servicio encargado de manejar los comandos relacionados con las mesas.
     - `TableQueryService`: Servicio encargado de manejar las consultas relacionadas con las mesas.

#### **Resources**

Los recursos representan los datos que se exponen a través de la API REST. Estos recursos son utilizados para estructurar las respuestas de los controladores y asegurar una representación clara y consistente de los datos. A continuación, se describen los principales recursos:

1. **AvailabilitySlotResource**
   - **Propósito**: Representa un slot de disponibilidad de una mesa.
   - **Atributos**:
     - `id`: Identificador único del slot.
     - `date`: Fecha del slot.
     - `startTime`: Hora de inicio del slot.
     - `endTime`: Hora de fin del slot.
     - `status`: Estado del slot (`AVAILABLE`, `RESERVED`).

2. **BookingResource**
   - **Propósito**: Representa una reserva en el sistema.
   - **Atributos**:
     - `id`: Identificador único de la reserva.
     - `clientId`: Identificador del cliente que realizó la reserva.
     - `tableId`: Identificador de la mesa reservada.
     - `bookingDate`: Fecha de la reserva.
     - `bookingSlots`: Lista de slots reservados.

3. **BookingSlotResource**
   - **Propósito**: Representa un slot reservado por un cliente.
   - **Atributos**:
     - `startTime`: Hora de inicio del slot reservado.
     - `endTime`: Hora de fin del slot reservado.

4. **CreateBookingResource**
   - **Propósito**: Representa los datos necesarios para crear una nueva reserva.
   - **Atributos**:
     - `clientId`: Identificador del cliente.
     - `tableId`: Identificador de la mesa.
     - `bookingDate`: Fecha de la reserva.
     - `slotIds`: Lista de identificadores de slots reservados.

5. **CreateTableResource**
   - **Propósito**: Representa los datos necesarios para crear una nueva mesa.
   - **Atributos**:
     - `headquarterId`: Identificador de la sede a la que pertenece la mesa.
     - `tableNumber`: Número de la mesa.
     - `seats`: Cantidad de asientos.

6. **TableResource**
   - **Propósito**: Representa una mesa en el sistema.
   - **Atributos**:
     - `id`: Identificador único de la mesa.
     - `headquarterId`: Identificador de la sede a la que pertenece la mesa.
     - `tableNumber`: Número de la mesa.
     - `seats`: Cantidad de asientos.
     - `status`: Estado actual de la mesa (`AVAILABLE`, `RESERVED`, `OCCUPIED`).

#### **Transformers**

Los transformadores son responsables de convertir las entidades del dominio en recursos y viceversa. Esto asegura que los datos expuestos a través de la API REST sean consistentes y estén en el formato esperado. A continuación, se describen los principales transformadores:

1. **AvailabilitySlotResourceFromEntityAssembler**
   - **Propósito**: Convierte una entidad `AvailabilitySlot` en un recurso `AvailabilitySlotResource`.
   - **Métodos principales**:
     - `toResourceFromEntity(AvailabilitySlot entity)`: Transforma un slot de disponibilidad en un recurso.
     - `toResourceListFromEntities(List<AvailabilitySlot> entities)`: Transforma una lista de slots de disponibilidad en una lista de recursos.

2. **BookingResourceFromEntityAssembler**
   - **Propósito**: Convierte una entidad `Booking` en un recurso `BookingResource`.
   - **Método principal**:
     - `toResourceFromEntity(Booking booking)`: Transforma una reserva en un recurso.

3. **CreateBookingCommandFromResourceAssembler**
   - **Propósito**: Convierte un recurso `CreateBookingResource` en un comando `CreateBookingCommand`.
   - **Método principal**:
     - `toCommandFromResource(CreateBookingResource resource)`: Transforma los datos de creación de una reserva en un comando.

4. **CreateTableCommandFromResourceAssembler**
   - **Propósito**: Convierte un recurso `CreateTableResource` en un comando `CreateTableCommand`.
   - **Método principal**:
     - `toCommandFromResource(CreateTableResource resource)`: Transforma los datos de creación de una mesa en un comando.

5. **TableResourceFromEntityAssembler**
   - **Propósito**: Convierte una entidad `Table` en un recurso `TableResource`.
   - **Método principal**:
     - `toResourceFromEntity(Table entity)`: Transforma una mesa en un recurso.

#### **Relaciones entre componentes**

- Los controladores (`BookingController`, `TableController`) utilizan los servicios de comandos y consultas para delegar la lógica de negocio.
- Los transformadores convierten las entidades del dominio en recursos para las respuestas HTTP y viceversa para las solicitudes entrantes.
- Los recursos estructuran los datos expuestos a los clientes, asegurando una representación clara y consistente.

Esta estructura asegura que la **Interface Layer** sea modular, reutilizable y fácil de mantener, facilitando la interacción entre los clientes y el sistema.

#### 4.2.4.3. Application Layer

La **Application Layer** del Booking Bounded Context actúa como un intermediario entre la **Domain Layer** y las capas externas, como la **Interface Layer** y la **Infrastructure Layer**. Su propósito principal es coordinar las operaciones de negocio, manejar comandos y consultas, orquestar la lógica de aplicación y garantizar que las reglas del dominio se cumplan de manera consistente. Además, esta capa incluye manejadores de eventos y servicios externos (ACL) para interactuar con otros contextos delimitados.

#### **Command Services**

Los servicios de comandos son responsables de ejecutar operaciones que modifican el estado del sistema. A continuación, se describen los principales servicios de comandos:

1. **BookingCommandServiceImpl**
   - **Propósito**: Gestiona las operaciones relacionadas con la creación de reservas.
   - **Métodos principales**:
     - `handle(CreateBookingCommand command)`: Crea una nueva reserva, validando la disponibilidad de los slots y asegurando que las reglas de negocio, como la duración máxima de la reserva, se cumplan.
   - **Validaciones**:
     - Verifica que el cliente exista utilizando el servicio externo `ExternalUserService`.
     - Valida que los slots solicitados estén disponibles y sean consecutivos.
     - Asegura que la duración total de la reserva no exceda las 2 horas.
   - **Dependencias**:
     - `BookingRepository`: Persistencia de reservas.
     - `TableRepository`: Gestión de mesas y sus slots de disponibilidad.
     - `ExternalUserService`: Verifica la existencia del cliente.

2. **TableCommandServiceImpl**
   - **Propósito**: Gestiona las operaciones relacionadas con la creación de mesas y la generación de slots de disponibilidad.
   - **Métodos principales**:
     - `handle(CreateTableCommand command)`: Crea una nueva mesa en una sede específica, validando que la sede exista y que no haya duplicados.
     - `handle(CreateTableScheduleCommand command)`: Genera los slots de disponibilidad para una mesa, basándose en los horarios y el intervalo de la sede.
   - **Validaciones**:
     - Verifica que la sede exista utilizando el servicio externo `ExternalHeadquarterService`.
     - Asegura que no existan mesas duplicadas en la misma sede.
   - **Dependencias**:
     - `TableRepository`: Persistencia de mesas y sus slots de disponibilidad.
     - `ExternalHeadquarterService`: Obtiene información de la sede, como horarios y intervalos.

#### **Query Services**

Los servicios de consultas son responsables de recuperar información del sistema sin modificar su estado. A continuación, se describen los principales servicios de consultas:

1. **BookingQueryServiceImpl**
   - **Propósito**: Gestiona las consultas relacionadas con las reservas.
   - **Métodos principales**:
     - `handle(GetBookingByIdQuery query)`: Recupera una reserva específica por su ID.
     - `handle(GetAllBookingsQuery query)`: Recupera todas las reservas registradas en el sistema.
   - **Dependencias**:
     - `BookingRepository`: Persistencia de reservas.

2. **TableQueryServiceImpl**
   - **Propósito**: Gestiona las consultas relacionadas con las mesas y sus slots de disponibilidad.
   - **Métodos principales**:
     - `handle(GetTableByIdQuery query)`: Recupera una mesa específica por su ID.
     - `handle(GetAllTablesQuery query)`: Recupera todas las mesas registradas en el sistema.
     - `handle(GetTableScheduleByIdAndDateQuery query)`: Recupera los slots de disponibilidad de una mesa para una fecha específica.
   - **Dependencias**:
     - `TableRepository`: Persistencia de mesas y sus slots de disponibilidad.


#### **Event Handlers**

Los manejadores de eventos son responsables de reaccionar a eventos específicos del sistema. A continuación, se describe el principal manejador de eventos:

1. **SingleTableAvailabilitySlotsGeneratedEventHandler**
   - **Propósito**: Maneja el evento `SingleTableAvailabilitySlotsGeneratedEvent`, que se dispara cuando se generan los slots de disponibilidad para una mesa.
   - **Método principal**:
     - `on(SingleTableAvailabilitySlotsGeneratedEvent event)`: Genera los slots de disponibilidad para una mesa específica.
   - **Dependencias**:
     - `TableCommandService`: Servicio encargado de manejar los comandos relacionados con las mesas.

#### **Outbound Services (ACL)**

Los servicios externos proporcionan funcionalidades auxiliares que no forman parte del dominio principal. A continuación, se describen los principales servicios externos:

1. **ExternalHeadquarterService**
   - **Propósito**: Interactúa con el Branching Bounded Context para obtener información de las sedes.
   - **Métodos principales**:
     - `getHeadquarterOpeningTime(Long headquarterId)`: Obtiene la hora de apertura de una sede.
     - `getHeadquarterClosingTime(Long headquarterId)`: Obtiene la hora de cierre de una sede.
     - `getHeadquarterIntervalMinutes(Long headquarterId)`: Obtiene el intervalo de servicio en minutos de una sede.
     - `existsHeadquarter(Long headquarterId)`: Verifica si una sede existe.

2. **ExternalUserService**
   - **Propósito**: Interactúa con el IAM Bounded Context para verificar la existencia de usuarios.
   - **Método principal**:
     - `existUserById(Long userId)`: Verifica si un usuario existe en el sistema.

#### **Relaciones entre componentes**

- Los **Command Services** interactúan con los repositorios para modificar el estado del sistema y con los servicios externos (ACL) para validar información de otros contextos.
- Los **Query Services** interactúan únicamente con los repositorios para recuperar información del sistema.
- Los **Event Handlers** reaccionan a eventos del dominio para ejecutar lógica adicional, como la generación de slots de disponibilidad.
- Los **Outbound Services** (ACL) permiten la integración con otros contextos delimitados, como el Branching Bounded Context y el IAM Bounded Context.

La **Application Layer** del Booking Bounded Context asegura que las operaciones relacionadas con la gestión de reservas y mesas sean robustas, consistentes y fáciles de mantener. Al coordinar la lógica de negocio, manejar eventos y facilitar la integración con otros contextos, esta capa garantiza que las reglas del dominio se cumplan de manera eficiente y que el sistema sea escalable y extensible.

#### 4.2.4.4. Infrastructure Layer

La **Infrastructure Layer** del Booking Bounded Context proporciona las implementaciones técnicas necesarias para soportar las operaciones del sistema relacionadas con la gestión de reservas y mesas. Esta capa incluye repositorios para la persistencia de datos y componentes que conectan la lógica de negocio con los recursos externos, como bases de datos. Su objetivo principal es garantizar que las operaciones de almacenamiento y recuperación de información sean eficientes, consistentes y seguras.

#### **Persistencia (JPA Repositories)**

1. **BookingRepository**
   - **Propósito**: Proporciona métodos para interactuar con la base de datos de reservas.
   - **Características**:
     - Extiende `JpaRepository`, lo que permite realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre las entidades `Booking`.
     - Facilita la persistencia y recuperación de reservas, asegurando que las operaciones relacionadas con las reservas sean eficientes y confiables.

2. **TableRepository**
   - **Propósito**: Proporciona métodos para interactuar con la base de datos de mesas y sus slots de disponibilidad.
   - **Métodos principales**:
     - `existsByHeadquarterIdAndTableDetails_TableNumber(HeadquarterId headquarterId, Integer tableDetails_tableNumber)`: Verifica si existe una mesa con un número específico en una sede.
     - `findAvailabilitySlotsByTableIdAndDate(Long tableId, LocalDate date)`: Recupera los slots de disponibilidad de una mesa para una fecha específica.
     - `findByIdWithSlotsForUpdate(Long id)`: Recupera una mesa junto con sus slots de disponibilidad utilizando un bloqueo pesimista para evitar modificaciones concurrentes.
   - **Características**:
     - Extiende `JpaRepository`, lo que permite realizar operaciones CRUD sobre las entidades `Table`.
     - Incluye consultas personalizadas para manejar la relación entre mesas y sus slots de disponibilidad.
     - Utiliza un bloqueo pesimista (`PESSIMISTIC_WRITE`) para garantizar la consistencia de los datos durante las operaciones críticas, como la creación de reservas.

#### **Relaciones entre componentes**

- **Persistencia**: Los repositorios `BookingRepository` y `TableRepository` proporcionan acceso a los datos almacenados en la base de datos, permitiendo a las capas superiores (como la **Application Layer**) interactuar con las entidades del dominio.
- **Validación**: Los métodos personalizados en `TableRepository` son utilizados para validar la existencia de mesas y recuperar información específica, como los slots de disponibilidad, asegurando la consistencia de los datos durante las operaciones de negocio.

La **Infrastructure Layer** del Booking Bounded Context asegura que las operaciones relacionadas con la persistencia de datos sean robustas y confiables. Al proporcionar repositorios especializados para las reservas y mesas, esta capa facilita la integración con la base de datos y garantiza que las reglas de negocio, como la validación de slots de disponibilidad y la unicidad de mesas, se cumplan de manera eficiente. Esta estructura modular y reutilizable permite que el sistema sea escalable y fácil de mantener.

#### 4.2.4.5. Bounded Context Software Architecture Component Level Diagrams

En esta sección se presenta el diagrama de componentes del **Booking Bounded Context**, el cual detalla los principales módulos y sus interacciones dentro del contexto delimitado. Este diagrama sigue el enfoque del C4 Model para representar los componentes clave, como servicios de aplicación, controladores, repositorios y servicios externos, junto con sus relaciones.

El propósito de este diagrama es proporcionar una visión clara y estructurada de cómo se organizan los componentes dentro del contexto, facilitando la comprensión de su arquitectura y permitiendo identificar puntos de integración y responsabilidades.

El **Booking Bounded Context** está compuesto por los siguientes módulos principales:

1. **Application Layer**:
   - Coordina las operaciones de negocio relacionadas con la gestión de reservas y mesas.
   - Incluye servicios de comandos y consultas que interactúan con la **Domain Layer** y la **Infrastructure Layer**.
   - Maneja eventos relacionados con la creación de reservas y la generación de slots de disponibilidad.

2. **Interface Layer**:
   - Expone los puntos de entrada al sistema a través de controladores REST.
   - Incluye recursos y transformadores que aseguran una representación adecuada de los datos y su conversión entre las capas de la aplicación.

3. **Domain Layer**:
   - Encapsula la lógica de negocio relacionada con la gestión de reservas y mesas.
   - Define los agregados, entidades y objetos de valor que representan los conceptos clave del dominio.

4. **Infrastructure Layer**:
   - Proporciona las implementaciones técnicas necesarias para soportar las operaciones del sistema.
   - Incluye repositorios para la persistencia de datos y componentes que conectan la lógica de negocio con los recursos externos, como bases de datos.

<img src="./images/c4-model/bc-component-diagram/IOT-Booking-BC-Component-Diagram.svg" alt="Booking BC Component Diagram"/><br>

#### 4.2.4.6. Bounded Context Software Architecture Code Level Diagrams

En este apartado se presentan los diagramas que ofrecen un mayor nivel de detalle sobre la implementación de los componentes del **Booking Bounded Context**. Estos diagramas están diseñados para ilustrar cómo se estructuran las clases, interfaces y relaciones dentro de las capas del contexto, proporcionando una visión técnica que facilita el desarrollo, mantenimiento y evolución del sistema.

##### 4.2.4.6.1. Bounded Context Domain Layer Class Diagrams

El diagrama de clases correspondiente a la **Domain Layer** del **Booking Bounded Context** incluye las clases principales, como agregados, entidades y objetos de valor, así como las interfaces y enumeraciones que definen el comportamiento del dominio. También se destacan las relaciones entre estos elementos, como asociaciones, composiciones y dependencias.

**Elementos principales del diagrama:**

1. **Aggregates**:
   - `Booking`: Agregado principal que encapsula la lógica de negocio relacionada con las reservas. Incluye atributos como `userId`, `tableId`, `bookingDate` y `bookingSlots`.
   - `Table`: Agregado que representa una mesa en una sede específica, incluyendo su disponibilidad y detalles.

2. **Entities**:
   - `AvailabilitySlot`: Representa un intervalo de tiempo disponible para una mesa en una fecha específica.
   - `BookingSlot`: Representa un intervalo de tiempo reservado por un cliente.

3. **Value Objects**:
   - `UserId`: Representa el identificador único de un cliente.
   - `HeadquarterId`: Representa el identificador único de una sede.
   - `TableDetails`: Representa los detalles de una mesa, como su número y cantidad de asientos.
   - `TimeSlot`: Representa un intervalo de tiempo con una hora de inicio y una hora de fin.
   - `TableStatus`: Enumera los estados posibles de una mesa (`AVAILABLE`, `RESERVED`, `OCCUPIED`).
   - `ScheduleSlotStatus`: Enumera los estados posibles de un slot de disponibilidad (`AVAILABLE`, `RESERVED`).

**Relaciones destacadas:**
- El agregado `Booking` gestiona las relaciones con las entidades `BookingSlot` y `Table`.
- El agregado `Table` gestiona la generación y actualización de los slots de disponibilidad (`AvailabilitySlot`).
- Los objetos de valor encapsulan datos inmutables y validaciones específicas, asegurando consistencia en el dominio.

<img src="./images/c4-model/class-diagram/booking_domain_class_diagram.webp" alt="Booking BC Domain Layer Class Diagram"/><br>


##### 4.2.4.6.2. Bounded Context Database Design Diagram.


