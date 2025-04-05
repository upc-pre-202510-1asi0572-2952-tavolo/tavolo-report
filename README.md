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
      - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
      - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
  - [1.3. Segmentos objetivo](#13-segmentos-objetivo)
    - [Perfil Demográfico](#perfil-demográfico)
    - [Perfil Psicográfico](#perfil-psicográfico)
    - [Hábitos y necesidades clave](#hábitos-y-necesidades-clave)
    - [Ejemplos de usuarios tipo](#ejemplos-de-usuarios-tipo)

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
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi. In hac habitasse platea dictumst. Aenean euismod neque vitae diam venenatis rutrum. Vivamus lobortis iaculis blandit. Nunc tempus accumsan nibh nec sagittis. Vivamus accumsan augue sed leo imperdiet efficitur. Aliquam laoreet in eros vitae dapibus. In et aliquet mauris. Etiam in ex varius, sodales purus in, euismod tellus. Aliquam vel enim turpis. In dignissim mauris ut ante euismod, a maximus eros ultricies. Etiam sit amet porttitor mi. Aliquam erat volutpat. Aliquam erat volutpat.
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
      <img src="./assets/profile_images/Fabio_image.jpg" alt="Franz's profile image" min-width="400" max-width="900"/>
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
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel erat sit amet enim fringilla tincidunt ut ut mi. In hac habitasse platea dictumst. Aenean euismod neque vitae diam venenatis rutrum. Vivamus lobortis iaculis blandit. Nunc tempus accumsan nibh nec sagittis. Vivamus accumsan augue sed leo imperdiet efficitur. Aliquam laoreet in eros vitae dapibus. In et aliquet mauris. Etiam in ex varius, sodales purus in, euismod tellus. Aliquam vel enim turpis. In dignissim mauris ut ante euismod, a maximus eros ultricies. Etiam sit amet porttitor mi. Aliquam erat volutpat. Aliquam erat volutpat.
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

#### 1.2.2.2. Lean UX Assumptions  

#### 1.2.2.3. Lean UX Hypothesis Statements  

**Supuesto:**  
Creemos que permitir a los usuarios ver en tiempo real la disponibilidad de asientos en nuestras sedes mejorará su experiencia de planificación y reducirá la frustración por llegar a un lugar lleno.

**Para:**  
Usuarios que trabajan o estudian fuera de casa y buscan un lugar tranquilo para sentarse con su laptop o tomar café.

**Nuestro producto/servicio:**  
Es una aplicación web y móvil que muestra la disponibilidad de asientos en tiempo real gracias a sensores IoT, además del menú del café y la opción de reservar.

**Nos ayudará a lograr:**  
Mejorar la organización de los usuarios y optimizar el uso de los espacios en las sedes, evitando aglomeraciones y maximizando la rotación de clientes satisfechos.

**Mediremos el éxito a través de:**  
- Número de reservas realizadas desde la app.  
- Disminución de quejas por falta de espacio.  
- Aumento de visitas a sedes menos concurridas gracias a la recomendación automática.  

#### 1.2.2.4. Lean UX Canvas

| **Sección**                | **Contenido para TAVOLO**                                                                 |
|---------------------------|-------------------------------------------------------------------------------------------|
| 1. Business Problem        | Muchos clientes llegan a las sedes y no encuentran asientos disponibles, lo que genera frustración y pérdida de clientes. |
| 2. Business Outcomes       | - Aumentar la rotación eficiente de clientes.<br>- Mejorar la experiencia de visita.<br>- Promover otras sedes con menor aforo. |
| 3. Users and Customers     | - Estudiantes, trabajadores remotos, freelancers.<br>- Personas que buscan un lugar cómodo para pasar tiempo. |
| 4. User Benefits           | - Ahorran tiempo y frustración.<br>- Pueden planificar mejor sus visitas.<br>- Pueden revisar el menú antes de llegar. |
| 5. Solutions Ideas         | - Ver aforo en tiempo real con sensores IoT.<br>- Reserva de asientos.<br>- Sugerencia automática de otras sedes. |                                                      |
| 6. Key Assumptions         | - Los usuarios realmente desean saber el aforo antes de ir.<br>- Usarán la app para hacer reservas.<br>- Los sensores IoT funcionarán de forma confiable. |
| 7. Experimentation         | - Medir reservas vs. aforo real.<br>- Encuestas a usuarios después del uso de la app. |


## 1.3. Segmentos objetivo

### Perfil Demográfico
- Jóvenes adultos entre 18 y 35 años.  
- Estudiantes universitarios y profesionales jóvenes.  
- Principalmente ubicados en zonas urbanas con acceso a tecnología y múltiples sedes del café.

### Perfil Psicográfico
- Personas que valoran su tiempo y organización personal.  
- Tienen un estilo de vida activo, flexible y con movilidad constante.  
- Están familiarizados con el uso de apps para planificar, reservar y tomar decisiones rápidas.

### Hábitos y necesidades clave
- Buscan lugares tranquilos y cómodos para trabajar, estudiar o socializar.  
- Prefieren evitar la incertidumbre de encontrar espacios disponibles.  
- Desean información clara antes de desplazarse (aforo, menú, ubicación).  
- Valoran la posibilidad de reservar o planificar con antelación desde su smartphone.

### Ejemplos de usuarios tipo
-  Estudiante universitaria que necesita un lugar para estudiar con su laptop entre clases.  
-  Freelancer o trabajador remoto que busca un lugar productivo con buena conexión.  
-  Creativo independiente que rota entre cafés para inspirarse y trabajar.  
-  Amigos que planean reunirse a tomar café y quieren saber dónde hay espacio libre.





