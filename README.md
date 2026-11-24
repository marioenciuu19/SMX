## 23 · Actividades

En este apartado se recopilarán las actividades y entregas realizadas durante el desarrollo del proyecto Impulsa. Se incluirán informes técnicos, diseños y documentación relacionada con las diferentes partes de la plataforma.

---

### 23.1. Informe del Backend

#### 23.1.1. Introducción

El backend de Impulsa será la parte encargada de gestionar la lógica interna de la aplicación. Su función principal será procesar las solicitudes de los usuarios, gestionar la información y comunicarse con la base de datos.

#### 23.1.2. Objetivos del Backend

Los principales objetivos serán:

- Gestionar el registro y acceso de usuarios.
- Administrar la información de las empresas.
- Gestionar clientes y trabajadores.
- Controlar los servicios disponibles.
- Gestionar las citas y reservas.
- Administrar presupuestos, facturas y pagos.
- Controlar el inventario.
- Gestionar los permisos de cada usuario.
- Mantener separados los datos de las diferentes empresas.

#### 23.1.3. Tecnologías utilizadas

Para desarrollar el backend se plantea utilizar las siguientes tecnologías:

- **Node.js:** permitirá ejecutar JavaScript en el servidor.
- **Next.js:** permitirá desarrollar las funciones del servidor y crear las rutas de la API.
- **Prisma ORM:** facilitará la comunicación entre el backend y la base de datos.
- **PostgreSQL:** almacenará toda la información de la plataforma.
- **API REST:** permitirá intercambiar información entre el frontend y el backend.

#### 23.1.4. Funcionamiento

Cuando un usuario realice una acción desde la interfaz, el frontend enviará una petición al backend.

El backend recibirá la petición, comprobará los datos, verificará los permisos y realizará la operación correspondiente en la base de datos.

Finalmente, devolverá una respuesta al frontend para mostrar el resultado al usuario.

#### 23.1.5. Seguridad

El backend deberá incorporar diferentes medidas de seguridad:

- Validación de los datos recibidos.
- Protección de contraseñas.
- Autenticación de usuarios.
- Control de permisos.
- Separación de información entre empresas.
- Protección frente a accesos no autorizados.

#### 23.1.6. Conclusión

El backend será una parte fundamental de Impulsa, ya que permitirá conectar la interfaz de usuario con la base de datos y gestionar todas las operaciones necesarias para el funcionamiento de la plataforma.

---

### 23.2. Mockup de Impulsa

#### 23.2.1. Introducción

El mockup representa una propuesta visual de cómo será la interfaz de Impulsa. Su objetivo es mostrar la distribución de los elementos, los apartados principales y la navegación de la plataforma antes de comenzar su desarrollo completo.

#### 23.2.2. Objetivos del diseño

- Crear una interfaz sencilla y profesional.
- Facilitar la navegación por los diferentes módulos.
- Organizar correctamente la información.
- Mantener una apariencia visual coherente.
- Facilitar el uso de la plataforma desde diferentes dispositivos.

#### 23.2.3. Elementos principales

El diseño contempla los siguientes apartados:

- Panel principal de administración.
- Gestión de clientes.
- Gestión de trabajadores.
- Gestión de servicios.
- Calendario de citas.
- Presupuestos y facturas.
- Inventario.
- Informes.
- Configuración de la empresa.

#### 23.2.4. Mockup visual

A continuación se incorporará la imagen del mockup realizado para representar el diseño de la plataforma Impulsa.

**[INSERTAR AQUÍ LA IMAGEN DEL MOCKUP]**

#### 23.2.5. Conclusión

El mockup permitirá visualizar cómo estará organizada la plataforma y servirá como referencia durante el desarrollo del frontend. También ayudará a mantener una estructura coherente entre los diferentes apartados de Impulsa.
