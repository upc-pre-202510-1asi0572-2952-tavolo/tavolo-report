

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


