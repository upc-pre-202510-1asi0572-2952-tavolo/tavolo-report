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
TAVOLO está diseñado para atender las necesidades reales de usuarios que interactúan directamente con el sistema dentro del entorno de atención y operación en cafeterías. A partir del análisis funcional y del levantamiento de requisitos, se identifican dos segmentos objetivos clave, sobre los cuales se construye y valida el producto.
**1. Comensales recurrentes en zonas urbanas de alta afluencia**
Este segmento está compuesto por usuarios finales que visitan frecuentemente cafeterías ubicadas en distritos con alto tránsito peatonal, como San Isidro, Miraflores, Surco y San Miguel. Se trata principalmente de estudiantes universitarios, trabajadores de oficina y profesionales jóvenes que priorizan la optimización de su tiempo durante el desayuno, el almuerzo o reuniones breves. Son usuarios digitales familiarizados con el uso de aplicaciones móviles y esperan poder visualizar la disponibilidad de mesas, hacer reservas y consultar el menú digital desde sus dispositivos personales. Este segmento es fundamental para validar la propuesta de valor del producto y su utilidad en entornos reales de consumo.
**2. Administradores operativos de cafeterías**
Este grupo corresponde a los encargados de gestionar el funcionamiento de una sede física. Tienen bajo su responsabilidad el control del aforo, la gestión de mesas y la administración de reservas. También requieren saber qué sede tienen asignada y mantener el sistema actualizado según los cambios del local. Este segmento valida la funcionalidad del panel de gestión administrativa, que incluye herramientas visuales, control de datos en tiempo real y facilidad de uso en entornos dinámicos como una cafetería con alta rotación.

Cabe precisar que, si bien el sistema contempla un **rol de superadministrador** con acceso total a las funcionalidades, este **no representa un segmento objetivo del producto**, sino que corresponde exclusivamente al equipo de desarrollo encargado de configurar el sistema, realizar pruebas y brindar soporte técnico al propietario del negocio.


# Capítulo II: Requirements Elicitation & Analysis
## 2.1. Competidores
Algunos de los competidores a los que Tavolo podría enfrentarse son:
<ul>
    <li>
        <b>Eat App: </b>Plataforma de gestión de reservas y mesas que permite a los restaurantes automatizar la asignación de mesas, mejorar la experiencia del cliente y analizar datos de comportamiento. Eat App se destaca por su CRM integrado y herramientas de marketing, aunque su sistema depende de reservas manuales y no detecta la ocupación en tiempo real.
    </li>
    <li>
        <b>OpenTable: </b>Uno de los líderes globales en reservas en línea para restaurantes. Ofrece una experiencia fluida para los usuarios al permitir reservas anticipadas y gestionar la disponibilidad de mesas. Sin embargo, su enfoque está más orientado a restaurantes formales y no cuenta con integración de sensores ni monitoreo automático de mesas.
    </li>
    <li>
        <b>Waitlist Me: </b>Aplicación que digitaliza la lista de espera tradicional, permitiendo a los clientes apuntarse desde sus teléfonos y recibir notificaciones cuando su mesa esté lista. Aunque mejora la organización y reduce aglomeraciones, depende de la actualización manual por parte del personal y no ofrece información en tiempo real sobre la ocupación real del local.
    </li>
</ul>

### 2.1.1. Análisis competitivo

<table><tr><th colspan="16" valign="top"><b>Competitive Analysis Landscape</b></th></tr>
<tr><td colspan="9" valign="top">¿Por qué llevar a cabo este análisis?  </td><td colspan="7" valign="top">Este análisis se lleva a cabo para poder investigar, analizar y comparar el comportamiento de los competidores directos o indirectos en el mercado.</td></tr>
<tr><td colspan="6" valign="top"><p><b>Nombre</b></p><p></p></td><td colspan="3" valign="top"><b>Tavolo</b></td><td colspan="3" valign="top"><b>Eat App</b></td><td colspan="3" valign="top"><b>OpenTable</b></td><td valign="top"><b>Waitlist Me</b></td></tr>
<tr><td colspan="6" valign="top"><b>Logo</b> </td><td colspan="3" valign="top"><img src="./images/analisis_competitivo/tavolo.jpg"></td><td colspan="3" valign="top"><img src="./images/analisis_competitivo/EatApp.png"></td><td colspan="3" valign="top"><img src="./images/analisis_competitivo/OpenTable.png"><td valign="top"><img src="./images/analisis_competitivo/WaitlistMe.png"></tr>
<tr><td colspan="3" rowspan="4" valign="top"><b>Perfil</b></td><td colspan="3" rowspan="2" valign="top"><b>Overview</b></td><td colspan="3" rowspan="2" valign="top">Es una solución tecnológica integral basada en IoT, diseñada específicamente para cafeterías. Utiliza sensores de peso para detectar automáticamente la ocupación de mesas y actualiza esta información cada 10 segundos en una app web y móvil. El sistema también ofrece una interfaz administrativa para la sede, facilitando la gestión del flujo de comensales y mejorando la rotación de mesas.</td><td colspan="3" rowspan="2" valign="top">Es una plataforma de gestión de restaurantes basada en la nube que permite manejar reservas, asignación de mesas, datos de clientes y campañas de marketing automatizadas. Su enfoque está en ofrecer una experiencia completa para restaurantes que desean profesionalizar la relación con sus clientes, utilizando herramientas de CRM, reportes y análisis de comportamiento.</td><td colspan="3" rowspan="2" valign="top">Es una de las plataformas más reconocidas a nivel mundial para reservas en restaurantes. Los usuarios pueden buscar establecimientos, ver disponibilidad en tiempo real, leer reseñas y reservar directamente desde la app o el sitio web. También ofrece herramientas para los restaurantes, aunque su enfoque principal está en mejorar la experiencia del comensal antes de llegar al lugar.</td><td rowspan="2" valign="top">Es una solución que digitaliza el proceso de espera en locales físicos, como restaurantes, cafeterías y tiendas. Los clientes pueden apuntarse a una lista desde sus dispositivos y reciben notificaciones cuando su turno se acerca. También permite al staff gestionar el flujo de clientes de forma más organizada, aunque depende de la intervención manual.</td></tr>
<tr></tr>
<tr><td colspan="3" rowspan="2" valign="top"><b>Ventaja competitiva ¿Qué valor ofrece a los clientes?</b></td><td colspan="3" rowspan="2" valign="top">Brinda información precisa y en tiempo real sobre la disponibilidad de mesas, ayudando a evitar esperas y optimizando su visita desde antes de llegar al local.</td><td colspan="3" rowspan="2" valign="top">Permite reservar mesas de forma sencilla y recibir un servicio más personalizado, gracias al uso de datos históricos y preferencias del cliente.</td><td colspan="3" rowspan="2" valign="top">Facilita la reserva anticipada en restaurantes de forma rápida y confiable, brindando acceso a una amplia variedad de opciones en una sola plataforma.</td><td rowspan="2" valign="top">Reduce la incertidumbre y el tiempo de espera físico, al permitirles ocupar su tiempo libremente mientras esperan su turno.</td></tr>
<tr></tr>
<tr><td colspan="3" rowspan="2" valign="top"><b>Perfil de Marketing</b></td><td colspan="3" valign="top"><b>Mercado objetivo</b></td><td colspan="3" valign="top">Cafeterías que buscan innovar en la gestión de mesas y mejorar la experiencia del cliente mediante tecnología avanzada.</td><td colspan="3" valign="top">Restaurantes que buscan mejorar su gestión de reservas y la experiencia del cliente. Su mercado abarca desde pequeños establecimientos hasta grandes cadenas hoteleras y restaurantes de alta gama.</td><td colspan="3" valign="top">Gama de restaurantes, desde pequeños locales hasta grandes cadenas internacionales, que buscan gestionar reservas en línea y mejorar la experiencia del cliente.</td><td valign="top">Restaurantes, cafeterías y otros establecimientos de servicio rápido que buscan gestionar eficientemente las listas de espera y mejorar la experiencia del cliente.</td></tr>
<tr><td colspan="3" valign="top"><b>Estrategias de Marketing</b></td><td colspan="3" valign="top"><p>Demostraciones en vivo.</p><p>Alianzas estratégicas.</p><p>Publicidad en redes sociales.</p><p>Marketing de contenidos.</p></td><td colspan="3" valign="top"><p>Optimización de motores de búsqueda.</p><p>Publicidad de pago por clic.</p><p>Alianzas estratégicas.</p></td><td colspan="3" valign="top"><p>Publicidad y promoción.</p><p>Análisis de datos.</p><p>Segmentación de clientes.</p></td><td valign="top"><p>Pruebas gratuitas y demostraciones.</p><p>Testimonios y reseñas.</p><p></p></td></tr>
<tr><td colspan="3" rowspan="3" valign="top"><b>Perfil de producto</b></td><td colspan="3" valign="top"><b>Productos y Servicios</b></td><td colspan="3" valign="top">Solución basada en IoT que utiliza sensores de peso para detectar la ocupación de las mesas en tiempo real. Esta información se refleja automáticamente en una app web y móvil, permitiendo a los comensales ver la disponibilidad de mesas antes de llegar. Además, incluye una interfaz administrativa para la gestión del flujo de comensales y optimización de la rotación de mesas.</td><td colspan="3" valign="top">Proporciona un sistema de reservas en línea, un CRM para gestionar relaciones con los clientes, herramientas de marketing automatizado, análisis de datos y reportes detallados, así como la integración con otros sistemas de restaurante como POS (punto de venta) y plataformas de pago.</td><td colspan="3" valign="top">Ofrece a los restaurantes herramientas para gestionar la disponibilidad de mesas, realizar reservas, y personalizar la experiencia del cliente. También proporciona servicios de marketing y publicidad, herramientas de CRM y análisis detallados del rendimiento del restaurante, como la ocupación y los tiempos de espera.</td><td valign="top">Ofrece una solución digital para gestionar las listas de espera en tiempo real. Los restaurantes pueden asignar mesas y notificar a los clientes mediante SMS o la app cuando su mesa esté lista. Además, la plataforma ofrece análisis sobre los tiempos de espera y la rotación de mesas para mejorar la eficiencia del establecimiento.</td></tr>
<tr><td colspan="3" valign="top"><b>Precios y Costos</b></td><td colspan="3" valign="top">Ofrece un modelo de suscripción mensual, con precios que varían según el número de mesas y funcionalidades requeridas. A diferencia de sus competidores, no cobra comisiones por cada reserva, lo que lo convierte en una opción más rentable a largo plazo. Puede haber un costo inicial por la instalación de los sensores.</td><td colspan="3" valign="top">Sigue un modelo de suscripción mensual, con precios que empiezan desde $99 por mes dependiendo del tamaño del restaurante y las funcionalidades necesarias. Además, en algunos casos, cobran comisiones por cada reserva realizada a través de la plataforma.</td><td colspan="3" valign="top">Opera con un modelo basado en suscripción mensual, cuyo precio inicial ronda los $39 por mes. Además, cobra una comisión por cada reserva realizada a través de la plataforma, que varía entre el 1% y el 5%. También puede haber costos adicionales por servicios de promoción o características premium.</td><td valign="top">Opera con un modelo de suscripción mensual, comenzando desde $29 al mes para restaurantes pequeños. No cobra comisiones por reserva, lo que lo hace una opción más accesible en términos de costos continuos. Los precios varían según el tamaño del restaurante y las funcionalidades adicionales requeridas.</td></tr>
<tr><td colspan="3" valign="top"><b>Canales de distribución</b></td><td colspan="3" valign="top"><p>- Página web</p><p>- Aplicaciones móviles en dispositivos iOS y Android.</p><p></p></td><td colspan="3" valign="top"><p>- Página web</p><p>- Aplicaciones móviles en dispositivos iOS y Android.</p></td><td colspan="3" valign="top"><p>- Página web</p><p>- Aplicaciones móviles en dispositivos iOS y Android.</p></td><td valign="top"><p>- Página web</p><p>- Aplicaciones móviles en dispositivos iOS y Android.</p></td></tr>
<tr><td colspan="3" rowspan="4" valign="top"><b>Análisis FODA</b></td><td colspan="3" valign="top"><b>Fortalezas</b></td><td colspan="3" valign="top"><p>- Detección automática de ocupación en tiempo real.</p><p>- App ligera, actualizaciones rápidas (cada 10 segundos).</p><p>- Instalación simple sin técnicos.</p></td><td colspan="3" valign="top"><p>- Plataforma integral con CRM y analítica.</p><p>- Buena integración con otros sistemas.</p><p>- Funciona en móviles y tablets.</p></td><td colspan="3" valign="top"><p>- Marca reconocida globalmente.</p><p>- Gran base de usuarios y restaurantes.</p><p>- Interfaz amigable para el cliente.</p></td><td valign="top"><p>- Fácil de usar y configurar.</p><p>- Económico y accesible.</p><p>- Sin comisiones por cliente.</p></td></tr>
<tr><td colspan="3" valign="top"><b>Debilidades</b></td><td colspan="3" valign="top"><p>- Requiere hardware (sensores).</p><p>- Etapa temprana de adopción y posicionamiento.</p></td><td colspan="3" valign="top"><p>- No detecta ocupación en tiempo real.</p><p>- Costos altos para pequeños restaurantes.</p></td><td colspan="3" valign="top"><p>- Comisiones por reserva.</p><p>- Menor personalización para negocios pequeños.</p></td><td valign="top"><p>- Dependencia del ingreso manual del personal.</p><p>- Sin monitoreo físico de mesas.</p></td></tr>
<tr><td colspan="3" valign="top"><b>Oportunidades</b></td><td colspan="3" valign="top"><p>- Escalamiento a grandes cadenas de cafeterías.</p><p>- Expansión hacia restaurantes u hoteles.</p></td><td colspan="3" valign="top"><p>- Expansión en mercados emergentes.</p><p>- Alianzas con grandes cadenas.</p></td><td colspan="3" valign="top"><p>- Ampliar servicios para cafeterías o locales pequeños.</p><p>- Integración con experiencias gastronómicas.</p></td><td valign="top"><p>- Penetrar en mercados de comida rápida y cafeterías.</p><p>- Mejora con inteligencia artificial.</p></td></tr>
<tr><td colspan="3" valign="top"><b>Amenazas</b></td><td colspan="3" valign="top"><p>- Copia del modelo por grandes competidores.</p><p>- Desconfianza inicial por ser una tecnología emergente.</p></td><td colspan="3" valign="top"><p>- Competencia con soluciones más automatizadas.</p><p>- Cambios en las tecnologías de reservas.</p></td><td colspan="3" valign="top"><p>- Nuevas plataformas sin comisiones.</p><p>- Desintermediación (restaurantes que prefieren sistemas propios).</p></td><td valign="top"><p>- Soluciones con detección automática.</p><p>- Apps integrales que lo superen en funcionalidades.</p></td></tr>
</table>

### 2.1.2. Estrategias y tácticas frente a competidores

Hemos empleado un análisis FODA para identificar las posibilidades y desafíos en el mercado, así como para evaluar nuestras fortalezas y debilidades internas. Esta metodología nos ha permitido concebir estrategias y tácticas que se ajusten de manera coherente a nuestro entorno y a los recursos disponibles.

**Estrategia de diferenciación tecnológica:**

La principal estrategia de Tavolo es posicionarse como una solución única en el mercado al incorporar tecnología IoT para detectar en tiempo real la ocupación de mesas, eliminando por completo la necesidad de intervención humana o registro manual. Esto permite ofrecer al cliente final información confiable y constante, algo que sus competidores no alcanzan con precisión.

**Estrategia de enfoque de nicho en cafeterías:**

Otra estrategia clave es enfocarse en un nicho específico y muy definido: las cafeterías. A diferencia de otras plataformas que buscan abarcar todo tipo de restaurantes, Tavolo se especializa en un entorno donde la rotación rápida, la autogestión y la simplicidad son fundamentales. En línea con esto, la táctica es desarrollar un lenguaje de marca, interfaz y funcionalidades adaptadas a este tipo de negocio, además de lanzar campañas dirigidas a franquicias de cafeterías o locales independientes que no requieren una infraestructura compleja, pero sí soluciones eficientes.

**Estrategia de escalabilidad y fácil instalación:**

Pensando en el crecimiento, Tavolo adopta una estrategia de escalabilidad técnica, diseñando un sistema que puede instalarse sin necesidad de personal técnico, en menos de una hora, lo que facilita su expansión sin altos costos logísticos. Como táctica, se crean tutoriales paso a paso, videos cortos y documentación visual clara que permiten a cualquier miembro del personal ejecutar la instalación.

**Estrategia de posicionamiento de marca y educación del mercado:**

Tavolo impulsa una estrategia de posicionamiento de marca basada en innovación y liderazgo de pensamiento en el sector horeca. La táctica principal para esto es la generación de contenido educativo (blogs, infografías, webinars) que informan sobre la importancia del monitoreo en tiempo real, las pérdidas por esperas largas y cómo la tecnología puede resolverlo, posicionando a Tavolo como referente en soluciones inteligentes para la industria.

## 2.2. Entrevistas
### 2.2.1. Diseño de entrevistas

### Propietarios de cafeterías

**Preguntas de presentación:**

1. ¿Podrías indicarnos tu nombre y el de tu cafetería?
2. ¿Qué puesto ocupas dentro de la empresa?
3. ¿Desde cuándo está funcionando tu cafetería?

**Propósito:** Queremos entender tus necesidades y retos para mejorar la gestión del aforo en tu cafetería.

**Entrevista:**

1. ¿Cómo gestionas actualmente las reservas y la disponibilidad de mesas?
2. ¿Qué problemas enfrentas con el tiempo de espera de los clientes?
3. ¿Estarías interesado en una solución tecnológica para gestionar las mesas en tiempo real?
4. ¿Qué características consideras más importantes en una plataforma de gestión de aforo?
5. ¿Qué tan importante es para ti la facilidad de instalación y el soporte técnico?
6. ¿Cómo crees que la tecnología puede mejorar la experiencia del cliente y optimizar la operación de tu cafetería?
7. ¿Algo más que te gustaría agregar sobre tus necesidades o expectativas?

### Clientes de establecimiento

**Preguntas de presentación:**

1. ¿Podrías indicarnos tu nombre?
2. ¿Con qué frecuencia sueles visitar cafeterías?
3. ¿Qué tipo de cafeterías prefieres (por ejemplo, locales, cadenas, cafeterías gourmet)?

**Propósito:** Queremos conocer tu experiencia como cliente en cafeterías y cómo la tecnología podría mejorarla.

**Entrevista:**

1. ¿Cómo sueles consultar la disponibilidad de mesas antes de ir a una cafetería?
2. ¿Qué tan importante es para ti poder hacer reservas online para evitar esperas?
3. ¿Te gustaría ver la disponibilidad de mesas en tiempo real a través de una app?
4. ¿Qué características debería tener una app de cafetería para que la uses con frecuencia?
5. ¿Cómo valoras la rapidez y facilidad de uso de una aplicación para gestionar tu experiencia en la cafetería?
6. ¿Algo más que consideras importante para mejorar tu experiencia como cliente?

### 2.2.2. Registro de entrevistas
### Propietarios de cafeterías
**Entrevista #1**

**Entrevista #2**

### Clientes de establecimiento
**Entrevista #1**

**Link:** [https://drive.google.com/file/d/1CVDQx8Ue15xk7yt8oukkN1S87bAc7TeB/view?usp=sharing](https://drive.google.com/file/d/1CVDQx8Ue15xk7yt8oukkN1S87bAc7TeB/view?usp=sharing) 

**Entrevistado:** Elias Yauri Paucar<br>
**Duración:** 3:18

<img src="images/entrevistas/elias.png"><br>

**Resumen:** El entrevistado indica que acostumbra visitar diferentes tipos de cafeterías, incluyendo tanto establecimientos gourmet como cadenas comerciales. Cuando tiene la opción, verifica la disponibilidad de espacio antes de ir, aunque no siempre lo hace. Expresa interés en poder acceder a información sobre disponibilidad y otros detalles similares. <br>Respecto a aplicaciones, valora principalmente tres aspectos: una interfaz intuitiva, facilidad de uso y funcionalidades relevantes. Finalmente, para el entrevistado es fundamental que la navegación dentro de la aplicación sea sencilla de comprender y que ofrezca una experiencia fluida.

**Entrevista #2**

**Link:** [https://youtu.be/QGSisj7iF-k](https://youtu.be/QGSisj7iF-k)

**Entrevistada:** Aleshka Fernández<br>
**Duración:** 3:54

<img src="images/entrevistas/Aleshka.png"><br>

**Resumen:** La entrevistada menciona que suele visitar cafeterías locales que ofrezcan cafés artesanales o exclusivos del establecimiento. Destaca que, cuando tiene poco tiempo, valora poder reservar sus lugares favoritos. También muestra interés en conocer el aforo en tiempo real. Le gustaría que la aplicación fuera intuitiva, atractiva y visualmente llamativa. Además, considera ideal que la app le sugiera las mejores cafeterías cercanas, según su ubicación y el tipo de cafetería que prefiere. También desea encontrar fácilmente un buscador dentro de la aplicación, dejar calificaciones sobre los lugares visitados y recibir recomendaciones de cafeterías similares en caso de que el tiempo de espera en su lugar habitual sea muy largo.

### 2.2.3. Análisis de entrevistas
### Propietarios de cafeterías

### Clientes de establecimiento

## 2.3. Needfinding
### 2.3.1. User Personas
Propietarios de cafeterías

![Propietarios](./images/needfinding/UserStoryPropietario.png)

Clientes de establecimiento

![Clientes](./images/needfinding/UserStoryCliente.png)

### 2.3.2. User Task Matrix
Propietarios de cafeterías

| Tarea |   Importancia   | Frecuencia |
|:------|:------|:----------|
|Consultar el estado de ocupación de mesas|Alta|Alta|
|Agregar/modificar mesas desde el panel administrativo|Media|Media|
|Gestionar reservas desde el panel|Media|Media|
|Configurar parámetros iniciales (sede, nombre, etc.)|Media|Baja|
|Supervisar que el sistema esté funcionando correctamente|Alta|Alta|
|Ver reportes o estadísticas de uso (futura función)|Alta|Media|

Clientes de establecimiento

| Tarea |   Importancia   | Frecuencia |
|:------|:------|:----------|
|Consultar disponibilidad de mesas en tiempo real|Alta|Alta|
|Acceder rápidamente desde el celular|Alta|Alta|
|Buscar cafeterías cercanas con disponibilidad|Alta|Media|
|Guardar su cafetería favorita (opcional futuro)|Media|Baja|
|Compartir o recomendar la cafetería con amigos|Media|Media|

### 2.3.3. User Journey Mapping
Propietarios de cafeterías

![Propietarios](./images/needfinding/UserJourneyMappingPropietario.png)

Clientes de establecimiento

![Clientes](./images/needfinding/UserJourneyMappingCliente.png)

### 2.3.4. Empathy Mapping
Propietarios de cafeterías

![Propietarios](./images/needfinding/EmpathyMappingPropietario.png)

Clientes de establecimiento

![Clientes](./images/needfinding/EmpathyMappingCliente.png)

### 2.3.5. As-is Scenario Mapping
Propietarios de cafeterías

| FASES | Apertura del local | Horas pico | Tiempos muertos o baja rotación | Cierre y evaluación |
|-------|--------------------|------------|---------------------------------|---------------------|
| **DOING** | Llego temprano a preparar el salón y reviso la limpieza <br><br> Organizo al personal según la estimación de flujo del día <br><br> Activo los pedidos de proveedores y abro caja | Superviso el movimiento del salón y doy indicaciones rápidas <br><br> Coordino con el personal para liberar mesas <br><br> Intento gestionar manualmente el flujo de comensales | Trato de motivar al personal a optimizar ocupación <br><br> Me enfoco en redes, promociones o planificación de eventos | Reviso la caja, analizo el desempeño del día <br><br> Comento con el equipo los problemas que se presentaron |
| **THINKING** | “¿Cómo puedo organizar mejor al equipo si se llena?” | “¿Hay alguien esperando afuera? ¿Ya se fue esa mesa del fondo?” <br><br> “Estamos perdiendo ventas por no rotar bien las mesas” | “¿Se estará yendo gente por no ver mesas disponibles?” <br><br> “¿Debemos reducir el horario de atención?” | “Hoy podríamos haber ganado más si organizábamos mejor” <br><br> “¿Y si hubiera una forma de saber cuántas mesas se usan realmente?” |
| **FEELING** | Expectativa positiva <br><br> Ligera ansiedad por la incertidumbre del día | Estrés por la carga simultánea de tareas <br><br> Frustración al ver ineficiencia en la atención | Impotencia por no tener visibilidad clara del flujo <br><br> Curiosidad por probar nuevas soluciones, pero con dudas | Frustración al no tener datos para tomar decisiones <br><br> Motivación parcial por mejorar, pero sin claridad sobre el cómo |

Clientes de establecimiento

| FASES | Decisión de salir | Camino al local | Llegada y evaluación del lugar | Cambio de plan o espera |
|-------|-------------------|-----------------|--------------------------------|-------------------------|
| **DOING** | Consulto Google Maps o redes sociales para elegir una cafetería <br><br> Pregunto a amigos si conocen un lugar con espacio <br><br> Busco una opción con buen ambiente y sin demasiada gente | Voy caminando o en transporte mientras reviso reseñas <br><br> Consulto stories o publicaciones recientes del local | Me asomo o entro para ver si hay mesas <br><br> Hablo con un mozo o espero que me asignen espacio <br><br> Evalúo el ambiente | Decido esperar de pie, buscar otro local o cancelar mi plan <br><br> Dejo una reseña o me quejo en redes si tuve mala experiencia |
| **THINKING** | “¿Estará lleno ese lugar que me gusta?” <br><br> “Sería genial saber desde casa si hay mesas” | “No tengo ganas de andar buscando otro lugar” <br><br> “Si llego y no hay lugar, capaz me vuelvo a casa” | “No hay lugar, otra vez” <br><br> “¿Por qué no hay una app para esto?” | “No vuelvo más a este lugar sin saber si hay lugar antes” |
| **FEELING** | Entusiasmo por salir a tomar algo o trabajar fuera <br><br> Inseguridad por no saber si encontrará lugar | Expectativa mezclada con incertidumbre <br><br> Poca paciencia, sobre todo si va con tiempo limitado | Decepción si no encuentra lugar <br><br> Irritación si ve mesas vacías sin uso | Frustración, molestia, desilusión <br><br> Sensación de que no valoraron su tiempo |

## 2.4. Ubiquitous Language
Estos son los términos y conceptos comunes utilizados en nuestro proyecto:

- **Sede:** Unidad donde opera una cafetería. Cada sede puede tener múltiples mesas y su propio panel administrativo.
- **Mesa:** Elemento disponible para ser ocupado por los clientes. Puede ser activada o desactivada desde el panel.
- **Silla con sensor:** Elemento equipado con un sensor de peso que detecta si está siendo utilizada. Su estado ayuda a determinar la ocupación de la mesa.
- **Sensor:** Dispositivo IoT instalado en cada silla que detecta cambios de peso para determinar si hay una persona sentada.
- **Ocupación:** Estado de una mesa, determinado por la detección de presencia en una o más sillas asociadas.
- **Panel administrativo:** Interfaz web usada por el propietario o administrador para gestionar mesas, consultar disponibilidad y visualizar estadísticas.
- **Administrador:** Usuario con control sobre una sede, encargado de gestionar mesas, configuraciones y visualización de datos.
- **Cliente:** Persona que visita la cafetería. Puede usar la app para ver disponibilidad de mesas en tiempo real.
- **Actualización de estado:** Proceso automático mediante el cual el sistema recibe datos de los sensores en las sillas y actualiza la información visible para clientes y administradores.
- **Rotación de mesas:** Número de veces que una mesa es ocupada en un período determinado. Métrica usada para medir eficiencia.



## 3.1. To-Be Scenario Mapping
Este mapeo “To-Be” presenta el escenario ideal posterior a la implementación de Tavolo, describiendo cómo cambiarán las experiencias del propietario de la cafetería y del comensal gracias a la solución IoT propuesta. Se detallan acciones, pensamientos y emociones alineadas a los beneficios que aporta el sistema.

### ¿Qué hace el Dueño del Café?

| **Phases**                     | **Doing**                                                                                          | **Thinking**                                           | **Feeling**               |
|-------------------------------|-----------------------------------------------------------------------------------------------------|--------------------------------------------------------|---------------------------|
| **Registro del local**        | • Instala la app Tavolo.  <br> • Crea su cuenta como dueño de local.  <br> • Registra su cafetería y sedes. | • “Qué bueno que puedo registrar todas mis sedes fácil.” <br> • “Ahora tengo visibilidad online.” | • Aliviado <br> • Organizado |
| **Gestión del aforo**         | • Consulta la ocupación en tiempo real de su sede. <br> • Revisa cada sede desde su celular o computadora.                    | • “Qué fácil es ver cuántas mesas están ocupadas.” <br> • “Ya no dependo del personal para esto.” <br>• “Qué accesible que pueda ver desde cualquier dispositivo la app de Tavolo.” | • En control <br> • Eficiente  |
| **Gestión del tiempo de espera** | • Ve cómo los clientes reservan online. <br> • Evita colas en la entrada.                             | • “Qué bueno que ya no hay filas innecesarias.” <br> • “Mis clientes llegan más contentos.”      | • Relajado <br> • Optimista   |
| **Monitoreo de mesas**        | • Agrega o elimina mesas. <br> • Coordina instalación de sensores IoT.                              | • “Wow, es sencillo gestionar las mesas con ayuda.” <br> • “No imaginé tanta flexibilidad.”      | • Empoderado <br> • Innovador  |
| **Visibilidad en Google Maps**| • Permite que los clientes lo busquen por nombre. <br> • Revisa su sede en la app de Tavolo.          | • “Qué útil que aparezcamos en Google con mis datos.” <br> • “Nos encuentran más rápido.”        | • Conectado <br> • Satisfecho  |

### ¿Qué hace el Usuario?

| Phases | Descubrimiento de la aplicación | Registro de datos personales | Búsqueda de cafeterías | Reserva de asientos |
|--------|-------------------------------|----------------------------|------------------------|-------------------|
| **Doing** | • Descarga Tavolo desde la tienda de aplicaciones.<br>• Explora las funcionalidades principales. | • Registra sus datos en Tavolo.<br>• Configura sus cafeterias favoritas. | • Utiliza la función de búsqueda por ubicación.<br>• Revisa la disponibilidad en tiempo real. | • Selecciona una mesa disponible.<br>• Confirma la reserva para una hora específica. |
| **Thinking** | "Esta app me ayudará a no perder tiempo buscando lugares disponibles." | "El proceso de registro es rápido." | "Me encanta poder ver exactamente dónde hay espacio antes de ir." | "La reserva fue sencilla y ahora tengo mi lugar asegurado." |
| **Feeling** | Curiosidad | Comodidad | Alivio | Satisfacción |


## 3.2. User Stories
### Épicas de Tavolo

| Epic ID | Nombre |
|---------|--------|
| EPIC-LANDING-001 | Funcionalidades landing page |
| EPIC-CLIENT-002 | Funcionalidades user comensal |
| EPIC-ADMIN-003 | Funcionalidades user administrador |
| EPIC-SUPERADMIN-004 | Funcionalidades user superadmin |

### Landing Page (EPIC-LANDING-001)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US001 | Ver sección "¿Qué es Tavolo?" | Como visitante de la página, quiero entender qué es Tavolo desde la landing page para conocer su propósito y cómo puede ayudarme como comensal o administrador de cafetería. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el visitante accede a la landing page<br>Cuando hace scroll o clic en "¿Qué es Tavolo?"<br>Entonces el sistema le muestra la sección donde se describe claramente el objetivo de la solución |
| US002 | Ver sección "Características clave" | Como visitante, quiero revisar una lista de características principales de Tavolo para evaluar si cubre mis necesidades como usuario final o administrador. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el usuario navega la landing<br>Cuando accede a la sección "Características clave"<br>Entonces el sistema le muestra un resumen de las funcionalidades más importantes del sistema |
| US003 | Ver la galería virtual | Como visitante, quiero ver una galería virtual en la landing para visualizar cómo luce Tavolo, su interfaz y los sensores en acción. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el usuario accede a la sección "Galería Virtual"<br>Cuando visualiza las imágenes o videos<br>Entonces el sistema le muestra el contenido visual ilustrativo del sistema en uso |
| US004 | Usar el formulario de contacto | Como visitante interesado, quiero tener acceso a un formulario o medio de contacto en la landing para comunicarme con el equipo de Tavolo. | EPIC-LANDING-001 | Visitante landing page | **Escenario 1:**<br>Dado que el visitante accede a "Contáctanos"<br>Cuando completa el formulario con sus datos<br>Entonces el sistema debe notificar al equipo de Tavolo |

### Usuario Comensal (EPIC-CLIENT-002)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US005 | Ver menú digital de una sede | Como comensal, quiero visualizar el menú de la cafetería para conocer los productos disponibles antes de asistir. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal accede a la app<br>Cuando le da click a la sección "Menú"<br>Entonces el sistema debe mostrar el menú completo de la cafetería |
| US006 | Visualizar reserva activa | Como comensal, quiero poder visualizar mi reserva activa desde la aplicación, para confirmar los detalles de mi mesa y el horario reservado antes de llegar a la cafetería. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal ha iniciado sesión en la aplicación<br>Y tiene al menos una reserva activa<br>Cuando accede a la sección principal<br>Entonces el sistema le muestra la información de la reserva actual incluyendo horario, sede y número de mesa |
| US007 | Ver disponibilidad de mesas en tiempo real | Como comensal, quiero conocer la disponibilidad de mesas para decidir que sede visitar de la cafetería. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal accede a la app<br>Cuando le da click a la sección "Explorar Sedes"<br>Entonces el sistema debe mostrarle la información de la sedes con sus respectivos aforos disponibles<br><br> **Escenario 2:**<br>Dado que el comensal visualiza el estado de aforo de las sedes<br>Cuando hay una actualización desde los sensores<br>Entonces el sistema debe reflejar el nuevo estado en menos de 5 segundos<br><br>**Escenario 3:**<br>Dado que todas las mesas están ocupadas en una sede<br>Cuando el comensal visualiza la disponibilidad<br>Entonces el sistema debe informar que no hay mesas disponibles actualmente |
| US008 | Reservar una mesa | Como comensal, quiero reservar una mesa para asegurarme un lugar al llegar a la cafetería. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal selecciona una sede en la sección "Explorar Sedes"<br>Cuando el comensal selecciona la hora aproximada de estadía<br>Y selecciona una mesa disponible<br>Entonces el sistema debe permitir realizar la reserva<br><br>**Escenario 2:**<br>Dado que el comensal ya tiene una reserva activa<br>Cuando intenta crear una nueva<br>Entonces el sistema debe evitarlo e informar que ya tiene una reserva activa |
| US009 | Visualizar más sedes en un mapa | Como comensal, quiero poder ver más sedes en el mapa para poder identificar el más cercano. | EPIC-CLIENT-002 | Comensal | **Escenario 1:**<br>Dado que el comensal quiere ver más sedes<br>Cuando le da click a la sección "Explorar sedes" <br>Y tipea el nombre de la sede en el buscador<br>Entonces el sistema debe mostrar todas las sedes de la cafetería en el mapa interactivo |
| US015 | Registro de cuenta de comensal | Como visitante, quiero poder registrarme como comensal en el sistema Tavolo para poder acceder a las funcionalidades de reserva y visualización de mesas. | EPIC-CLIENT-002 | Visitante | **Escenario 1:**<br>Dado que un visitante accede a la aplicación<br>Cuando completa el formulario de registro con nombre, correo y contraseña<br>Y acepta los términos y condiciones<br>Entonces el sistema debe crear una cuenta nueva<br>Y permitir el acceso a las funcionalidades de comensal |
| US016 | Login de cuenta de comensal | Como comensal registrado, quiero poder iniciar sesión en el sistema para acceder a mis reservas y funcionalidades personalizadas. | EPIC-CLIENT-002 | Comensal registrado | **Escenario 1:**<br>Dado que un comensal registrado accede a la pantalla de login<br>Cuando ingresa sus credenciales correctas (email y contraseña)<br>Entonces el sistema debe autenticarlo<br>Y redirigirlo al dashboard principal<br><br>**Escenario 2:**<br>Dado que un usuario ingresa credenciales incorrectas<br>Cuando intenta iniciar sesión<br>Entonces el sistema debe mostrar un mensaje de error<br>Y permitir reintentar |

### Usuario Administrador (EPIC-ADMIN-003)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US010 | Agregar nuevas mesas | Como administrador de cafetería, quiero agregar mesas al sistema para gestionar mejor la ocupación. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el admin accede al panel de su sede<br>Cuando le da click a la sección "Gestión de Mesas"<br>Y posteriormente a la opción "Agregar una nueva mesa" <br> Entonces el sistema le brinda un formulario simple de registro de mesa. <br>**Escenario 2:** <br> Dado que el admin ingresa los datos correctos de la mesa como su identificador y capacidad de sillas <br>Y le da click al botón "Guardar"<br>Entonces el sistema guarda con su identificador y capacidad de sillas la mesa registrada |
| US011 | Visualizar reservas realizadas | Como administrador, quiero ver las reservas registradas en mi sede para planificar el servicio. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el admin accede a su sede<br>Cuando le da clic a la sección "Visualizar Reservas"<br>Entonces el sistema debe mostrar las reservas con usuario, fecha y hora |
| US012 | Ver la sede asignada | Como administrador, quiero confirmar qué sede tengo asignada para asegurarme de gestionar la correcta. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el admin inicia sesión<br>Cuando accede a su información<br>Entonces el sistema debe mostrar la sede asociada a su cuenta |
| US013 | Eliminar mesas | Como administrador, quiero poder eliminar mesas que ya no están en uso en mi sede, para mantener el sistema actualizado y evitar asignaciones incorrectas. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que el administrador ha iniciado sesión<br>Y se encuentra en la sección "Ver Mesas"<br>Cuando selecciona una mesa existente y confirma su eliminación<br>Entonces la mesa es eliminada del sistema y deja de aparecer en la lista |
| US017 | Login de administrador | Como administrador, quiero poder iniciar sesión en el sistema con mis credenciales específicas para acceder al panel de administración de mi sede. | EPIC-ADMIN-003 | Administrador | **Escenario 1:**<br>Dado que un administrador accede a la pantalla de login<br>Cuando ingresa sus credenciales válidas<br>Entonces el sistema debe autenticarlo<br>Y mostrar el panel de administración con las funcionalidades asociadas a su sede<br><br>**Escenario 2:**<br>Dado que un administrador ingresa credenciales incorrectas<br>Cuando intenta acceder<br>Entonces el sistema debe mostrar un mensaje de error<br>Y registrar el intento fallido por seguridad |

### Usuario Superadmin (EPIC-SUPERADMIN-004)

| Story ID | Título | Descripción | Epic ID | Usuario | Criterios de aceptación |
|----------|--------|-------------|---------|---------|------------------------|
| US014 | Acceder a todos los módulos del sistema | Como superadmin, quiero tener acceso a todas las funcionalidades del sistema para realizar pruebas, crear sedes y admins. | EPIC-SUPERADMIN-004 | Superadmin | **Escenario 1:**<br>Dado que el superadmin accede al sistema<br>Cuando desea visualizar sedes o usuarios<br>Entonces el sistema debe permitirle ver toda la información<br><br>**Escenario 2:**<br>Dado que el superadmin crea un nuevo admin o sede<br>Cuando registra los datos<br>Entonces el sistema debe almacenarlos y mostrar confirmación |


## 3.3. Impact mapping.
<img src="./images/impact_mapping/Impact_Mapping.png" alt="Impact Mapping"/><br>



## 3.4. Product Backlog.

| #  | User Story Id | Título                                     | Descripción                                                                                                                                                                    | Story Points |
|----|---------------|--------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
|  1 | US014         | Acceder a todos los módulos del sistema    | Como superadmin, quiero tener acceso a todas las funcionalidades del sistema para realizar pruebas, crear sedes y admins.                                                      |            8 |
|  2 | US010         | Agregar nuevas mesas                       | Como administrador de cafetería, quiero agregar mesas al sistema para gestionar mejor la ocupación.                                                                            |            8 |
|  3 | US009         | Visualizar más sedes en un mapa            | Como comensal, quiero poder ver más sedes en el mapa para poder identificar el más cercano.                                                                                    |            8 |
|  4 | US015         | Registro de cuenta de comensal             | Como visitante, quiero poder registrarme como comensal en el sistema Tavolo para poder acceder a las funcionalidades de Tavolo.                                                |            5 |
|  5 | US016         | Login de cuenta de comensal                | Como comensal registrado, quiero poder iniciar sesión en el sistema para acceder a mis reservas o visualizar la disponibilidad y el menú de una sede en específico.            |            5 |
|  6 | US012         | Ver la sede asignada                       | Como administrador, quiero confirmar qué sede tengo asignada para asegurarme de gestionar la correcta.                                                                         |            5 |
|  7 | US008         | Reservar una mesa                          | Como comensal, quiero reservar una mesa para asegurarme un lugar al llegar a la cafetería.                                                                                     |            5 |
|  8 | US013         | Eliminar mesas                             | Como administrador, quiero poder eliminar mesas que ya no están en uso en mi sede, para mantener el sistema actualizado y evitar asignaciones incorrectas.                     |            5 |
|  9 | US006         | Visualizar reserva activa                  | Como comensal, quiero poder visualizar mi reserva activa desde la aplicación, para confirmar los detalles de mi mesa y el horario reservado antes de llegar a la cafetería.    |            5 |
| 10 | US007         | Ver disponibilidad de mesas en tiempo real | Como comensal, quiero conocer la disponibilidad de mesas para decidir que sede visitar de la cafetería.                                                                        |            5 |
| 11 | US004         | Usar el formulario de contacto             | Como visitante interesado, quiero tener acceso a un formulario o medio de contacto en la landing para comunicarme con el equipo de Tavolo.                                     |            3 |
| 12 | US005         | Ver menú digital de una sede               | Como comensal, quiero visualizar el menú de la cafetería para conocer los productos disponibles antes de asistir.                                                              |            3 |
| 13 | US011         | Visualizar reservas realizadas             | Como administrador, quiero ver las reservas registradas en mi sede para planificar el servicio.                                                                                |            3 |
| 14 | US003         | Ver la galería virtual                     | Como visitante, quiero ver una galería virtual en la landing para visualizar cómo luce Tavolo, su interfaz y los sensores en acción.                                           |            2 |
| 15 | US002         | Ver sección "Características clave"        | Como visitante, quiero revisar una lista de características principales de Tavolo para evaluar si cubre mis necesidades como usuario final o administrador.                    |            2 |
| 16 | US001         | Ver sección "¿Qué es Tavolo?"              | Como visitante de la página, quiero entender qué es Tavolo desde la landing page para conocer su propósito y cómo puede ayudarme como comensal o administrador de cafetería.   |            2 |
| 17 | US017         | Login de administrador                     | Como administrador, quiero poder iniciar sesión en el sistema con mis credenciales específicas como: usuario y contraseña, para acceder al panel de administración de mi sede. |            2 |

