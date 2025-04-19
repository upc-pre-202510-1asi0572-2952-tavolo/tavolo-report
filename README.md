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
- Jimena Cama     (aksonie)
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
            - He demostrado la capacidad de trabajar eficazmente en equipos multidisciplinarios, asumiendo roles de liderazgo compartido para la toma de decisiones y el logro de objetivos comunes. En el desarrollo de proyectos, fomenté un entorno inclusivo donde cada integrante pudo aportar sus fortalezas, promoviendo la comunicación abierta, la planificación conjunta de tareas y la adaptación ante cambios.
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
            - He demostrado la capacidad de crear un entorno de trabajo colaborativo e inclusivo, en el que se valora la participación activa de todos los integrantes del equipo. A lo largo del desarrollo del proyecto, trabajé en la definición de metas comunes, la planificación de tareas con enfoque estratégico y el cumplimiento de los objetivos establecidos, asegurando una gestión eficiente del tiempo y los recursos.
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

**TAVOLO** es una solución tecnológica desarrollada para **optimizar la experiencia en cafeterías peruanas** mediante el uso de **dispositivos IoT** integrados a un sistema web y móvil. Su propuesta se enfoca exclusivamente en resolver los problemas relacionados con la ocupación de mesas, la gestión de reservas y la visualización de información relevante para los comensales, administradores y usuarios superadministradores.

Para los comensales, TAVOLO permite visualizar el menú digital de una sede, conocer la disponibilidad de mesas en tiempo real, realizar reservas y consultar detalles de las mismas. También se ofrece la posibilidad de visualizar la ubicación de todas las sedes en un mapa interactivo, registrarse como nuevo usuario o iniciar sesión para acceder a funcionalidades personalizadas. Estas características permiten al usuario planificar su visita con antelación y evitar tiempos de espera innecesarios. Un estudio reciente de Apoyo Consultoría (2023) reveló que el 62 % de los limeños evita acudir a locales con alta concurrencia si no puede consultar previamente la disponibilidad, lo cual respalda la utilidad de este enfoque preventivo basado en datos en tiempo real.

Desde el panel de administración, los administradores pueden gestionar la sede que se les ha asignado. Esto incluye agregar nuevas mesas, eliminar aquellas que ya no estén en uso, visualizar todas las reservas registradas en su local y confirmar que están gestionando la sede correcta. Esta funcionalidad permite a los encargados mantener un control actualizado del aforo, planificar la atención de manera eficiente y optimizar la logística operativa. La digitalización de estas tareas manuales no solo mejora la precisión en la gestión, sino que también incrementa la productividad del personal administrativo.

TAVOLO se presenta así como una respuesta concreta y realista a los desafíos cotidianos que enfrentan las cafeterías en Perú. No pretende cubrir todo el ciclo de negocio de un restaurante, sino **centrarse exclusivamente en la mejora del proceso de aforo, reservas y atención al cliente**. Este enfoque especializado y realista busca generar impacto directo en la experiencia del usuario y en la eficiencia del negocio, con una implementación que puede ser gradual, asequible y con bajo nivel de complejidad técnica.

**Mision:**<br>
Brindar una solución tecnológica eficiente y accesible para la gestión de aforo en cafeterías peruanas, utilizando dispositivos IoT y plataformas digitales que permitan a los comensales acceder a información en tiempo real, y a los administradores optimizar la ocupación de mesas y las reservas, **mejorando así la experiencia del cliente y la operación del negocio.**

**Visión:**<br>
Consolidarse como la **solución de referencia en el Perú** para la digitalización de procesos de atención en cafeterías, mediante el uso de tecnología embebida, edge computing y sistemas en la nube, promoviendo una experiencia de consumo más ordenada, rápida y satisfactoria para los comensales, y una gestión más eficiente para los negocios del sector gastronómico.

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

**TAVOLO es una solución tecnológica integral basada en IoT** que transforma la forma en que los comensales interactúan con las cafeterías. El sistema utiliza sensores de peso (con un margen de error inferior al 5 %) para detectar en tiempo real la ocupación de las mesas. Esta información se transmite automáticamente a una aplicación web y móvil dirigida a los comensales, permitiéndoles consultar la disponibilidad de mesas desde sus dispositivos personales antes de llegar al establecimiento.

El objetivo principal es minimizar los tiempos de espera, asegurando que el **usuario final no espere más de 2 minutos para acceder a una mesa libre**. Para ello, el sistema realiza **actualizaciones cada 10 segundos** y cuenta con una interfaz optimizada con tiempos de carga inferiores a 5 segundos. De este modo, se mejora significativamente la experiencia del cliente, brindándole información clara, precisa y en tiempo real que le facilite tomar decisiones sobre su visita.

Actualmente, la implementación del sistema, tanto a nivel físico como tecnológico, está a cargo del equipo de desarrollo, quienes conocen a fondo su funcionamiento. Sin embargo, contemplamos una fase de escalamiento en la que el personal de cada cafetería podrá instalar el sistema en menos de una hora, sin necesidad de asistencia técnica especializada.

Además, TAVOLO incluye una interfaz administrativa exclusiva para cada sede, donde los administradores pueden agregar mesas, consultar la sede asignada, visualizar reservas y, próximamente estadísticas. Esta funcionalidad permitirá optimizar la rotación de mesas y mejorar la gestión del flujo de comensales.

### 1.2.1. Antecedentes y problemática  

En los últimos años, el sector gastronómico en el Perú ha mostrado un crecimiento sostenido, especialmente en ciudades como Lima, Arequipa y Cusco, donde las cafeterías han ganado popularidad como espacios de encuentro social y laboral. Según el Ministerio de la Producción (2022), **los negocios relacionados con alimentos y bebidas representaron más del 35 % del total de microempresas en el sector servicios**. Sin embargo, la mayoría de estos establecimientos aún carece de tecnologías que les permitan gestionar de forma eficiente su aforo y rotación de clientes, especialmente en horas pico. Pese al avance de la digitalización en otros rubros, la implementación de tecnologías inteligentes, como sensores IoT o aplicaciones móviles personalizadas, aún es limitada en el sector gastronómico peruano (INEI, 2021).

Actualmente, uno de los principales desafíos para los clientes de cafeterías en el Perú es la incertidumbre sobre la disponibilidad de mesas, lo que genera pérdidas de tiempo, experiencias insatisfactorias y, en algunos casos, la decisión de no ingresar al local. Esta problemática se intensifica en zonas urbanas con alta demanda, donde la falta de sistemas de gestión en tiempo real impide una distribución óptima del aforo. Según un estudio de Apoyo Consultoría (2023), **más del 60 % de los consumidores en Lima indicaron que evitarían acudir a locales concurridos si tuvieran una alternativa digital que les informe sobre la disponibilidad antes de salir de casa.** Esta situación representa no solo una oportunidad de mejora para la experiencia del cliente, sino también una necesidad de transformación digital en la industria.

Aplicando la técnica de las 5 W y 2 H:

**What? - ¿Qué?** <br>
TAVOLO es una solución tecnológica integrada con IoT que permite **monitorear en tiempo real la ocupación de mesas en cafeterías**, proporcionando a los clientes información precisa sobre la disponibilidad antes de llegar al establecimiento. Además, ofrece a los administradores la posibilidad de **gestionar las mesas** y **reservas de comensales** mediante una interfaz intuitiva.

**Why? - ¿Por qué?**<br>
El problema se vuelve crítico en momentos de alta afluencia, como durante almuerzos, cenas, fines de semana o eventos especiales, en los cuales la ocupación irregular de las mesas puede generar aglomeraciones y una mala experiencia para los clientes.

**Where? - ¿Dónde?**<br>
El sistema está destinado a **cafeterías ubicadas en áreas urbanas** de alta demanda, comenzando con Lima, y se proyecta expandir a otras ciudades del Perú y eventualmente a Latinoamérica. La interfaz web y móvil estará disponible para clientes en cualquier lugar, mientras que la instalación física de los sensores de ocupación será realizada dentro de las cafeterías.

**When? - ¿Cuando?** <br>
La implementación inicial del sistema se desarrollará en un corto plazo, con un escalamiento proyectado a futuro para permitir la instalación por parte del personal de las cafeterías sin soporte técnico especializado.

**Who? - ¿Quién?** <br>
El sistema está dirigido a comensales y administradores de cafeterías. Los comensales utilizan la aplicación para verificar la disponibilidad de mesas y realizar reservas. Los administradores gestionan las mesas y reservas.

**How? - ¿Cómo?** <br>
La solución se implementará instalando sensores de peso en cada mesa, conectados a una red IoT que transmite datos en tiempo real a una plataforma centralizada. A través de una aplicación móvil y web, los usuarios podrán visualizar la disponibilidad de mesas y, a su vez, el personal del establecimiento podrá gestionar la ocupación de manera óptima y recibir alertas en caso de anomalías.

**How much? - ¿Cuánto?** <br>
_¿Cuánto afecta este problema?_ <br>
La falta de control de aforo puede traducirse en pérdidas económicas para los establecimientos debido a la ineficiencia en la asignación de mesas, así como en sanciones por incumplimiento de normativas de seguridad.

_¿Cuánto costará resolver este problema?_ <br>
El costo de implementación dependerá del número de mesas y la infraestructura necesaria para la conexión y mantenimiento de los sensores, así como del desarrollo de la plataforma digital. Se estima que la inversión inicial se recuperará rápidamente mediante la optimización del uso del espacio y el incremento en la satisfacción del cliente.

_¿Cuántas personas se beneficiarán?_ <br>
Esta solución beneficiará directamente a los clientes y al personal de los establecimientos, con un impacto indirecto en el sector gatronómico en general. Se estima que, en establecimientos de tamaño mediano, la adopción de la tecnología podría mejorar la eficiencia operativa en un 30-40%, beneficiando a cientos de usuarios diarios.

La problemática identificada no requiere una transformación completa del modelo de negocio de las cafeterías, sino una **intervención técnica puntual** que resuelva los cuellos de botella más frecuentes: **el acceso a información de disponibilidad, la planificación anticipada y la gestión eficiente del espacio físico**. En ese sentido, **TAVOLO no busca reemplazar los procesos tradicionales**, sino complementarlos con herramientas tecnológicas que permitan a las cafeterías peruanas operar con mayor previsibilidad, rapidez y satisfacción del cliente.



### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements 

### Visitante
**Para** los visitantes que desean informarse sobre soluciones tecnológicas aplicadas a cafeterías,  
**que necesitan** comprender qué es TAVOLO, cómo funciona y qué valor ofrece,  
**pero** actualmente no encuentran en el ecosistema digital peruano una presentación clara ni accesible que comunique efectivamente los beneficios de una solución basada en IoT para el sector gastronómico.  
**Esto les impide** considerar su adopción, recomendarla o confiar en su utilidad real.

El 35 % de las microempresas peruanas del sector servicios corresponde a negocios de alimentos y bebidas, pero más del 70 % de estas aún no cuenta con estrategias digitales de comunicación técnica o funcional.  
**TAVOLO busca resolver** este vacío mediante una landing page visual, estructurada y orientada a comunicar desde el **primer contacto su propuesta de valor**, casos de uso y beneficios diferenciadores.

### Comensal
**Para** comensales que frecuentan cafeterías en zonas urbanas del Perú,  
**que necesitan** conocer en tiempo real la disponibilidad de mesas, visualizar el menú digital y reservar con antelación,  
**pero** actualmente enfrentan esperas innecesarias, incertidumbre al llegar al local y una experiencia de consumo poco predecible,  
**lo que afecta** su comodidad y decisión de volver a consumir en el mismo establecimiento.

Según un estudio de Apoyo Consultoría (2023), **el 62 % de los consumidores limeños evitaría ingresar a un local si no puede verificar previamente su nivel de aforo**.  
TAVOLO responde a esta necesidad con una plataforma sincronizada con sensores embebidos, que ofrece al comensal una app móvil para autogestión de su visita y planificación de su consumo con mínima fricción.


### Administrador
**Para** los administradores de cafeterías encargados de operar las sedes en tiempo real,  
**que necesitan** gestionar la ocupación de mesas, controlar reservas y visualizar su sede asignada mediante una interfaz digital centralizada,  
**pero** actualmente dependen de métodos manuales y no cuentan con herramientas que integren sensores físicos con flujos operativos,  
**lo que genera** errores en la asignación, sobreaforo no controlado y decisiones reactivas.

En cafeterías de tamaño mediano en Lima, la falta de automatización genera pérdidas operativas y afecta la experiencia del cliente. Según datos internos y análisis del sector, **la eficiencia puede incrementarse en un 30–40 % con tecnologías de digitalización inteligente**.  
TAVOLO busca transformar este escenario mediante un panel de administración en la nube, que unifica la gestión de sedes, mesas y reservas en una interfaz intuitiva con datos en tiempo real.

#### 1.2.2.2. Lean UX Assumptions
A partir del análisis del contexto y las necesidades identificadas en los distintos perfiles de usuario, se establecen los siguientes supuestos iniciales que guían el diseño y validación del producto TAVOLO. Estos supuestos serán **contrastados durante el desarrollo iterativo** del proyecto para asegurar que el producto responda realmente a los objetivos planteados.

###### **Business Outcomes:**
- Aumento del 25% en la eficiencia operativa de los establecimientos que adopten la solución.
- Reducción del 30% en incidencias por sobreaforo y problemas de asignación de mesas.
- Incremento del 20% en la satisfacción de los clientes, medido a través de encuestas de experiencia.
- Incremento del 15% en el flujo de clientes al evitar tiempos de espera prolongados.
- Mejora en el cumplimiento de protocolos de seguridad y normativas vigentes.

###### **Users:**
Los usuarios primarios son:
- Propietarios y administradores cafeterías: Interesados en optimizar el uso del espacio y garantizar la seguridad en el establecimiento. <br>
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
- Visualización en tiempo real del estado de ocupación de las mesas.
- Funcionalidad de reservas digitales.
- Menú accesible por sede desde la aplicación.
- Gestión de mesas y reservas para administradores.
- Acceso completo a la plataforma para superadministradores.
- Seguridad basada en autenticación por roles.

###### **Business Assumptions:**
1.  **Creemos que nuestros usuarios necesitan** un sistema automatizado y en tiempo real que facilite la gestión del aforo en establecimientos de hostelería.

2. **Estas necesidades se pueden satisfacer** mediante la implementación de sensores IoT y el desarrollo de una plataforma digital accesible desde dispositivos móviles y computadoras.

3. **Nuestros clientes serán** cafeterías que buscan mejorar la eficiencia en la gestión de sus espacios y la experiencia de sus clientes.

4. **El valor más importante que un cliente quiere de nuestros servicios es** la capacidad de optimizar la ocupación de mesas en tiempo real, garantizando tanto la seguridad como la eficiencia operativa.

5. **El cliente también va obtener** beneficios adicionales como la recopilación de datos para análisis futuros.

6. **Vamos a obtener la mayoría de nuestros clientes mediante** estrategias de marketing digital, participación en ferias de tecnología y colaboraciones con asociaciones del sector de gastronomía.

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
La solución se integra en la operación diaria de las cafeterías, facilitando tanto la gestión interna (para administradores) como la experiencia del cliente al planificar su visita.<br>

**¿Cuándo y cómo es nuestro producto? ¿Usado?** <br>
El producto es utilizado en tiempo real, especialmente durante horas pico y en momentos de alta afluencia, permitiendo a los establecimientos gestionar el aforo de forma continua y los clientes verificar la disponibilidad antes de llegar. <br>

**¿Cómo debe verse nuestro productoo y cómo debe comportarse?** <br>
La interfaz visual debe ser moderna, limpia e intuitiva, con gráficos y datos en tiempo real que faciliten la rápida comprensión del estado de ocupación. Además, el sistema debe ser ágil, confiable y accesible desde múltiples dispositivos, garantizando una experiencia fluida y sin complicaciones. <br>

#### 1.2.2.3. Lean UX Hypothesis Statements  

A continuación, se detallan las hipótesis formuladas para abordar la problemática mediante las funcionalidades incluidas en nuestra propuesta de solución IoT. Cada hipótesis está diseñada para ser clara, cuantificable y permitir una evaluación objetiva de su éxito.

- **Hypothesis Statement 1:** <br>
    **Creemos que** los propietarios y administradores de cafeterías necesitan una herramienta en tiempo real que les permita monitorear la ocupación de mesas de forma automatizada. 
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

- **Propietarios de Cafeterías:** <br>
 Este segmento es clave, ya que busca herramientas que faciliten la gestión en tiempo real de la ocupación de mesas, reduzcan errores manuales y optimicen la operación del negocio. Son usuarios que valoran la eficiencia operativa y la posibilidad de obtener estadísticas precisas para la toma de decisiones. 
 <br>

- **Clientes del Establecimientos** <br>
Los clientes se benefician al contar con información actualizada sobre la disponibilidad de mesas, lo que les permite planificar su visita de manera eficiente, evitar largos tiempos de espera y disfrutar de una experiencia más cómoda y agradable.






