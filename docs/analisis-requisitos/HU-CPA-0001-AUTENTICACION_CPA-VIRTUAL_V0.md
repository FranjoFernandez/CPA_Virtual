# DOCUMENTO DE ANÁLISIS DE REQUISITOS

## HU-CPA-0001-AUTENTICACION_CPA-VIRTUAL_V0

---

## 📋 INFORMACIÓN GENERAL

| Campo | Valor |
|-------|-------|
| **ID Historia de Usuario** | HU-CPA-0001-AUTENTICACION_CPA-VIRTUAL |
| **Versión Documento** | V0 |
| **Fecha Creación** | 2025-11-03 |
| **Analista** | FranjoFernandez |
| **Estado** | En Análisis |
| **Prioridad** | Alta |
| **Módulo** | Autenticación y Acceso |
| **Proyecto** | CPA Virtual |

---

## 📖 HISTORIA DE USUARIO

### Narrativa

**Como** usuario que debe logarse y tener cuenta (usuario y clave)

**Quiero** poder acceder a la parte privada del aplicativo CPA Virtual

**Para** una vez verificado que es un usuario autorizado a la parte privada de CPA Virtual, obtener el CPA al que pertenece y su perfil de usuario. Y en base a su perfil, mostrar en pantalla las distintas opciones de menú activadas a las que podrá acceder.

### Descripción Funcional

Se accederá desde la zona pública del aplicativo CPA Virtual, desde su menú superior, con la opción 'Mi CPA', desde la que se presentará el formulario detallado en esta HU.

En dicho formulario, debe verificarse, mediante la cumplimentación del código de acceso y clave, que la persona Socia/usuaria logada tenga cuenta para poder acceder a la parte privada del aplicativo CPA Virtual.

---

## ✅ CRITERIOS DE ACEPTACIÓN

### Escenario 1: Formulario Autenticación

**Contexto:** Debe verificarse que el usuario que se introduzca en pantalla, esté autorizado y tenga acceso a la parte privada del CPA Virtual.

**Resultado esperado:** Una vez verificado que el usuario tiene cuenta privada y por tanto acceso a la parte privada CPA, se le mostrará un menú personalizado, acorde a su perfil, desde donde poder realizar las distintas funciones que le aparezcan en su menú.

---

### Escenario 2: Nombre de usuario

**Contexto:** Se presenta un campo texto. Editable. Obligatorio. Por defecto sin contenido.

**Resultado esperado:** Se presentará en el campo del formulario el valor introducido manualmente por el usuario.

---

### Escenario 3: Clave

**Contexto:** Se presenta un campo texto. Editable. Obligatorio. Por defecto sin contenido.

**Resultado esperado:** Se presentará en el campo del formulario el valor introducido manualmente por el usuario.

---

### Escenario 4: Botón Iniciar Sesión

**Contexto:** Se presenta en el formulario el botón Iniciar Sesión

**Evento:** Si se decide pulsar.

**Resultado esperado:** 

Mediante la operación `VerificarUsuario` se verificará si el 'nombre de usuario' y 'clave' introducidos existen en el tipo de contenido 'Usuarios', 'TiposUsuarios', 'PersonasSocias' del repositorio Drupal, filtrando por 'tipo usuario' con valor 'Persona Socia/usuaria'. 

**Si encuentra:**
- Se obtendrán los datos personales del usuario (DNI/NIE, nombre y apellidos, dirección, teléfono, correo, fotografía, avisar a, fecha alta), así como los datos del centro (codigo centro, nombre centro, codigo postal, codigo provincia del centro, nombre provincia del centro) y perfil al que pertenece el usuario autenticado (codigo perfil, nombre perfil)
- Todo ello mediante las operaciones:
  - `consultarDatosPersonalesUsuario` de los tipos de contenido 'Usuarios', 'PersonasSocias', 'TiposVia', 'Provincias', 'Municipios' y 'Localidades'
  - `consultarListadoCentros` de los tipos de contenido 'Centros', 'UsuariosCentros', 'Provincias', 'Municipios' y 'Localidades' del repositorio Drupal
  - `consultarListadoPerfilesCentros` de los tipos de contenido 'Perfiles' y 'UsuariosCentrosPerfiles'
- En base al sumatorio de los perfiles del usuario, se le mostrarán al usuario las opciones de menú que le correspondan en el menú personalizado del Escritorio CPA Virtual
- De los centros obtenidos, será a los que podrá acceder en las distintas opciones de menú presentados en el Escritorio CPA Virtual
- Por último se accederá al 'Formulario Acceso Parte Privada', detallado en la HU-CPA-0051-ACCESO-PARTE-PRIVADA-CPA-VIRTUAL_V0

**Si no encuentra:**
- Se presentará el mensaje informativo de error: 'Usuario o contraseña no reconocidos. ¿Olvidaste tu contraseña?'

---

### Escenario 5: Botón ¿Olvidó su contraseña?

**Contexto:** Se presenta en el formulario el botón ¿Olvidó su contraseña?

**Evento:** Si se decide pulsar.

**Resultado esperado:** 

Se accederá de inicio a la ventana con título 'Reinicializar su contraseña', que presentará el campo 'Nombre de usuario o correo electrónico' en la que el usuario deberá introducir su email para poder gestionar la nueva contraseña. 

Una vez cumplimentada su dirección de correo y pulsado el botón 'enviar', recibirá un correo en dicha dirección desde dónde podrá cumplimentar la nueva contraseña, la cual una vez enviada, será actualizada y almacenada en la base de datos de Drupal, mediante las operaciones:
- `obtenerCódigoUsuarioPorEmail` 
- `actualizarClaveAccesoUsuario` 

Ambas operaciones accederán al tipo de contenido 'Usuarios' del repositorio Drupal.

---

## 🎯 REQUISITOS FUNCIONALES

### RF-001: Presentación del Formulario de Autenticación
**Prioridad:** Alta  
**Descripción:** El sistema debe presentar un formulario de autenticación accesible desde la opción 'Mi CPA' del menú superior de la zona pública.

**Criterios de validación:**
- El formulario debe ser accesible desde la zona pública
- Debe mostrarse al seleccionar la opción 'Mi CPA'
- El formulario debe estar correctamente estructurado con todos sus elementos

---

### RF-002: Campo Nombre de Usuario
**Prioridad:** Alta  
**Descripción:** El sistema debe presentar un campo de texto para introducir el nombre de usuario.

**Criterios de validación:**
- Tipo: Campo de texto
- Estado: Editable
- Validación: Obligatorio
- Valor por defecto: Vacío
- Debe aceptar entrada manual del usuario

---

### RF-003: Campo Clave
**Prioridad:** Alta  
**Descripción:** El sistema debe presentar un campo de texto para introducir la contraseña.

**Criterios de validación:**
- Tipo: Campo de texto (password)
- Estado: Editable
- Validación: Obligatorio
- Valor por defecto: Vacío
- Debe ocultar los caracteres introducidos
- Debe aceptar entrada manual del usuario

---

### RF-004: Verificación de Credenciales
**Prioridad:** Alta  
**Descripción:** El sistema debe verificar las credenciales introducidas contra la base de datos de usuarios autorizados.

**Criterios de validación:**
- Implementar operación `VerificarUsuario`
- Consultar tipos de contenido: 'Usuarios', 'TiposUsuarios', 'PersonasSocias'
- Filtrar por tipo usuario: 'Persona Socia/usuaria'
- Validar coincidencia de usuario y clave
- Gestión de intentos fallidos

---

### RF-005: Obtención de Datos Personales
**Prioridad:** Alta  
**Descripción:** Una vez autenticado, el sistema debe obtener los datos personales del usuario.

**Criterios de validación:**
- Implementar operación `consultarDatosPersonalesUsuario`
- Obtener: DNI/NIE, nombre, apellidos, dirección, teléfono, correo, fotografía, avisar a, fecha alta
- Consultar tipos de contenido: 'Usuarios', 'PersonasSocias', 'TiposVia', 'Provincias', 'Municipios', 'Localidades'
- Datos completos y actualizados

---

### RF-006: Obtención de Datos de Centro(s)
**Prioridad:** Alta  
**Descripción:** El sistema debe obtener información del/los centro(s) al(los) que pertenece el usuario.

**Criterios de validación:**
- Implementar operación `consultarListadoCentros`
- Obtener: código centro, nombre centro, código postal, código provincia, nombre provincia
- Consultar tipos de contenido: 'Centros', 'UsuariosCentros', 'Provincias', 'Municipios', 'Localidades'
- Permitir múltiples centros por usuario

---

### RF-007: Obtención de Perfiles de Usuario
**Prioridad:** Alta  
**Descripción:** El sistema debe obtener el/los perfil(es) asignado(s) al usuario autenticado.

**Criterios de validación:**
- Implementar operación `consultarListadoPerfilesCentros`
- Obtener: código perfil, nombre perfil
- Consultar tipos de contenido: 'Perfiles', 'UsuariosCentrosPerfiles'
- Permitir múltiples perfiles por usuario

---

### RF-008: Generación de Menú Personalizado
**Prioridad:** Alta  
**Descripción:** El sistema debe generar un menú personalizado basado en el sumatorio de perfiles del usuario.

**Criterios de validación:**
- Calcular permisos basados en todos los perfiles del usuario
- Mostrar solo opciones de menú autorizadas
- Menú dinámico según perfiles
- Acceso restringido a centros autorizados

---

### RF-009: Acceso a Parte Privada
**Prioridad:** Alta  
**Descripción:** Una vez verificado y obtenidos los datos, el sistema debe redirigir al usuario a la parte privada.

**Criterios de validación:**
- Redirigir al 'Formulario Acceso Parte Privada' (HU-CPA-0051-ACCESO-PARTE-PRIVADA-CPA-VIRTUAL_V0)
- Mantener sesión activa
- Transferir contexto de usuario

---

### RF-010: Gestión de Errores de Autenticación
**Prioridad:** Alta  
**Descripción:** El sistema debe informar al usuario cuando las credenciales sean incorrectas.

**Criterios de validación:**
- Mostrar mensaje: 'Usuario o contraseña no reconocidos. ¿Olvidaste tu contraseña?'
- No especificar qué campo es incorrecto (seguridad)
- Ofrecer opción de recuperación de contraseña

---

### RF-011: Funcionalidad Olvidó Contraseña - Acceso
**Prioridad:** Media  
**Descripción:** El sistema debe proporcionar acceso a la funcionalidad de recuperación de contraseña.

**Criterios de validación:**
- Botón '¿Olvidó su contraseña?' visible en formulario
- Al pulsar, abrir ventana 'Reinicializar su contraseña'
- Presentar campo 'Nombre de usuario o correo electrónico'

---

### RF-012: Funcionalidad Olvidó Contraseña - Envío
**Prioridad:** Media  
**Descripción:** El sistema debe enviar un correo electrónico para restablecer la contraseña.

**Criterios de validación:**
- Implementar operación `obtenerCódigoUsuarioPorEmail`
- Validar que el email existe en el sistema
- Enviar correo con enlace de restablecimiento
- Enlace temporal y seguro

---

### RF-013: Funcionalidad Olvidó Contraseña - Actualización
**Prioridad:** Media  
**Descripción:** El sistema debe permitir actualizar la contraseña desde el enlace recibido.

**Criterios de validación:**
- Implementar operación `actualizarClaveAccesoUsuario`
- Validar token de restablecimiento
- Actualizar contraseña en tipo de contenido 'Usuarios'
- Confirmar actualización al usuario

---

## 🔒 REQUISITOS NO FUNCIONALES

### RNF-001: Seguridad - Encriptación de Contraseña
**Categoría:** Seguridad  
**Descripción:** Las contraseñas deben almacenarse de forma segura mediante algoritmos de hash.

**Criterios:**
- Utilizar algoritmos seguros (bcrypt, Argon2, etc.)
- No almacenar contraseñas en texto plano
- Salt único por contraseña

---

### RNF-002: Seguridad - Transmisión de Datos
**Categoría:** Seguridad  
**Descripción:** La transmisión de credenciales debe realizarse de forma segura.

**Criterios:**
- Utilizar HTTPS/SSL para todas las comunicaciones
- No transmitir contraseñas sin encriptar
- Certificados válidos y actualizados

---

### RNF-003: Seguridad - Sesiones
**Categoría:** Seguridad  
**Descripción:** La gestión de sesiones debe ser segura.

**Criterios:**
- Tokens de sesión seguros y únicos
- Timeout de sesión configurable
- Invalidación de sesión al cerrar sesión
- Protección contra CSRF

---

### RNF-004: Seguridad - Intentos de Acceso
**Categoría:** Seguridad  
**Descripción:** Protección contra ataques de fuerza bruta.

**Criterios:**
- Limitar intentos de login fallidos
- Bloqueo temporal tras X intentos fallidos
- Log de intentos de acceso
- Captcha opcional tras varios intentos

---

### RNF-005: Usabilidad - Accesibilidad
**Categoría:** Usabilidad  
**Descripción:** El formulario debe ser accesible según estándares WCAG.

**Criterios:**
- Cumplimiento WCAG 2.1 nivel AA
- Navegación por teclado
- Etiquetas ARIA apropiadas
- Contraste de colores adecuado

---

### RNF-006: Rendimiento - Tiempo de Respuesta
**Categoría:** Rendimiento  
**Descripción:** La verificación de credenciales debe ser rápida.

**Criterios:**
- Tiempo de respuesta < 2 segundos en condiciones normales
- Optimización de consultas a base de datos
- Caché de datos no sensibles cuando sea apropiado

---

### RNF-007: Compatibilidad - Navegadores
**Categoría:** Compatibilidad  
**Descripción:** El formulario debe funcionar en navegadores modernos.

**Criterios:**
- Chrome (últimas 2 versiones)
- Firefox (últimas 2 versiones)
- Safari (últimas 2 versiones)
- Edge (últimas 2 versiones)

---

### RNF-008: Compatibilidad - Dispositivos
**Categoría:** Compatibilidad  
**Descripción:** Responsive design para diferentes dispositivos.

**Criterios:**
- Diseño adaptable (desktop, tablet, móvil)
- Touch-friendly en dispositivos táctiles
- Viewport configurado correctamente

---

### RNF-009: Auditoria - Logging
**Categoría:** Auditoria  
**Descripción:** Registro de eventos de autenticación.

**Criterios:**
- Log de accesos exitosos
- Log de accesos fallidos
- Información: timestamp, usuario, IP, resultado
- Cumplimiento LOPD/GDPR

---

### RNF-010: Disponibilidad
**Categoría:** Disponibilidad  
**Descripción:** El sistema de autenticación debe estar altamente disponible.

**Criterios:**
- Disponibilidad 99.5% o superior
- Mecanismos de failover
- Monitorización continua

---

## 📊 MODELO DE DATOS

### Entidades Implicadas

#### 1. Usuarios
**Descripción:** Información de credenciales y datos de acceso

**Atributos:**
- codigo_usuario (PK)
- nombre_usuario
- clave_acceso (hash)
- correo_electronico
- fecha_alta
- estado
- ultimo_acceso
- intentos_fallidos

---

#### 2. PersonasSocias
**Descripción:** Datos personales de las personas socias/usuarias

**Atributos:**
- codigo_persona (PK)
- codigo_usuario (FK)
- dni_nie
- nombre
- apellidos
- direccion
- telefono
- fotografia
- avisar_a
- codigo_tipo_via (FK)
- codigo_municipio (FK)
- codigo_localidad (FK)

---

## 🔄 FLUJOS DE PROCESO

### Flujo Principal: Autenticación Exitosa

1. Usuario accede a zona pública de CPA Virtual
2. Usuario selecciona opción 'Mi CPA' del menú superior
3. Sistema presenta Formulario de Autenticación
4. Usuario introduce nombre de usuario y clave de acceso
5. Usuario pulsa botón 'Iniciar Sesión'
6. Sistema ejecuta OP-001: VerificarUsuario
7. Si credenciales válidas:
   - Sistema ejecuta OP-002: consultarDatosPersonalesUsuario
   - Sistema ejecuta OP-003: consultarListadoCentros
   - Sistema ejecuta OP-004: consultarListadoPerfilesCentros
   - Sistema genera menú personalizado según perfiles
   - Sistema redirige a Formulario Acceso Parte Privada

---

**FIN DEL DOCUMENTO**