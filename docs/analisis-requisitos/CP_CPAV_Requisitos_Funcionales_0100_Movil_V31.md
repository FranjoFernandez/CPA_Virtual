![](./media/Pictures/100000000000033E000004915BFB5B90B227BCAA.jpg){width="24.067cm"
height="34.022cm"}

> **Junta de Andalucía**

> Centro Participación Activa Virtual App Móvil. Requisitos Funcionales.

> 

> 

> **Certificado de Entrega**

> Estado del documento: Borrador

> Versión: 3.1

> Fecha entrega: 02 septiembre 2025

> 

> 

> **Confidencialidad comercial**

# []{#anchor}[]{#anchor-1}Control del documento

  ---------------------------------- -------------------------------------------------------------------------------------
  **Título:**                        Centro Participación Activa Virtual App Móvil. Requisitos Funcionales.
  **Cliente:**                       Junta de Andalucía -- Consejería de Inclusión Social, Juventud, Familias e Igualdad
  **Referencia:**                    
  **Versión:**                       3.1
  **Fecha Entrega:**                 
  **Autor:**                         UTE Babel Getronics
  **Páginas Totales:**               
  **Tipo Seguridad:**                Confidencialidad Comercial
  **Distribución:**                  Getronics
  **Descargo de responsabilidad:**   Este documento no está controlado cuando se imprime.
  ---------------------------------- -------------------------------------------------------------------------------------

\

**Aprobación de documentos**

  ------------------- -- --------------------
  **Aprobado Por:**      Aprobación Inicial
  ------------------- -- --------------------

**Historial de Versiones**

  **Versión**   **Fecha**    Expedido por   **Estado**   Comentarios
  ------------- ------------ -------------- ------------ --------------------------------------------------------------------------------------------------------------------------------------------
  0.1           27/05/2025                  Borrador     Borrador Inicial del Documento. Alcance Fase1 y Fase 2 App Móvil.
  0.2           19/06/2025                  Borrador     Se añade personalización del menú en función del centro al que pertenezca el usuario autenticado.
  1.0           24/06/2025                  Borrador     Se añaden instancias de CPA Virtual para Personas Socias y CPA Virtual Administración para Administradores, Plantilla CPA y Profesionales.
  1.1           10/07/2025                  Borrador     Actualización de funcionalidades.
  2.0           08/08/2025                  Borrador     Actualización de funcionalidades.
  3.0           14/08/2025                  Borrador     Se añaden funcionalidades de servicios
  3.1           02/09/2025                  Borrador     Añadir funcionalidad solicitudes alta usuarios por parte de la persona socia y CRUD por parte del administrador.

**Declaración ISO**

Getronics aplica sistemas de gestión globales que cubren varias normas
ISO (9001, 14001, 20000, 22301, 27001, 50000), con certificados BSI que
cubren muchos países, véase[]{#anchor-2}:

[www.getronics.com/policy-pages/iso-itil/](https://www.getronics.com/policy-pages/iso-itil/)\

# []{#anchor-3}[]{#anchor-4}Introducción

## []{#anchor-5}[]{#anchor-6}Propósito

Este documento describe los requisitos funcionales para el desarrollo de
una aplicación destinada a la Junta de Andalucía. La aplicación
permitirá a los usuarios desarrollar y proporcionar un Sistema Web
Social-Colaborativo a la Consejería de Inclusión Social, Juventud,
Familias e Igualdad con el que se facilite la comunicación, la
participación y la gestión telemática de los servicios de los Centros de
Participación Activa (CPA) de Andalucía.

- 

  Permitirá extender y mejorar el nivel de accesibilidad de las personas
  socias/usuarias/profesionales de los Centros de Participación Activa
  (CPAs) de Andalucía facilitando a los usuarios la tramitación de su
  condición de persona socia y usuaria del CPA, permitiendo la gestión
  de la participación de las personas solicitantes en los diversos
  eventos, fomentando la comunicación y la interrelación de las personas
  mayores entre sí y con los profesionales de los CPA.

Para ello se propone que el sistema a desarrollar esté compuesto de una
plataforma digital accesible desde cualquier tipo de terminal, fijo o
móvil, y con distintos sistemas operativos y de una APP para que las
personas socias/usuarias y usuarias de los CPA.

Desde la plataforma web 'CPA Virtual Administración' se realizará la
gestión ý difusión de contenidos y servicios de los Centros de Población
Activa de Andalucía y desde 'CPA Virtual' accesible desde la plataforma
web y la aplicación móvil complementaria (en dispositivos con sistema
operativo Android e IOS), se facilitará a los usuarios la conexión con
la Web desde todo tipo de dispositivos móviles, tales como móviles,
tablets o Android TV box, facilitándose el acceso a los servicios
ofrecidos desde cualquier dispositivo.

El nuevo proyecto CPA Virtual permitirá la gestión integral de usuarios
y servicios, fomentará la interacción social entre usuarios y
profesionales, ofrecerá funcionalidades avanzadas como la emisión en
directo de talleres y actividades o la publicación de información sobre
los CPA e incluirá herramientas para la explotación de datos, junto con
recursos formativos y videotutoriales para usuarios y profesionales.

Además, el proyecto deberá incluir un plan de formación para una
formación especializada en el uso de la herramienta que se va a
desarrollar, tanto para los usuarios como para los profesionales que
hagan uso de la misma.

Por último, mencionar que este documento se centrará unicamente en las
funcionalidades que recogerá la instancia 'CPA Virtual' desde la APP
Móvil.

## []{#anchor-7}[]{#anchor-8}Descripción del Proyecto

El proyecto contendrá dos instancias:

-Plataforma web 'CPA Virtual Administración' desde donde gestionar los
contenidos y servicios por parte de los administradores y profesionales,
a ofrecer en CPA Virtual.

-Plataforma web y app móvil 'CPA Virtual' desde dónde las personas
socias/usuarias podrán disfrutar de los servicios ofrecidos por el
aplicativo e interactuar con los profesionales de cada CPA al que
pertenezcan.

- Se detalla a continuación la instancia 'CPA Virtual', a la que podrán
  acceder las Personas socias/usuarias desde la app móvil:

- Ser accesible por Internet desde cualquier tipo de terminal fijo y/o
  móvil mediante navegador web y desde diferentes sistemas operativos
  (windows, ios, android, ...).

- Ser accesible para personas con deficiencia visual y/o auditiva.

- Acceder a una zona pública de contenidos (noticias, talleres,
  actividades) de interés ofrecidos por las distintas CPAs, para las
  personas socias/usuarias de dichas CPAs y las personas profesionales.

- Autenticación por parte de las personas socias/usuarias de cada CPA
  para poder acceder a la parte privada del aplicativo CPA Virtual.

- Personalización de menú en función del perfil o perfiles del usuario.

- Registrarse como personas socias/usuarias de un CPA, para acceder a
  las funcionalidades privadas ofrecidas por las distintas CPA de forma
  individual y personalizada, realizándose en la tramitación la
  comprobación de los requisitos de Identidad y Residencia a través de
  la plataforma SCSP y firmada digitalmente. Pudiendo encontrarse
  distintos escenarios:

  \*Que la persona no sea ni usuaria de la plataforma, ni socia de
  ningún CPA.

- \*Que la persona haya podido completar el proceso de registro en la
  plataforma, es decir: sea usuaria, pero no el de la solicitud de
  asociación por la complejidad del uso del certificado electrónico para
  esa persona.

- \*Que la persona sea socia de un CPA, pero aún no se haya dado de alta
  en la plataforma como usuaria.

- Registro y alta de nuevas personas socias/usuarias, hacer baja de las
  mismas o modificar su situación. En el caso de personas
  socias/usuarias, mediante una importación de éstos, con la información
  necesaria para confirmar su identidad. En el caso de usuarios no
  socios, una vez registrados en la plataforma con un mínimo de datos y
  confirmación de éste a través del email, los usuarios dispondrán de un
  botón en el home, que les permita realizar su suscripción como socios.
  Dichas solicitudes podrán ser admitidas o rechazadas por el
  administrador correspondiente.

- El conjunto de actividades que los CPA ofrecen a sus socias/usuarias
  se pueden dividir en tres grandes grupos:

  \*Talleres (baile, pintura, historia, etc.): Eventos con un plazo de
  suscripción, un plazo de realización, un aforo máximo y evaluación por
  parte de las personas socias/usuarias que los realizan. También se
  caracterizan porque los recursos humanos y físicos se planifican a la
  hora de convocar el taller. Los talleres tienen un seguimiento de
  asistencia por parte de los profesionales que lo imparten. No todos
  los CPA dan los mismos talleres, pero si están obligados a dar al
  menos un taller de cada Área que el proyecto Sum@ clasifica cada año.

  0.  0.  0.  0.  0.   ****\*Actividades (película, exposición,
                      conferencia): Eventos propios de cada centro con
                      una suscripción o cita, un lugar con día y hora
                      determinado donde se realizan. También se
                      caracterizan porque los recursos humanos y físicos
                      se planifican a la hora de publicar el evento. Las
                      actividades son exclusivas de los CPA y no están
                      condicionadas por ninguna directriz externa.

                      - - -  \*Servicios (peluquería, soporte legal,
                            gimnasio, etc.): Eventos que se ofrecen de
                            manera indefinida y que las personas
                            socias/usuarias pueden solicitar a través de
                            cita previa para acceder a estas. No todos
                            los CPA dan los mismos servicios.

- Las solicitudes de las personas socias/usuarias, desde dónde iniciar
  su tramitación mediante procedimiento administrativo.

- Las tramitaciones de las solicitudes realizadas por las personas
  socias/usuarias: Registro solicitudes, solicitudes de reconocimiento,
  otras solicitudes pendientes de tramitar (emisión de tarjetas, emisión
  de duplicados, rectificaciones, bajas, cambios de vinculación),
  liquidaciones de contrato, tramites pendientes de firma...

- El archivado del resultado de las tramitaciones de las solicitudes
  realizadas por las personas socias/usuarias.

- Evaluar los talleres.

- Evaluar las actividades.

- Consultar contenidos públicos (vídeos, imágenes, noticias,...) del
  banco contenidos, desde la zona pública de CPA Virtual, por parte de
  cualquier usuario.

- Gestionar la retransmisión contenidos (vídeos,..) zona pública, por
  parte de cualquier usuario.

- Consultar talleres (activos) públicos, desde la zona pública de CPA
  Virtual, por parte de cualquier usuario.

- Consultar actividades (activas), desde la zona pública de CPA Virtual,
  por parte de cualquier usuario.

- Consultar agenda citas previas de los servicios que puedan ser
  consumidos por las personas socias/usuarias.

- Gestionar citas previas de los servicios que puedan ser consumidos por
  las personas socias/usuarias.

- Consultar Mi CPA, zona privada, por parte de las personas
  socias/usuarias.

- Consultar Mis Trámites, zona privada, por parte de las personas
  socias/usuarias.

- Gestionar (consultas, inscripciones, cancelaciones) los talleres
  privados CPA (activos), zona privada, por parte de las personas
  socias/usuarias.

- Gestionar (consultas, inscripciones, cancelaciones) las actividades
  privadas CPA (activos), zona privada, por parte de las personas
  socias/usuarias.

- Gestionar (consultas, inscripciones, cancelaciones) los servicios
  privados CPA (activos), zona privada, por parte de las personas
  socias/usuarias.

- Permitir a las personas socias/usuarias comunicarse entre sí (chat
  público/privado, email...).

- Permitir a las personas socias/usuarias/Usuarias comunicarse con los
  profesionales de su CPA.

- Ayuda online sobre el uso general de la Plataforma, para las personas
  socias/usuarias.

- Formación mediante video tutoriales del funcionamiento de CPA Virtual.

- Formación mediante manuales de usuario, para cada uno de los perfiles
  participantes de CPA Virtual.

  Como ya se ha mencionado anteriormente, este documento se centrará
  unicamente en las funcionalidades que recogerá al aplicativo CPA
  Virtual desde la App Móvil, que se detallan en el siguiente apartado.

## []{#anchor-9}[]{#anchor-10}**Requisitos Funcionales**

Para la app móvil 'CPA Virtual', el listado general de los requisitos
funcionales que componen este documento será el siguiente:

- Acceso por Internet desde cualquier tipo de terminal fijo y/o móvil
  mediante navegador web y desde diferentes sistemas operativos (ios,
  android, ...).

- Sea accesible para personas con deficiencia visual y/o auditiva.

- Autenticación por parte del usuario para poder acceder a la parte
  privada del aplicativo CPA Virtual.

- Personalización menú en función del perfil o perfiles del usuario.

- Registro usuarios personas socias/usuarias con acceso a la zona
  privada del aplicativo por parte de los usuarios administradores CPA.

- Gestión de las solicitudes de las personas socias/usuarias por parte
  de los usuarios administradores CPA.

- Gestión de las tramitaciones de las solicitudes.

- Gestión del archivado de las tramitaciones de las solicitudes.

- Evaluaciones de las actividades.

- Consulta Contenidos (noticias, eventos,..) zona pública.

- Retransmisión Contenidos (vídeos,..) zona pública.

- Consulta Talleres CPA (activos) zona pública.

- Consulta Actividades CPA (activos) zona pública.

- Consulta Servicios CPA (activos) zona pública.

- Gestión Mi CPA, zona privada por parte de las personas
  socias/usuarias.

- Gestión Mis Trámites, zona privada por parte de las personas
  socias/usuarias.

- Gestión Comunicaciones, zona privada por parte de las personas
  socias/usuarias, desde dónde las personas socias/usuarias podrán
  comunicarse con personas profesionales de su CPA, o con otras personas
  socias/usuarias.

- Gestión Talleres privados CPA (activos), zona privada por parte de las
  personas socias/usuarias.

- Gestión Actividades privadas CPA (activos), zona privada por parte de
  las personas socias/usuarias.

- Gestión Servicios privados CPA (activos), zona privada por parte de
  las personas socias/usuarias.

- Formación mediante manuales de usuario y video tutoriales, para cada
  uno de los perfiles que interactúan con el aplicativo CPA Virtual.

- Formación en materia de configuración o setup de los elementos que
  intervienen en retransmisiones por streaming.

  Como ya se ha mencionado anteriormente, este documento se centrará
  unicamente en las funcionalidades que recogerá al aplicativo CPA
  Virtual desde la App Movil, que se detallan en el siguiente apartado.

# []{#anchor-11}[]{#anchor-12}Requisitos funcionales

## []{#anchor-13}Instancia 'CPA Virtual'

### []{#anchor-14}Acceso CPA Virtual 

El acceso a CPA Virtual para la plataforma digital por Internet podrá
realizarse desde cualquier tipo de terminal fijo mediante cualquier
navegador web y desde los sistemas operativos IOS, Android.

CPA Virtual deberá ser accesible para personas con deficiencia visual
y/o con discapacidad auditiva.

#### []{#anchor-15}Acceso CPA Virtual

- Funcionalidad: CPA Virtual será accesible por Internet desde cualquier
  tipo de terminal fijo y/o móvil mediante cualquier navegador web y
  desde diferentes sistemas operativos (IOS, Android,\...).
- Perfil usuario: Persona socia/usuaria.
- Detalles: La persona socia/usuaria de CPA Virtual podrá acceder a
  cualquiera de las pantallas de la plataforma digital, desde cualquiera
  de los navegadores web y desde cualquiera de los sistemas operativos
  que aplique.
- Ejemplo: El usuario Juan Luis Cárdenas accede a la plataforma digital
  desde el navegador Edge y el sistema operativo Android.

### []{#anchor-16}Autenticación[]{#anchor-17} Usuarios 

La autenticación de usuarios permitirá a los distintos usuarios acceder
a la parte privada del aplicativo CPA Virtual. Para ello, deberá haberse
previamente registrado como usuario de CPA, siendo del tipo 'persona
socia/usuaria'.

#### []{#anchor-18}Autenticación Usuarios

- Funcionalidad: Una vez el usuario haya sido registrado y dado de alta
  en el aplicativo CPA Virtual, deberá autenticarse mediante nombre de
  usuario y clave, para de esta forma, acceder a la parte privada.

- Perfil usuario: Usuario persona socia/usuaria.

- Detalles: Todo usuario del tipo persona socia/usuaria que desee
  acceder a la instancia 'CPA Virtual', deberá previamente autenticarse
  mediante nombre de usuario y clave. Para ello, habrá debido darse
  previamente de alta. Una vez autorizado su acceso, se presentará en la
  esquina superior derecha del escritorio sus datos personales del
  usuario autenticado: nombre y apellidos. Una vez autenticado podrá
  acceder a todos los centros a los que pertenezca o esté autorizado.
  Igualmente se le mostrarán todas las opciones de menú correspondiente
  a los distintos perfiles que pueda tener definido.

  En el caso de que haya olvidado su clave, tendrá la posibilidad de
  solicitar una nueva, cumplimentado su email y una vez recibida
  respuesta, indicando su nueva clave, la cual será almacenada en el
  sistema, quedando de esta forma registrada y actualizada.

- Ejemplo: El usuario del tipo persona socia/usuaria Juan Luis Cárdenas
  accede a la parte privada de CPA Virtual, tras introducir previamente
  su usuario/contraseña.

### []{#anchor-19}Personalización por centro de usuario 

La personalización por centro de usuario, permitirá presentar al usuario
que se haya logado en la instancia 'CPA Virtual', el centro al que
pertenece, desde la parte privada de CPA Virtual.

#### []{#anchor-20}Personalización por centro de usuario

- Funcionalidad: Una vez el usuario se haya autenticado y accedido a la
  parte privada del aplicativo CPA Virtual, se le presentará el centro
  al que pertenece.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: Todo usuario que que acceda a la parte privada del
  aplicativo CPA Virtual, tras haberse autenticado, se le presentará el
  centro al que pertenece (nombre centro y provincia centro) en la
  esquina superior derecha del escritorio, junto a los datos personales
  del usuario autenticado y el de su perfil.
- Ejemplo: El usuario Juan Luis Cárdenas, con perfil persona
  socia/usuaria, accede a la parte privada de CPA Virtual y se le
  presenta el centro al que pertenece: CPA 'Triana', con el cual
  interactuará en las distintas opciones de menú.

### []{#anchor-21}Personalización menú por perfil de usuario 

La personalización del menú por perfil de usuario, desde la parte
privada de CPA Virtual, permitirá presentar al usuario que haya logado y
en función de su perfil (obtenido previamente en función del centro al
que pertenezca el usuario), el menú con las funcionalidades que podrá
realizar.

#### []{#anchor-22}Personalización menú por perfil de usuario

- Funcionalidad: Una vez el usuario se haya autenticado y accedido a la
  parte privada del aplicativo CPA Virtual, en función de su perfil
  (obtenido previamente en función del centro al que pertenezca el
  usuario), se le presentará un menú con las funcionalidades que podrá
  realizar.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: Todo usuario que que acceda a la parte privada del
  aplicativo CPA Virtual, tras haberse autenticado y en función de su
  perfil (obtenido previamente en función del centro al que pertenezca
  el usuario), se le presentará un menú personalizado desde dónde poder
  las distintas funcionalidades que ofrece el aplicativo.
- Ejemplo: El usuario Juan Luis Cárdenas, accede a la parte privada de
  CPA Virtual y al autenticarse, accede al centro 'Triana', en el que
  tiene perfil 'persona socia/usuaria', y se le presenta el menú con las
  funcionalidades correspondientes al perfil 'persona socia/usuaria'.

### []{#anchor-23}Registro[]{#anchor-24} de Usuarios Personas socias/usuarias

El registro de usuarios de Personas socias/usuarias permitirá al usuario
anónimo solicitar el darse de alta en el CPA virtual, como persona
socia/usuaria, con el fin de obtener una cuenta desde la que poder
acceder a la zona privada de la plataforma digital y/o la app móvil.
Para ello, deberá cumplimentar la persona solicitante una solicitud con
sus datos personales, los cuales una vez completados, el cual deberá ser
firmado (digitalmente o presencialmente en el CPA que corresponda), para
finalmente, crearse una cuenta desde la que el usuario (ya persona
socia/usuaria), podrá acceder a CPA Virtual, para poder interactuar con
el CPA de su localidad.

#### []{#anchor-25}[]{#anchor-26}Registro como persona socia/usuaria mediante firma digital

- Funcionalidad: El usuario anónimo podrá solicitar el darse de alta
  como persona socia/usuaria del CPA de su localidad, a través del
  aplicativo CPA virtual, desde la app móvil, cumplimentado el
  formulario de alta con sus datos personales, y que deberá firmar
  digitalmente. Tras la firma, la solicitud será enviada al
  administrador del CPA que corresponda para su validación, la cual una
  vez verificada con la presencia de la persona socia/usuaria en el CPA
  que solicita, será dada de alta mediante un código de acceso y clave
  que le permitirá acceder a la parte privada del aplicativo CPA Virtual
  para el CPA solicitado, ya como persona socia/usuaria.

- Perfil usuario: Usuario anónimo.

- Detalles: El usuario podrá solicitar el darse de alta como persona
  socia/usuaria del CPA de su localidad, a través del aplicativo CPA
  virtual, desde la app móvil, cumplimentado el formulario de alta con
  sus datos personales, y que deberá firmar digitalmente. Tras la firma,
  la solicitud será enviada al administrador del CPA que corresponda
  para su validación, la cual una vez verificada con la presencia de la
  persona socia/usuaria en el CPA que solicita, será dada de alta
  mediante un código de acceso y clave que le permitirá acceder a la
  parte privada del aplicativo CPA Virtual para el CPA solicitado, ya
  como persona socia/usuaria. Desde ese momento el usuario, ya como
  persona socia/usuaria, podrá acceder e interactuar, iniciando la
  sesión desde la zona privada de CPA Virtual, con el CPA de su
  localidad, desde su espacio 'Mi CPA'. Desde el espacio 'Mi CPA', una
  vez realizada la autenticación, el nuevo usuario podrá acceder a una
  visión personalizada, dentro de las siguientes funcionalidades de CPA
  Virtual:

  - Gestionar inscripciones a talleres y actividades.
  - Gestionar citas previas a servicios.
  - Consultar su agenda.
  - Ver/descargar tarjeta identificativa.
  - Comunicación con profesionales.
  - Gestionar sus trámites.
  - Certámenes, grupos, foros, etc.

- Ejemplo: El usuario Juan Luis Cárdenas solicita el alta como persona
  socia/usuaria para el CPA de Triana a través del CPA virtual,
  cumplimentado la solicitud y firmándola digitalmente.

### []{#anchor-27}Evaluaciones Taller

Las Evaluaciones de talleres, permitirá al usuario con perfil persona
socia/usuaria, antes de que finalice o ya finallizado el taller de un
CPA, evaluarla con valores de 0 a 5 estrellas. En el caso de que el
taller se haya impartido en diferentes centros CPA, el resultado de la
evaluación deberá ser la media de todas ellas.

#### []{#anchor-28}Evaluaciones Taller 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado, para un determinado CPA, de evaluar el taller seleccionado
  en el que se haya inscrito, valorando la misma de 0 a 5 estrellas.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario será el encargado, mediante la funcionalidad
  evaluar taller, para un determinado CPA, evaluar el taller al que se
  haya inscrito y que haya sido seleccionado, pudiendo valorarse de 0 a
  5 estrellas. En el caso de haberse impartido el taller en diferentes
  centros CPA, el resultado de la evaluación será la media de todas
  ellas.
- Ejemplo: La persona socia/usuaria Juan Luis Cárdenas desea evaluar
  para el centro de 'Triana', el taller 'baile flamenco grupo1' con
  '\*\*\*'.

### []{#anchor-29}Evaluaciones Actividad

Las Evaluaciones de actividad, permitirán al usuario con perfil persona
socia/usuaria, antes de que finalice o una vez finalizada la actividad
de un CPA, evaluarla con valores de 0 a 5 estrellas. En el caso de que
la actividad se haya impartido en diferentes centros CPA, el resultado
de la evaluación deberá ser la media de todas ellas.

#### []{#anchor-30}Evaluaciones Actividad

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado, para un determinado CPA, de evaluar la actividad
  seleccionada, valorando la misma de 0 a 5 estrellas.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario será el encargado, mediante la funcionalidad
  evaluar una actividad, para un determinado CPA, que haya sido
  seleccionada, valorándola de 0 a 5 estrellas. En el caso de haberse
  impartido la actividad en diferentes centros CPA, el resultado de la
  evaluación será la media de todas ellas.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea evaluar para el centro de 'Triana', la programación de
  la actividad 'certamen villancicos grupo1' con '\*\*\*'.

### []{#anchor-31}Consulta Contenidos zona pública 

La Consulta de Contenidos de la zona pública de CPA Virtual permitirá a
cualquier usuario, consultar los distintos contenidos informativos
publicados (noticias, certámenes, concursos, encuentros, recitales,
exposiciones, representaciones, actuaciones formativas\...)

#### []{#anchor-32}Consulta Lista Contenidos zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá consultar la relación de contenido
  informativo público, para el cual no necesitará autenticarse.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, mediante la funcionalidad
  consulta lista contenidos, desde la zona pública del aplicativo CPA
  Virtual, podrá acceder a los distintos contenidos informativos
  ofrecidos, de ámbito de publicación 'Público'.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta desde la zona pública
  las noticias informativas.

#### []{#anchor-33}Consulta Contenidos zona pública

- Funcionalidad: Cualquier usuario anónimo podrá consultar el detalle
  del contenido informativo seleccionado previamente en la zona pública
  del aplicativo CPA Virtual.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, tras haber seleccionado
  previamente un contenido informativo en la zona pública de CPA
  Virtual, consulta el detalle del contenido.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta desde la zona pública
  el detalle de una noticia informativa, seleccionada previamente.

### []{#anchor-34}Retransmisión Contenidos zona pública 

La Retransmisión de Contenidos de la zona pública de CPA Virtual,
permitirá al usuario, ver la retransmisión en formato digital
(vídeos,..) los distintos contenidos informativos publicados (noticias,
certámenes, concursos, encuentros, recitales, exposiciones,
representaciones, actuaciones formativas...), que se encuentren
disponibles en el aplicativo CPA Virtual.

#### []{#anchor-35}Retransmisión Contenidos zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá ver la retransmisión de aquellos
  contenidos publicados y presentados en formato digital (vídeos,...),
  que se encuentren disponibles en el aplicativo CPA Virtual.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá ver la retransmisión de aquellos
  contenidos publicados y presentados en formato digital (vídeos,...),
  que se encuentren disponibles en el aplicativo CPA Virtual. Para ello,
  se contará con una agenda, desde donde se mostrarán en los días del
  calendario que apliquen, los enlaces a las retransmisiones de los
  contenidos públicos activos.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta desde la zona pública
  el vídeo informativo sobre el taller 'baile flamenco' que el CPA
  'Triana' ofrece en el mes de junio.

### []{#anchor-36}A la carta 

El espacio 'A la carta' definido dentro de la sección 'Directo a',
accesible desde la zona pública de CPA Virtual, desde dónde cualquier
usuario anónimo podrá acceder a los distintos de recursos multimedia
(talleres, actividades u otros recursos) de los CPAs. Así como poder
visualizar las retransmisiones de talleres y actividades que se hayan
incluido en dicha sección. Y desde la zona privada, desde dónde las
personas socias/usuarias podrán acceder al mismo contenido, pero
correspondientes al CPA o Provincia de dicho CPA, al que pertenezcan.

#### []{#anchor-37}A la carta zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá acceder al contenido definido en el
  espacio 'A la carta' dentro de la sección 'Directo a'.
- Perfil usuario: Persona socia/usuaria
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá acceder al contenido definido en el
  espacio 'A la carta' dentro de la sección 'Directo a'. Aplicando el
  filtro 'taller', 'actividad' u 'otros recursos', podrá acceder a las
  retransmisiones del contenido seleccionado.
- Ejemplo: El usuario anónimo Juan Luis Cárdenas, consulta desde la zona
  pública la retransmisión del taller 'baile flamenco' del día
  09-agosto-2025 del centro 'Triana'.

#### []{#anchor-38}A la carta zona privada

- Funcionalidad: La persona socia/usuaria, desde la zona privada del
  aplicativo CPA Virtual, podrá acceder al contenido definido en el
  espacio 'A la carta' dentro de la sección 'Directo a' correspondientes
  al CPA o Provincia de dicho CPA, al que pertenezcan.
- Perfil usuario: Usuario anónimo.
- Detalles: La persona socia/usuaria, desde la zona privada del
  aplicativo CPA Virtual, podrá acceder al contenido definido en el
  espacio 'A la carta' dentro de la sección 'Directo a'. Aplicando el
  filtro 'taller', 'actividad' u 'otros recursos', podrá acceder a las
  retransmisiones del contenido seleccionado al que tenga acceso.
- Ejemplo: El usuario anónimo Juan Luis Cárdenas, consulta desde la zona
  pública la retransmisión del taller 'baile flamenco' del día
  09-agosto-2025 del centro 'Triana'.

### []{#anchor-39}Agenda zona pública 

La Agenda de la zona pública de CPA Virtual permitirá al usuario
anónimo, consultar la agenda con los distintos talleres, actividades y
citas ofertados para la CPA Virtual. Se le ofrecerá al usuario anónimo
filtrar la búsqueda por código postal, localidad o nombre del CPA, con
el fin de que pueda seleccionar uno y que toda la información mostrada
corresponda al CPA seleccionado.

#### []{#anchor-40}Agenda zona pública

- Funcionalidad: El usuario anónimo podrá consultar los talleres,
  actividades y citas previas ofertadas por el CPA que previamente haya
  seleccionado. Para ello, contará con una agenda, desde la cual,
  seleccionando un determinado día, le mostrará la agenda horaria del
  día, con la relación de sesiones de actividades y talleres existentes
  para el día indicado, así como las citas previas de servicios
  ofrecidos a las personas anónimas.
- Perfil usuario: Usuario anónimo.
- Detalles: El usuario anónimo podrá consultar los talleres, actividades
  y citas ofertados por el CPA que previamente haya seleccionado. Para
  ello, contará con una agenda, desde la cual, seleccionando un
  determinado día, le mostrará la agenda horaria del día, con la
  relación de sesiones de actividades y talleres existentes para el día
  indicado, así como las citas previas de servicios ofrecidos a las
  personas anónimas..
- Ejemplo: El usuario anónimo desea consultar la agenda del día
  '01/02/2025' para el centro 'Triana'.

### []{#anchor-41}Consulta Talleres zona pública 

La Consulta de Talleres de la zona pública de CPA Virtual permitirá al
usuario anónimo, consultar las distintos talleres ofertados para la CPA
Virtual. Se le ofrecerá al usuario anónimo filtrar la búsqueda por
código postal, localidad o nombre del CPA, con el fin de que pueda
seleccionar uno y que toda la información mostrada corresponda al CPA
seleccionado.

#### []{#anchor-42}Consulta Listado Centros Zona Pública

- Funcionalidad: Cualquier usuario anónimo será el encargado de escoger
  los criterios de búsqueda y consultar el listado de CPA que ofrecen
  talleres ofertados en los distintos CPAs, en base a los filtros código
  postal, localidad o nombre del centro.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, mediante la funcionalidad consulta listado
  centros zona pública, podrá escoger los filtros de búsqueda y
  consultar el listado de los CPA que ofertan talleres en los distintos
  CPAs. El usuario tendrá la posibilidad de poder filtrar la búsqueda
  por el centro que considere, en base a los filtros código postal,
  localidad o nombre del centro.
- Ejemplo: El usuario Juan Luis Cárdenas, busca y consulta la relación
  de CPA que ofertan categorías de talleres por el código postal
  '45001'.

#### []{#anchor-43}Consulta Listado Categorías Zona Pública

- Funcionalidad: Cualquier usuario anónimo será el encargado de escoger
  los criterios de búsqueda y consultar el listado de categorías de los
  talleres ofertados, en base a un determinado CPA, que se haya
  seleccionado previamente.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario, desde la zona pública del aplicativo CPA
  Virtual, mediante la funcionalidad consulta listado categorías zona
  pública, podrá escoger los filtros de búsqueda y consultar el listado
  de categorías de talleres ofertados a los distintos CPAs, en base al
  CPA seleccionado previamente. El usuario anónimo tendrá la posibilidad
  de poder filtrar la búsqueda por el centro que considere.
- Ejemplo: El usuario Juan Luis Cárdenas, busca y consulta la relación
  de categorías ofertados por el CPA 'Triana'.

#### []{#anchor-44}Consulta Listado Sesiones Taller zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá consultar el listado de sesiones del
  taller del CPA y categoría seleccionados previamente.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá visualizar el listado de sesiones del
  taller del CPA y categoría seleccionados previamente.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta el listado de las
  sesiones del taller 'iniciación baile flamenco' ofertado por el CPA
  'Triana', de la categoría 'Baile'.

### []{#anchor-45}Consulta Actividades zona pública 

La Consulta de actividades de la zona pública de CPA Virtual permitirá
al usuario, consultar las distintas actividades ofertadas para la CPA
Virtual. Se le ofrecerá al usuario anónimo filtrar la búsqueda por
código postal, localidad o nombre del CPA, con el fin de que pueda
seleccionar uno y que toda la información mostrada corresponda al CPA
seleccionado.

#### []{#anchor-46}Consulta Listado Centros Zona Pública

- Funcionalidad: Cualquier usuario anónimo será el encargado de escoger
  los criterios de búsqueda y consultar el listado de CPA que ofrecen
  actividades ofertados en los distintos CPAs, en base a los filtros
  código postal, localidad o nombre del centro.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, mediante la funcionalidad consulta listado
  centros zona pública, podrá escoger los filtros de búsqueda y
  consultar el listado de los CPA que ofertan actividades en los
  distintos CPAs. El usuario tendrá la posibilidad de poder filtrar la
  búsqueda por el centro que considere, en base a los filtros código
  postal, localidad o nombre del centro.
- Ejemplo: El usuario Juan Luis Cárdenas, busca y consulta la relación
  de CPA que ofertan actividades por el código postal '45001'.

#### []{#anchor-47}Consulta Listado Actividades zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá consultar el listado de categorías de
  actividades ofertados para un determinado CPA, en base al CPA y
  categoría seleccionados previamente.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá visualizar el listado de categorías de
  actividades en base al CPA y categoría seleccionados previamente.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta el listado de las
  actividades ofertadas por el CPA 'Triana', de la categoría 'Baile'.

#### []{#anchor-48}Consulta Listado Sesiones Actividad zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá consultar el listado de sesiones en base
  al CPA y categoría de actividad seleccionados previamente.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá visualizar el listado de sesiones de la
  actividad del CPA y categoría seleccionados previamente.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta el listado de las
  sesiones de la actividad 'iniciación baile flamenco' ofertado por el
  CPA 'Triana', de la categoría 'Baile'.

### []{#anchor-49}Consulta Servicios Zona Pública 

La Consulta de servicios de la zona pública de CPA Virtual permitirá al
usuario, consultar los distintos servicios ofertados para la CPA
Virtual. Se le ofrecerá al usuario anónimo filtrar la búsqueda por
código postal, localidad o nombre del CPA, con el fin de que pueda
seleccionar uno y que toda la información mostrada corresponda al CPA
seleccionado.

#### []{#anchor-50}Consulta Listado Centros Zona Pública

- Funcionalidad: Cualquier usuario anónimo será el encargado de escoger
  los criterios de búsqueda y consultar el listado de CPA que ofrecen
  servicios ofertados en los distintos CPAs, en base a los filtros
  código postal, localidad o nombre del centro.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, mediante la funcionalidad consulta listado
  centros zona pública, podrá escoger los filtros de búsqueda y
  consultar el listado de los CPA que ofertan servicios en los distintos
  CPAs. El usuario tendrá la posibilidad de poder filtrar la búsqueda
  por el centro que considere, en base a los filtros código postal,
  localidad o nombre del centro.
- Ejemplo: El usuario Juan Luis Cárdenas, busca y consulta la relación
  de CPA que ofertan servicios por el código postal '45001'.

#### []{#anchor-51}Consulta Listado Servicios zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá consultar el listado de categorías de
  servicios ofertados para un determinado CPA, en base al CPA y
  categoría seleccionados previamente.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá visualizar el listado de categorías de
  servicios en base al CPA y categoría seleccionados previamente.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta el listado de las
  actividades ofertadas por el CPA 'Triana', de la categoría 'Baile'.

#### []{#anchor-52}Consulta Listado Citas Previas zona pública

- Funcionalidad: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá consultar el listado de citas previas en
  base al CPA y categoría de servicio seleccionados previamente.
- Perfil usuario: Usuario anónimo.
- Detalles: Cualquier usuario anónimo, desde la zona pública del
  aplicativo CPA Virtual, podrá visualizar el listado de citas previas
  del CPA y categoría de servicio seleccionados previamente.
- Ejemplo: El usuario Juan Luis Cárdenas, consulta el listado de las
  citas previas del servicio 'Peluquería centro Triana' ofertado por el
  CPA 'Triana', de la categoría 'Peluquería'.

### []{#anchor-53}Gestión Mi CPA

La gestión de 'Mi CPA' permitirá al usuario con perfil persona
socia/usuaria tener una visión personalizada de su agenda, sus
inscripciones a talleres, actividades y/o servicios, descarga su
tarjeta, modifcar sus datos, solicitar la baja o ver un histórico de sus
participaciones en actividades/talleres, así como de sus conocimientos y
habilidades.

#### []{#anchor-54}Acceso Mi CPA

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  acceder a la parte privada de CPA Virtual, mediante este acceso a la
  autenticación, mediante código de acceso y clave.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá acceder a
  la parte privada de CPA Virtual, mediante este acceso a la
  autenticación, mediante código de acceso y clave.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea acceder a la parte privada, mediante la autenticación
  previa.

#### []{#anchor-55}Mis Datos

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  consultar sus datos, tanto personales, como los correspondientes al
  CPA al que pertenece. Igualmente podrá actualizar los mismos.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá consultar
  sus datos, tanto personales, como los correspondientes al CPA al que
  pertenece. Igualmente podrá actualizar los mismos.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea consultar sus datos personales y el centro al que
  pertenece.

#### []{#anchor-56}Mi Agenda

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  consultar los talleres, actividades y citas previas agendadas en su
  día a día. Para ello, contará con una agenda, desde la cual,
  seleccionando un determinado día, le mostrará la agenda horaria del
  día, con la relación de sesiones de actividades y talleres a los que
  se haya inscrito, así como a citas previas de servicios para ese día.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá consultar
  las sesiones de talleres, actividades a los que esté inscrito, así
  como a citas previas de servicios agendados en su día a día. Para
  ello, contará con una agenda, desde la cual, seleccionando un
  determinado día, se le mostrará la agenda horaria del día, con la
  relación de servicios mencionados.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea consultar su agenda del día '01/02/2025'.

#### []{#anchor-57}Mis inscripciones

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  consultar las solicitudes de inscripciones a los talleres, actividades
  y servicios, pudiendo saber en todo momento en que estado se
  encuentran. Y en el caso de inscripciones a talleres o actividades
  retransmitidas por streaming, acceder al enlace que le permita ver la
  retransmisión del evento que corresponda.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá consultar
  las solicitudes de inscripciones a los talleres, actividades y citas
  previas de servicios, pudiendo saber en todo momento en que estado se
  encuentran. Y en el caso de inscripciones a talleres o actividades
  retransmitidas por streaming, acceder al enlace que le permita ver la
  retransmisión del evento que corresponda.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea ver el estado de la inscripción al taller 'iniciacion
  baile flamenco' del CPA 'Triana'.

#### []{#anchor-58}Mi participación

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  consultar las participaciones (como profesional de tipo personal
  'CMD') en los talleres y actividades en los que haya participado.
  Igualmente podrá definir sus conocimientos y habilidades.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá consultar
  las participaciones (como profesional de tipo personal 'CMD') en los
  talleres y actividades en los que haya participado. Igualmente podrá
  definir sus conocimientos y habilidades.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea ver el histórico de sus participaciones como
  profesional de tipo personal 'CMD'.

#### []{#anchor-59}Descarga/Consulta tarjeta identificativa

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  consultar o descargarse su tarjeta identificativa.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá consultar
  o descargarse su tarjeta identificativa.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea visualizar su tarjeta identificativa.

### []{#anchor-60}Gestión Mis Trámites Personas socias/usuarias

La gestión de 'Mis Trámites' permitirá al usuario con perfil persona
socia/usuaria tener una visión personalizada de sus trámites pendientes,
y poder gestionar los mismos desde ella.

#### []{#anchor-61}Baja Voluntaria

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  realizar una solicitud de baja voluntaria del CPA al que corresponda,
  mediante el formulario correspondiente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá realizar
  una solicitud de baja voluntaria del CPA al que corresponda, mediante
  el formulario correspondiente. Para ello deberá reflejar el motivo por
  el cual solicita la baja del CPA al que pertenece. La solicitud no
  será efectiva hasta que no sea validada y ejecuta por el usuario
  administrador del CPA.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea darse de baja voluntariamente del CPA 'Triana'.

### []{#anchor-62}Gestión Comunicación Personas socias/usuarias

La gestión de la comunicación permitirá al usuario con perfil persona
socia/usuaria enviar y recibir comunicaciones de profesionales y/o
personas socias/usuarias de su CPA. Así como recibir notificaciones con
información de interés del personal de su CPA.

#### []{#anchor-63}Notificaciones 

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  recibir notificaciones con información de interés de su CPA, tanto con
  contenido personal, como contenido de interés para todas las personas
  socias del centro.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá recibir
  notificaciones con información de interés de su CPA, tanto con
  contenido personal, como contenido de interés para todas las personas
  socias del centro.
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, recibe una notificación de su monitor del taller de
  'baile flamenco'.

#### []{#anchor-64}Comunicación con Profesionales 

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  enviar y recibir comunicaciones con profesionales de su CPA.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá recibir
  comunicaciones emitidas por profesionales de su CPA a través del
  sistema digital que corresponda (chat público/privado, correo
  electrónico\...).
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, recibe una comunicación de su monitor del taller de
  'baile flamenco'.

#### []{#anchor-65}Comunicación con Personas socias/usuarias 

- Funcionalidad: El usuario con perfil persona socia/usuaria podrá
  enviar y recibir comunicaciones de otras personas socias de su CPA.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria podrá enviar y
  recibir comunicaciones de otras personas socias de su CPA a través del
  sistema digital que corresponda (chat público/privado, correo
  electrónico\...)..
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, envía una comunicación al usuario Pedro Santos con
  perfil persona socia/usuaria, ambos del centro 'Triana'.

### []{#anchor-66}Gestión Talleres Personas socias/usuarias

La gestión de los talleres permitirá al usuario con perfil persona
socia/usuaria gestionar para el CPA al que pertenezca y que seleccione
previamente, los distintos talleres ofertados para el CPA, desde dónde
podrá consultar, inscribirse, cancelar la inscripción y ver las
retransmisiones en el caso de sesiones streaming.

#### []{#anchor-67}Consulta Listado Categorías Talleres 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las categorías del tipo talleres, que contengan talleres ofertados
  en los CPAs a los que pertenece el usuario.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las categorías del tipo talleres, que contengan talleres ofertados
  en los CPAs a los que pertenece el usuario.
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, consulta la lista de categorías de talleres,
  correspondientes al CPA 'Triana'.

#### []{#anchor-68}Consulta Listado Talleres 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de los talleres ofertados por el CPA al que pertenece y que
  corresponden a la categoría seleccionada previamente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de los talleres ofertados por el CPA al que pertenece y que
  corresponden a la categoría seleccionada previamente.
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, consulta la lista de talleres, correspondientes al
  centro CPA 'Triana' y categoría 'Baile'.

#### []{#anchor-69}Inscripción Talleres 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la inscripción al taller del CPA que haya
  seleccionado previamente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la inscripción al taller del CPA que haya
  seleccionado previamente. Como resultado de la gestión, la solicitud
  quedará en estado 'sin validar', a la espera que el usuario con perfil
  administrador, la valide, aceptando o rechazando la misma. La
  inscripción al taller solo podrá ser presencial en el caso de talleres
  que correspondan al centro al que pertenece la persona socia/usuaria.
  En el resto de los casos, deberá ser En Línea.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea inscribirse para el centro de 'Triana' al taller
  'iniciació baile flamenco'.

#### []{#anchor-70}Cancelación Inscripciones Talleres 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la cancelación de la inscripción al taller del
  CPA que haya seleccionado previamente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la cancelación de la inscripción all taller del
  CPA que haya seleccionado previamente. Deberá borrarse la inscripción.
  Si la inscripción de la persona solicitante estuviera en estado
  'Admitida', deberá actualizarse el valor de las plazas disponibles en
  la programación del taller del CPA que aplique, sumándole 1.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea cancelar la inscripción para el centro de 'Triana' al
  taller 'baile flamenco'.

#### []{#anchor-71}Retransmisión Talleres 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de poder ver la retransmisión de la sesión En Línea de un
  determinado taller al que se haya inscrito previamente y al que se le
  haya admitido, en aquellos talleres que ofrezcan esa posibilidad.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de poder ver la retransmisión de la sesión En Línea de un
  determinado taller al que se haya inscrito previamente y al que se le
  haya admitido, en aquellos talleres que ofrezcan esa posibilidad. Para
  ello, una vez su solicitud de inscripción haya sido admitida, se le
  presentará en pantalla el enlace que le permitirá acceder desde CPA
  Virtual a la retransmisión de la sesión del taller.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea ver la retransmisión de la sesión del día '01/01/2025
  9h' del taller 'baile flamenco grupo1' del centro de 'Triana'.

### []{#anchor-72}Gestión Actividades Personas socias/usuarias

La gestión de las actividades permitirá al usuario con perfil persona
socia/usuaria gestionar para el CPA al que pertenezca y que seleccione
previamente, las distintas actividades ofertadas para el CPA, desde
dónde podrá consultar, inscribirse, cancelar la inscripción y ver las
retransmisiones en el caso de sesiones streaming.

#### []{#anchor-73}Consulta Listado Categorías Actividades 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las categorías del tipo actividades, que contengan actividades
  ofertadas en los CPAs a los que pertenece el usuario.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las categorías del tipo actividades, que contengan actividades
  ofertadas en los CPAs a los que pertenece el usuario.
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, consulta la lista de categorías de actividades,
  correspondientes al CPA 'Triana'.

#### []{#anchor-74}Consulta Listado Actividades 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las actividades ofertadas por el CPA al que pertenece y que
  corresponden a la categoría seleccionada previamente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las actividades ofertadas por el CPA al que pertenece y que
  corresponden a la categoría seleccionada previamente.
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, consulta la lista de actividades, correspondientes al
  centro CPA 'Triana' y categoría 'Baile'.

#### []{#anchor-75}Inscripción Actividades 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la inscripción a la actividad del CPA que haya
  seleccionado previamente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la inscripción a la actividad del CPA que haya
  seleccionado previamente. Como resultado de la gestión, la solicitud
  quedará en estado 'sin validar', a la espera que el usuario con perfil
  administrador, la valide, aceptando o rechazando la misma. La
  inscripción a la actividad solo podrá ser presencial en el caso de
  actividades que correspondan al centro al que pertenece la persona
  socia/usuaria. En el resto de los casos, deberá ser online.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea inscribirse para el centro de 'Triana' a la actividades
  'iniciación baile flamenco'.

#### []{#anchor-76}Cancelación Inscripciones Actividades 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la cancelación de la inscripción a la actividad
  del CPA que haya seleccionado previamente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de solicitar la cancelación de la inscripción a la actividad
  del CPA que haya seleccionado previamente. Deberá borrarse la
  inscripción. Si la inscripción de la persona solicitante estuviera en
  estado 'Admitida', deberá actualizarse el valor de las plazas
  disponibles en la actividad del CPA que aplique, sumándole 1.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea cancelar la inscripción para el centro de 'Triana' a la
  actividad 'baile flamenco'.

#### []{#anchor-77}Retransmisión Actividades

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de poder ver la retransmisión de la sesión online de una
  determinada actividad al que se haya inscrito previamente y al que se
  le haya admitido, en aquellos talleres que ofrezcan esa posibilidad.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de poder ver la retransmisión de la sesión online de una
  determinada actividad a la que se haya inscrito previamente y al que
  se le haya admitido, en aquellas actividades que ofrezcan esa
  posibilidad. Para ello, una vez su solicitud de inscripción haya sido
  admitida, se le presentará en pantalla el enlace que le permitirá
  acceder desde CPA Virtual a la retransmisión de la sesión de la
  actividad.
- Ejemplo: El usuario con perfil persona socia/usuaria Juan Luis
  Cárdenas desea ver la retransmisión de la sesión del día '01/01/2025
  9h' de la actividad 'baile flamenco grupo1' del centro de 'Triana'.

### []{#anchor-78}Gestión Servicios Personas socias/usuarias

La gestión de los servicios permitirá al usuario con perfil persona
socia/usuaria gestionar para el centro que seleccione (bien al que
pertenezca o bien a otro CPA), los distintos servicios definidos, desde
dónde podrá consultar, inscribirse y cancelar la inscripción.

#### []{#anchor-79}Consulta Listado Categorías Servicios 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las categorías del tipo servicios, que contengan servicios
  ofertados en los CPAs a los que pertenece el usuario.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de las categorías del tipo servicios, que contengan servicios
  ofertados en los CPAs a los que pertenece el usuario.
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, consulta la lista de categorías de servicios,
  correspondientes al CPA 'Triana'.

#### []{#anchor-80}Consulta Listado Servicios 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de los servicios ofrecidos al CPA y categoría seleccionados
  previamente.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de definir los criterios de búsqueda y consultar el listado
  de los servicios ofrecidos al CPA seleccionado previamente. Solo se
  presentarán los servicios que cumplan que su estado sea 'Abierta' o
  'Cerrada'.
- Ejemplo: El usuario Juan Luis Cárdenas con perfil persona
  socia/usuaria, consulta la lista de servicios, correspondientes a la
  categoría 'Peluquería' y CPA 'Triana'.

#### []{#anchor-81}Consultar Agenda Cita Previa

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de poder consultar la agenda de citas previas para el CPA y
  servicio del tipo 'cita previa' previamente seleccionados.
- Perfil usuario: Usuario persona socia/usuaria.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de poder consultar la agenda de citas previas para el CPA y
  servicio del tipo 'cita previa' previamente seleccionados.
- Ejemplo: El usuario profesional con perfil administrador Juan Luis
  Cárdenas desea consultar el detalle del servicio 'comedor' del centro
  de 'Triana'.

#### []{#anchor-82}Alta Cita 

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de cumplimentar los datos de alta de una cita para el día de
  la agenda de citas previas del servicio y el centro previamente
  seleccionados. En los datos a cumplimentar se detallarán sus datos
  personales, así como el día y la hora.
- Perfil usuario: Usuario Persona socia.
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de cumplimentar los datos de alta de una cita para el día de
  la agenda de la cita previa del servicio y CPA previamente
  seleccionados. En los datos a cumplimentar se detallarán sus datos
  personales del solicitante, así como el día y la hora. Se le
  presentará previamente un calendario y al seleccionar un día, se le
  mostrarán las horas disponibles del día, dentro del horario definido
  para esa cita previa del servicio del CPA.
- Ejemplo: El usuario Juan Luis Cárdenas desea dar de alta una cita para
  la cita previa de servicio del catálogo 'Peluquería' del centro
  'Triana', el día '01/01/2025' a las '9h'.

#### []{#anchor-83}Cancelación Cita

- Funcionalidad: El usuario con perfil persona socia/usuaria será el
  encargado de cancelar una cita para la cita previa del servicio y
  centro seleccionados previamente.
- Perfil usuario: Usuario persona socia
- Detalles: El usuario con perfil persona socia/usuaria será el
  encargado de cancelar una cita para la cita previa del servicio y
  centro seleccionados previamente.
- Ejemplo: El usuario profesional con perfil administrador Juan Luis
  Cárdenas desea dar de baja una cita para la cita previa del servicio
  del catálogo 'Peluquería', en el centro 'Triana', el día '01/01/2025'
  a las '9h'.

### []{#anchor-84}Formación 

Formación mediante vídeos tutoriales y manuales de usuario, cuyo
contenidos sean la forma de trabajar e interactuar con el aplicativo CPA
Virtual, para cada uno de los perfiles.

#### []{#anchor-85}Formación 

- Funcionalidad: Formación mediante manuales de usuario y vídeos
  tutoriales, con el fin de que puedan ser utilizados para la formación
  de los distintos perfiles que interactúen con el aplicativo CPA
  Virtual.
- Perfil usuario: Todos los perfiles de usuario.
- Detalles: Se crearán manuales de usuario y videos tutoriales, con el
  fin de que puedan ser utilizados para la formación de los distintos
  perfiles que interactúen con el aplicativo CPA Virtual.
- Ejemplo: Manual de usuario para el perfil 'Persona Profesional'.

### 

### 

****Confidencialidad del Documento****

Propiedad de Getronics.

Este documento en su totalidad está sujeto a los términos del Acuerdo
Mutuo de Confidencialidad y NDA.

Esta propuesta es comercial confidencial y contiene información
confidencial y de propiedad de Getronics específicamente para su
evaluación por la Junta de Andalucía, entendiéndose que no debe ser
revelada a terceros salvo autorización expresa de Getronics. Esta
propuesta seguirá siendo propiedad de Getronics en todo momento.
