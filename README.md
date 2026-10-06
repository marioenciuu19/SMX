# Impulsa

### Plataforma SaaS de gestión empresarial para empresas de servicios

---

<details>
<summary><strong>Índice</strong></summary>

1. [Introducción — ¿Qué estamos haciendo?](#01--introducción--qué-estamos-haciendo)
2. [Briefing de ideas](#02--briefing-de-ideas)
3. [Arquitectura del software](#03--arquitectura-del-software)
4. [Tecnologías a utilizar](#04--tecnologías-a-utilizar)
5. [Red](#05--red)
6. [Diagrama de la red](#06--diagrama-de-la-red)
7. [Mapa físico](#07--mapa-físico)
8. [Mapa lógico](#08--mapa-lógico)
9. [Web](#09--web)
10. [Diseño](#10--diseño)
11. [Mockup](#11--mockup)
12. [Mapa de navegabilidad](#12--mapa-de-navegabilidad)
13. [Base de datos](#13--base-de-datos)
14. [Servicios explicado de un modo sencillo](#14--servicios-explicado-de-un-modo-sencillo)
15. [DNS](#15--dns)
16. [DHCP](#16--dhcp)
17. [Apache](#17--apache)
18. [Firewall](#18--firewall)
19. [Copias de seguridad](#19--copias-de-seguridad)
20. [Conclusiones](#20--conclusiones)
21. [Bibliografía](#21--bibliografía)
22. [Guías de usuario](#22--guías-de-usuario)

</details>

---

<details>
<summary><strong>01 · Introducción — ¿Qué estamos haciendo?</strong></summary>

### 1.1. ¿Qué es Impulsa?

**Impulsa** es una plataforma SaaS de gestión empresarial destinada principalmente a pequeñas y medianas empresas de servicios.

El objetivo es crear una herramienta que permita gestionar diferentes áreas de una empresa desde un único lugar.

### 1.2. ¿Qué significa SaaS?

**SaaS** significa *Software as a Service*, es decir, **software como servicio**.

La aplicación estará disponible a través de Internet para que los usuarios puedan utilizarla sin necesidad de instalar todo el sistema localmente.

### 1.3. Objetivo principal

El objetivo principal de Impulsa es facilitar la gestión diaria de una empresa.

La plataforma permitirá gestionar:

* **Empresas.**
* **Clientes.**
* **Trabajadores.**
* **Servicios.**
* **Citas y calendario.**
* **Presupuestos.**
* **Facturas y pagos.**
* **Inventario.**
* **Informes.**
* **Página web pública.**
* **Área privada de clientes.**
* **Inteligencia Artificial.**

### 1.4. Funcionamiento general

El funcionamiento será sencillo:

1. La empresa se registra.
2. Introduce la información de su negocio.
3. Accede al panel de gestión.
4. Gestiona clientes, trabajadores y servicios.
5. Organiza las citas.
6. Gestiona presupuestos, facturas y pagos.
7. Controla el inventario.
8. Consulta informes.
9. La información introducida puede utilizarse para generar automáticamente la página web pública.

### 1.5. Página web automática

Una de las principales características de Impulsa será la generación automática de una página web para cada empresa.

La empresa no tendrá que crear manualmente una página web desde cero.

Por ejemplo:

* Introduce el nombre.
* Añade el logotipo.
* Añade los servicios.
* Añade el horario.
* Añade la información de contacto.

Impulsa utilizará estos datos para mostrar la información correspondiente en la página pública.

### 1.6. Usuarios

#### 1.6.1. Empresa

La empresa será el usuario principal y podrá gestionar su negocio.

#### 1.6.2. Trabajadores

Los trabajadores podrán disponer de cuentas con diferentes permisos.

#### 1.6.3. Clientes

Los clientes podrán consultar la página pública y acceder a un área privada.

</details>

---

<details>
<summary><strong>02 · Briefing de ideas</strong></summary>

### 2.1. Idea inicial

La idea de Impulsa surge de la necesidad de facilitar la gestión de pequeñas y medianas empresas de servicios.

Muchas empresas utilizan diferentes herramientas para gestionar clientes, citas, facturas o inventario.

La propuesta consiste en reunir estas funciones dentro de una única plataforma.

### 2.2. Problemas detectados

#### 2.2.1. Información repartida

La información puede estar almacenada en diferentes programas o documentos.

#### 2.2.2. Gestión manual

Algunas tareas pueden realizarse manualmente, aumentando el tiempo necesario para gestionarlas.

#### 2.2.3. Creación de páginas web

Una empresa puede necesitar conocimientos técnicos o contratar a otra persona para crear una página web.

#### 2.2.4. Gestión de clientes

La información de los clientes puede resultar difícil de organizar cuando se utilizan diferentes herramientas.

#### 2.2.5. Gestión de citas

La gestión manual de citas puede provocar errores o dificultades para organizar el calendario.

### 2.3. Solución propuesta

Impulsa pretende centralizar estas funciones.

La empresa tendrá un único panel desde el que podrá gestionar toda su información.

### 2.4. Lluvia de ideas

#### 2.4.1. Gestión de empresas

* Nombre.
* Logotipo.
* Dirección.
* Teléfono.
* Correo electrónico.
* Horario.
* Descripción.
* Datos fiscales.
* Servicios.

#### 2.4.2. Gestión de clientes

* Datos personales.
* Información de contacto.
* Historial de servicios.
* Citas.
* Presupuestos.
* Facturas.
* Pagos.
* Notas.
* Incidencias.

#### 2.4.3. Gestión de trabajadores

* Datos personales.
* Horarios.
* Servicios asignados.
* Citas.
* Permisos.

#### 2.4.4. Gestión de servicios

* Nombre.
* Descripción.
* Precio.
* Duración.
* Disponibilidad.

#### 2.4.5. Gestión de citas

* Calendario.
* Fecha.
* Hora.
* Cliente.
* Trabajador.
* Servicio.
* Estado.

#### 2.4.6. Presupuestos

* Creación de presupuestos.
* Datos del cliente.
* Servicios.
* Precios.
* Estado.
* Aceptación.

#### 2.4.7. Facturas y pagos

* Creación de facturas.
* Control de pagos.
* Estado de las facturas.
* Historial.

#### 2.4.8. Inventario

* Productos.
* Cantidad.
* Stock.
* Precio.
* Avisos de stock bajo.

#### 2.4.9. Inteligencia Artificial

La plataforma podrá incorporar diferentes funciones de IA:

* Responder preguntas sobre la empresa.
* Generar informes.
* Ayudar a crear presupuestos.
* Redactar mensajes para clientes.
* Analizar información.
* Detectar necesidades de inventario.
* Crear un chatbot para la página web.

#### 2.4.10. Funciones futuras

* Aplicación móvil.
* Pagos online.
* Reseñas.
* Notificaciones por WhatsApp.
* Integración con Google Calendar.
* Predicción de ventas.
* Predicción de inventario.
* Integraciones contables.
* Aplicación para trabajadores.
* Firmas digitales.

</details>

---

<details>
<summary><strong>03 · Arquitectura del software</strong></summary>

### 3.1. Estructura general

La arquitectura de Impulsa estará formada por diferentes componentes que trabajarán conjuntamente.

### 3.2. Frontend

El **frontend** será la parte visual de la aplicación.

Será la parte con la que interactuará directamente el usuario.

#### 3.2.1. Funciones

* Mostrar información.
* Mostrar formularios.
* Mostrar tablas.
* Mostrar botones.
* Mostrar menús.
* Permitir la interacción del usuario.

### 3.3. Backend

El **backend** será la parte encargada de procesar la información y ejecutar la lógica de la aplicación.

#### 3.3.1. Funciones

* Gestionar usuarios.
* Gestionar autenticación.
* Gestionar empresas.
* Gestionar clientes.
* Gestionar trabajadores.
* Gestionar servicios.
* Gestionar citas.
* Gestionar presupuestos.
* Gestionar facturas.
* Gestionar inventario.

### 3.4. Base de datos

La base de datos almacenará la información necesaria para el funcionamiento de Impulsa.

#### 3.4.1. Información almacenada

* Empresas.
* Usuarios.
* Clientes.
* Trabajadores.
* Servicios.
* Citas.
* Presupuestos.
* Facturas.
* Pagos.
* Inventario.

### 3.5. Servidor

El servidor ejecutará los diferentes servicios necesarios para que Impulsa funcione.

### 3.6. Sistema multiempresa

Impulsa permitirá gestionar diferentes empresas dentro de la misma plataforma.

```text
IMPULSA
│
├── Empresa A
│   ├── Clientes
│   ├── Trabajadores
│   ├── Citas
│   └── Facturas
│
├── Empresa B
│   ├── Clientes
│   ├── Trabajadores
│   ├── Citas
│   └── Facturas
│
└── Empresa C
    ├── Clientes
    ├── Trabajadores
    ├── Citas
    └── Facturas
```

### 3.7. Separación de datos

Cada empresa tendrá sus propios datos.

**Una empresa no podrá acceder a los datos de otra empresa.**

</details>

---

<details>
<summary><strong>04 · Tecnologías a utilizar</strong></summary>

### 4.1. HTML

HTML se utilizará para crear la estructura de las páginas web.

### 4.2. CSS

CSS se utilizará para definir el diseño visual.

Permitirá controlar:

* Colores.
* Tamaños.
* Espaciados.
* Posición de elementos.
* Diseño de formularios.

### 4.3. JavaScript

JavaScript permitirá añadir interactividad.

Por ejemplo:

* Botones.
* Formularios.
* Menús.
* Validaciones.
* Actualización de información.

### 4.4. Backend

El backend utilizará una tecnología adecuada para gestionar la lógica de Impulsa y comunicarse con la base de datos.

### 4.5. Base de datos

Se utilizará una base de datos para almacenar toda la información.

### 4.6. Docker

**Docker** permite ejecutar aplicaciones dentro de contenedores.

En Impulsa podrá utilizarse para separar diferentes servicios.

```text
Docker
│
├── Aplicación
├── Base de datos
├── Servidor web
└── Otros servicios
```

### 4.7. Git

Git permitirá controlar las diferentes versiones del proyecto.

### 4.8. GitHub

GitHub se utilizará para almacenar el código y documentar el desarrollo.

</details>

---

<details>
<summary><strong>05 · Red</strong></summary>

### 5.1. Estructura de la red

La red permitirá conectar los diferentes dispositivos y servicios necesarios para Impulsa.

### 5.2. Router

El router permitirá conectar la red interna con Internet.

### 5.3. Switch

El switch permitirá conectar los diferentes dispositivos dentro de la red.

### 5.4. Servidor

El servidor ejecutará los servicios de Impulsa.

### 5.5. Firewall

El firewall controlará el tráfico de red.

### 5.6. Puntos de acceso

Los puntos de acceso permitirán conectar dispositivos mediante Wi-Fi.

### 5.7. Seguridad

Se utilizarán diferentes medidas:

* Firewall.
* VLAN.
* Contraseñas seguras.
* Control de acceso.
* HTTPS.
* Copias de seguridad.

</details>

---

<details>
<summary><strong>06 · Diagrama de la red</strong></summary>

### 6.1. Diagrama general

```text
                         INTERNET
                             |
                          ROUTER
                             |
                          FIREWALL
                             |
                           SWITCH
                    _________|_________
                   |         |         |
                SERVIDOR  ORDENADORES  WIFI
                   |         |         |
                IMPULSA   EMPLEADOS  CLIENTES
```

### 6.2. Funcionamiento

#### 6.2.1. Internet

Proporciona la conexión externa.

#### 6.2.2. Router

Gestiona la comunicación entre Internet y la red interna.

#### 6.2.3. Firewall

Controla las conexiones permitidas y bloquea las no autorizadas.

#### 6.2.4. Switch

Conecta los diferentes dispositivos.

#### 6.2.5. Servidor

Ejecuta los servicios necesarios para Impulsa.

#### 6.2.6. Wi-Fi

Permite conectar dispositivos inalámbricos.

</details>

---

<details>
<summary><strong>07 · Mapa físico</strong></summary>

### 7.1. Distribución física

La infraestructura estará organizada para facilitar el mantenimiento y la seguridad.

### 7.2. Zona de comunicaciones

En esta zona estarán los principales dispositivos de red:

* Router.
* Firewall.
* Switch.
* Servidor.
* SAI.

### 7.3. Zona de trabajo

En esta zona estarán:

* Ordenadores.
* Impresoras.
* Puntos de acceso.

### 7.4. Conexiones

Los dispositivos podrán conectarse mediante:

* Cable Ethernet.
* Wi-Fi.

Los dispositivos principales utilizarán conexiones cableadas para disponer de una conexión estable.

</details>

---

<details>
<summary><strong>08 · Mapa lógico</strong></summary>

### 8.1. Direccionamiento IP

La red utilizará direcciones IP privadas.

### 8.2. Ejemplo de configuración

```text
Red:       192.168.0.0/24
Gateway:   192.168.0.1
Servidor:  192.168.0.10
```

### 8.3. VLAN

Las VLAN permitirán separar diferentes tipos de dispositivos y tráfico.

#### 8.3.1. Ejemplo

* VLAN de administración.
* VLAN de trabajadores.
* VLAN de invitados.
* VLAN de servidores.

### 8.4. Seguridad

La comunicación entre las diferentes redes estará controlada mediante las reglas correspondientes y el firewall.

</details>

---

<details>
<summary><strong>09 · Web</strong></summary>

### 9.1. Página web pública

Cada empresa registrada tendrá una página web pública.

### 9.2. Información pública

La página podrá mostrar:

* Nombre.
* Logotipo.
* Descripción.
* Servicios.
* Horario.
* Teléfono.
* Correo electrónico.
* Ubicación.

### 9.3. Panel de gestión

La empresa tendrá un panel privado.

#### 9.3.1. Funciones

* Clientes.
* Trabajadores.
* Servicios.
* Citas.
* Presupuestos.
* Facturas.
* Pagos.
* Inventario.
* Informes.
* Inteligencia Artificial.

### 9.4. Área privada del cliente

El cliente podrá iniciar sesión y consultar su información.

#### 9.4.1. Funciones

* Datos personales.
* Citas.
* Historial.
* Presupuestos.
* Facturas.
* Pagos.
* Incidencias.

### 9.5. Generación automática

La información introducida en el panel podrá utilizarse automáticamente para generar la página pública.

</details>

---

<details>
<summary><strong>10 · Diseño</strong></summary>

### 10.1. Diseño general

El diseño de Impulsa será sencillo, profesional y fácil de utilizar.

### 10.2. Objetivos del diseño

* Facilitar la navegación.
* Mostrar la información claramente.
* Mantener una estructura organizada.
* Evitar interfaces innecesariamente complicadas.

### 10.3. Elementos de la interfaz

* Menú lateral.
* Barra superior.
* Dashboard.
* Tarjetas.
* Tablas.
* Formularios.
* Botones.
* Ventanas de información.

### 10.4. Experiencia de usuario

La plataforma estará diseñada para que las funciones principales sean fáciles de localizar y utilizar.

</details>

---

<details>
<summary><strong>11 · Mockup</strong></summary>

### 11.1. Panel de empresa

El mockup mostrará cómo será la interfaz principal.

#### 11.1.1. Elementos

* Menú lateral.
* Dashboard.
* Clientes.
* Citas.
* Servicios.
* Facturas.
* Inventario.
* Informes.

### 11.2. Página web pública

El mockup mostrará cómo verá la página un cliente.

#### 11.2.1. Elementos

* Logotipo.
* Nombre.
* Información.
* Servicios.
* Horario.
* Contacto.
* Botón para solicitar cita.

### 11.3. Área privada

El mockup mostrará la zona privada del cliente.

#### 11.3.1. Elementos

* Perfil.
* Citas.
* Historial.
* Presupuestos.
* Facturas.
* Pagos.

</details>

---

<details>
<summary><strong>12 · Mapa de navegabilidad</strong></summary>

### 12.1. Navegación de la empresa

```text
Inicio
│
├── Empresas
├── Clientes
├── Trabajadores
├── Servicios
├── Citas
├── Presupuestos
├── Facturas
├── Pagos
├── Inventario
├── Informes
├── Inteligencia Artificial
└── Configuración
```

### 12.2. Navegación del cliente

```text
Inicio
│
├── Empresa
├── Servicios
├── Citas
└── Área privada
    │
    ├── Datos personales
    ├── Historial
    ├── Presupuestos
    ├── Facturas
    ├── Pagos
    └── Incidencias
```

### 12.3. Objetivo

El mapa de navegabilidad permitirá representar de forma sencilla cómo se desplazará el usuario por la plataforma.

</details>

---

<details>
<summary><strong>13 · Base de datos</strong></summary>

### 13.1. Estructura

La base de datos almacenará toda la información necesaria para el funcionamiento de Impulsa.

### 13.2. Empresas

Almacenará la información de cada empresa.

### 13.3. Usuarios

Almacenará los usuarios y sus permisos.

### 13.4. Clientes

Almacenará la información de los clientes.

### 13.5. Trabajadores

Almacenará la información de los trabajadores.

### 13.6. Servicios

Almacenará los servicios disponibles.

### 13.7. Citas

Almacenará las citas programadas.

### 13.8. Presupuestos

Almacenará los presupuestos realizados.

### 13.9. Facturas

Almacenará las facturas.

### 13.10. Pagos

Almacenará la información de los pagos.

### 13.11. Inventario

Almacenará los productos y las cantidades disponibles.

### 13.12. Relaciones

Las diferentes tablas estarán relacionadas mediante identificadores.

Por ejemplo:

```text
Empresa
   |
   └── Cliente
         |
         └── Cita
               |
               └── Servicio
```

### 13.13. Separación de datos

Cada registro estará relacionado con la empresa correspondiente.

Esto permitirá mantener separados los datos de las diferentes empresas.

</details>

---

<details>
<summary><strong>14 · Servicios explicado de un modo sencillo (vinculado al diagrama de la red)</strong></summary>

### 14.1. ¿Qué son los servicios?

Los servicios son diferentes elementos que permiten que la red, el servidor y la aplicación funcionen correctamente.

Para entenderlos mejor, se pueden relacionar directamente con el diagrama de red.

### 14.2. Router

El router conecta nuestra red con Internet.

**Ejemplo:** cuando un ordenador necesita acceder a Internet, la comunicación pasa por el router.

### 14.3. Firewall

El firewall controla qué conexiones pueden entrar o salir de la red.

**Ejemplo:** puede bloquear conexiones que no estén permitidas.

### 14.4. Switch

El switch permite conectar diferentes dispositivos dentro de la red.

Puede conectar:

* Servidores.
* Ordenadores.
* Impresoras.
* Puntos de acceso.

### 14.5. Servidor

El servidor es el equipo encargado de ejecutar los servicios de Impulsa.

Puede almacenar:

* Aplicación.
* Base de datos.
* Archivos.
* Servicios web.

### 14.6. DNS

DNS permite utilizar nombres en lugar de direcciones IP.

### 14.7. DHCP

DHCP asigna automáticamente direcciones IP a los dispositivos.

### 14.8. Apache

Apache actúa como servidor web y permite servir páginas web.

### 14.9. Copias de seguridad

Las copias de seguridad permiten recuperar información en caso de pérdida.

</details>

---

<details>
<summary><strong>15 · DNS</strong></summary>

### 15.1. ¿Qué es DNS?

DNS significa **Domain Name System**.

Es el sistema encargado de traducir nombres de dominio a direcciones IP.

### 15.2. ¿Para qué sirve?

Permite utilizar nombres fáciles de recordar en lugar de direcciones IP.

### 15.3. Ejemplo

En lugar de utilizar directamente:

```text
192.168.0.10
```

se puede utilizar un nombre de dominio.

### 15.4. Uso en Impulsa

DNS permitirá dirigir un dominio hacia el servidor correspondiente.

También podrá utilizarse para las páginas públicas de las empresas.

</details>

---

<details>
<summary><strong>16 · DHCP</strong></summary>

### 16.1. ¿Qué es DHCP?

DHCP es un servicio que permite asignar automáticamente configuraciones de red.

### 16.2. Información proporcionada

Puede proporcionar:

* Dirección IP.
* Máscara de red.
* Puerta de enlace.
* Servidor DNS.

### 16.3. ¿Para qué sirve?

Evita tener que configurar manualmente todos los dispositivos de la red.

### 16.4. Uso en Impulsa

Se utilizará para facilitar la configuración de los equipos conectados a la red.

</details>

---

<details>
<summary><strong>17 · Apache</strong></summary>

### 17.1. ¿Qué es Apache?

Apache es un servidor web.

### 17.2. ¿Para qué sirve?

Su función es recibir peticiones web y proporcionar el contenido correspondiente.

### 17.3. Funcionamiento

Cuando un usuario accede a una página:

1. El usuario realiza una petición.
2. La petición llega al servidor.
3. Apache recibe la petición.
4. Apache busca el contenido correspondiente.
5. El servidor devuelve la respuesta.
6. El usuario visualiza la página.

### 17.4. Uso en Impulsa

Apache podrá utilizarse para servir las páginas web de Impulsa y gestionar las peticiones de los usuarios.

</details>

---

<details>
<summary><strong>18 · Firewall</strong></summary>

### 18.1. ¿Qué es un firewall?

Un firewall es un sistema encargado de controlar el tráfico de red.

### 18.2. ¿Para qué sirve?

Permite:

* Permitir conexiones.
* Bloquear conexiones.
* Controlar puertos.
* Controlar accesos.
* Proteger servicios.

### 18.3. Uso en Impulsa

El firewall ayudará a proteger los servicios de Impulsa frente a conexiones no autorizadas.

### 18.4. Ejemplo

Si un puerto no debe estar disponible desde Internet, el firewall puede bloquear el acceso.

### 18.5. Importancia

El firewall será una de las principales medidas de seguridad de la infraestructura.

</details>

---

<details>
<summary><strong>19 · Copias de seguridad</strong></summary>

### 19.1. ¿Qué son?

Las copias de seguridad son copias de la información que permiten recuperarla si se pierde.

### 19.2. Información que se puede copiar

* Base de datos.
* Archivos.
* Configuración.
* Información de las empresas.
* Información de los clientes.

### 19.3. Situaciones en las que son útiles

* Fallo del servidor.
* Eliminación accidental.
* Corrupción de datos.
* Problemas de hardware.
* Errores humanos.

### 19.4. Sistema de copias

Las copias podrán realizarse periódicamente y almacenarse en una ubicación diferente al servidor principal.

### 19.5. Recuperación

En caso de pérdida de información, se podrá utilizar una copia anterior para restaurar los datos.

</details>

---

<details>
<summary><strong>20 · Conclusiones</strong></summary>

### 20.1. Conclusión general

Impulsa es un proyecto que busca crear una plataforma capaz de centralizar diferentes tareas de gestión empresarial.

El proyecto combina:

* Desarrollo web.
* Redes.
* Bases de datos.
* Seguridad.
* Gestión empresarial.
* Automatización.
* Inteligencia Artificial.

### 20.2. Objetivos conseguidos

El proyecto está planteado para incorporar:

* Gestión empresarial.
* Gestión de clientes.
* Gestión de trabajadores.
* Gestión de servicios.
* Gestión de citas.
* Presupuestos.
* Facturas.
* Pagos.
* Inventario.
* Informes.
* Inteligencia Artificial.
* Página web pública.
* Área privada.
* Sistema multiempresa.
* Separación de datos.
* Seguridad.

### 20.3. Mejoras futuras

En el futuro se podrían añadir:

* Aplicación móvil.
* Pagos online.
* Notificaciones.
* Integración con WhatsApp.
* Google Calendar.
* Firma digital.
* Integraciones contables.
* Aplicación para trabajadores.
* Nuevas funciones de Inteligencia Artificial.

</details>

---

<details>
<summary><strong>21 · Bibliografía</strong></summary>

### 21.1. Fuentes consultadas

En este apartado se incluirán las fuentes utilizadas durante la investigación, planificación y desarrollo del proyecto.

### 21.2. Documentación técnica

Se podrán incluir:

* Documentación oficial de las tecnologías.
* Documentación de redes.
* Documentación de bases de datos.
* Documentación de servidores.
* Documentación de seguridad.

### 21.3. Recursos educativos

También se incluirán:

* Manuales.
* Tutoriales.
* Documentación técnica.
* Recursos educativos.
* Fuentes consultadas durante el desarrollo.

</details>

---

<details>
<summary><strong>22 · Guías de usuario</strong></summary>

### 22.1. Guía del administrador

El administrador podrá gestionar la configuración general de la plataforma.

#### 22.1.1. Funciones

* Gestionar empresas.
* Gestionar usuarios.
* Gestionar permisos.
* Configurar

