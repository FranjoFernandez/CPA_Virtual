### Autenticación Usuarios

#### User Story Narrative
Como usuario de CPA Virtual, quiero autenticarme en la plataforma para acceder a mis funcionalidades reservadas.

#### Functional Description
El sistema debe permitir que los usuarios se autentiquen utilizando su nombre de usuario y contraseña. Si las credenciales son correctas, se les debe permitir el acceso. Si no, se debe mostrar un mensaje de error.

#### Acceptance Criteria Scenarios
1. **Credenciales Válidas**: Los usuarios deben poder iniciar sesión con credenciales válidas.
2. **Credenciales Inválidas**: El sistema debe mostrar un mensaje de error si las credenciales son incorrectas.
3. **Bloqueo de Cuenta**: Después de 5 intentos fallidos, la cuenta del usuario debe ser bloqueada.
4. **Recuperación de Contraseña**: Los usuarios deben poder recuperar su contraseña a través de un enlace enviado a su correo electrónico.
5. **Tiempo de Sesión**: La sesión del usuario debe expirar después de 30 minutos de inactividad.

#### Functional Requirements (RF-001 to RF-013)
- **RF-001**: El sistema debe permitir a los usuarios registrarse con un correo electrónico y contraseña.
- **RF-002**: El sistema debe permitir el inicio de sesión con correo electrónico y contraseña.
- **RF-003**: El sistema debe mostrar un mensaje de error en caso de credenciales incorrectas.
- **RF-004**: El sistema debe permitir a los usuarios recuperar su contraseña.
- **RF-005**: El sistema debe definir un límite de intentos fallidos de inicio de sesión.
- **RF-006**: El sistema debe permitir que los usuarios cierren sesión.
- **RF-007**: El sistema debe permitir que los administradores bloqueen cuentas de usuario.
- **RF-008**: El sistema debe almacenar las contraseñas de manera segura.
- **RF-009**: El sistema debe registrar los intentos de inicio de sesión.
- **RF-010**: El sistema debe ajustar el tiempo de sesión de acuerdo con la política de seguridad.
- **RF-011**: Los emails de recuperación de contraseña deben incluir un enlace seguro.
- **RF-012**: El sistema debe proporcionar una opción de autenticación de dos factores.
- **RF-013**: El sistema debe actualizar el estado de la cuenta después de un intento fallido.

#### Non-Functional Requirements (RNF-001 to RNF-010)
- **RNF-001**: El sistema debe ser capaz de manejar hasta 1000 intentos de inicio de sesión por segundo.
- **RNF-002**: La respuesta del sistema a una autenticación válida debe ser menor de 2 segundos.
- **RNF-003**: El sistema debe cumplir con las normativas de protección de datos personales.
- **RNF-004**: La interfaz debe ser accesible desde dispositivos móviles y de escritorio.
- **RNF-005**: El código debe seguir las mejores prácticas de seguridad.
- **RNF-006**: El sistema debe ser auditado periódicamente en términos de seguridad.
- **RNF-007**: El rendimiento del sistema debe ser monitoreado continuamente.
- **RNF-008**: Los logs deben almacenar la información necesaria sin comprometer la privacidad.
- **RNF-009**: Las contraseñas de usuario no deben ser recuperables.
- **RNF-010**: El sistema debe actualizarse para incorporar nuevas tecnologías de seguridad.

#### Drupal Data Model
- **Content Types**: Usuarios, Autenticación, Sesiones.
- **Taxonomies**: Roles de usuario (Administrador, Usuario Normal, Invitado).

#### Process Flows
1. El usuario accede a la página de inicio de sesión.
2. Introduce su nombre de usuario y contraseña.
3. El sistema verifica las credenciales.
4. Si son válidas, se establece una sesión.
5. Si son inválidas, se muestra un mensaje de error.

### Version History
- **3.2** - 04/11/2025: Actualización sección Autenticación Usuarios con análisis completo de requisitos HU-CPA-0001.