# Análisis de Requisitos  
Funcionalidad: Autenticación CPA Virtual  
ID Historia de usuario: HU-CPA-0001-AUTENTICACION_CPA-VIRTUAL
---  
## 1. Descripción General
Enunciado:
Como usuario que debe logarse y tener cuenta (usuario y clave), para poder acceder a la parte privada del aplicativo CPA Virtual.
Funcionalidad:
El acceso se realizará desde la zona pública del aplicativo CPA Virtual, a través del menú superior ('Mi CPA'), que presentará el formulario de login con usuario y clave.
Una vez verificado que el usuario tiene cuenta, se identificará el CPA al que pertenece y su perfil, y se mostrarán en pantalla las opciones de menú habilitadas según el perfil.
---  
## 2. Requisitos Funcionales
RF1. Presentación del formulario
El sistema debe presentar un formulario de acceso con los siguientes campos y botones:
- Campo 'Nombre de usuario': texto, editable, obligatorio.
- Campo 'Clave': texto, editable, obligatorio.
- Botón 'Iniciar Sesión'.
- Botón '¿Olvidó su contraseña?'.
RF2. Autenticación
El sistema debe verificar, mediante el formulario, que el usuario y clave introducidos existen en 'Usuarios', 'TiposUsuarios', 'PersonasSocias' en Drupal, filtrando solo usuario tipo 'Persona Socia/usuaria'.
RF3. Acceso exitoso
Si la verificación es exitosa:
- El sistema obtiene los datos personales, centro y perfiles del usuario mediante operaciones en Drupal.
- Se muestra un menú personalizado en la parte privada ('Escritorio CPA Virtual') según los perfiles y centros asignados.
- Se accede al 'Formulario Acceso Parte Privada' de la historia HU-CPA-0051.
RF4. Acceso denegado
Si usuario/clave no son válidos:
- Se muestra mensaje: 'Usuario o contraseña no reconocidos. ¿Olvidaste tu contraseña?'
RF5. Recuperación de contraseña
Al pulsar '¿Olvidó su contraseña?', el sistema debe mostrar una ventana para ingresar usuario/correo; tras enviar, el usuario recibirá un correo para restablecer la clave.  
Operaciones:
- 'obtenerCódigoUsuarioPorEmail' y 'actualizarClaveAccesoUsuario' sobre el tipo de contenido 'Usuarios' (Drupal).
---  
## 3. Requisitos No Funcionales
- Seguridad: Transmisión cifrada de credenciales.
- Usabilidad: Campos obligatorios y mensaje claro en caso de error.
- Interfaz: Formulario intuitivo y disponible desde la zona pública del CPA Virtual.
- Integración: Consultas y operaciones contra el repositorio Drupal usando las entidades indicadas.
---  
## 4. Casos de Uso
Actor: Usuario CPA  
Caso de uso: Autenticación en el CPA Virtual
Flujo principal:
1. El usuario accede al formulario desde 'Mi CPA'.
2. Completa usuario y clave; pulsa 'Iniciar Sesión'.
3. El sistema verifica las credenciales.
  - Si son válidas: obtiene datos y muestra menú privado, permite operar según perfil y centro.
  - Si no son válidas: muestra mensaje de error.
4. Si pulsa '¿Olvidó su contraseña?': sistema gestiona el envío y actualización de clave vía email.
---  
## 5. Criterios de Aceptación
1. Formulario Autenticación: Debe validar usuario autorizado.
2. Nombre de usuario: Campo texto, editable, obligatorio.
3. Clave: Campo texto, editable, obligatorio.
4. Botón Iniciar Sesión: Verifica existencia en Drupal; obtiene datos y menú personalizado si éxito, muestra error si falla.
5. Botón ¿Olvidó su contraseña?: Gestiona recuperación y actualización vía correo electrónico.
---  
## 6. Consideraciones Técnicas y de Negocio
- Operaciones integradas con Drupal para autenticación y recuperación de clave.
- Gestión de perfiles y centros según datos del usuario autenticado.
- Cumplimiento de la normativa de protección de datos.
---  
## 7. Dependencias
- Repositorio Drupal y sus entidades: Usuarios, Centros, Perfiles, etc.
- HU-CPA-0051 (Acceso Parte Privada CPA Virtual).
---  
## 8. Glosario
- CPA: Centro/Perfil de Aplicación Virtual.
- Usuario: Persona socia/usuaria autenticada en la aplicación.
- Drupal: Plataforma de gestión de contenidos utilizada como backend.