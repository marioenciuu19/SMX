# 🧹 CleanFlow

### Plataforma SaaS de gestión empresarial para empresas de servicios

---

# 📑 Índice

1. [Introducción — ¿Qué estamos haciendo?](#1-introducción--qué-estamos-haciendo)
2. [Briefing de ideas — Lluvia de ideas](#2-briefing-de-ideas--lluvia-de-ideas)
3. [Arquitectura del software](#3-arquitectura-del-software)
4. [Tecnologías a utilizar](#4-tecnologías-a-utilizar)
5. [Red](#5-red)
6. [Diagrama de la red](#6-diagrama-de-la-red)
7. [Mapa físico](#7-mapa-físico)
8. [Mapa lógico](#8-mapa-lógico)
9. [Web](#9-web)
10. [Diseño](#10-diseño)
11. [Mockup](#11-mockup)
12. [Mapa de navegabilidad](#12-mapa-de-navegabilidad)
13. [Base de datos](#13-base-de-datos)
14. [Servicios](#14-servicios)
15. [DNS](#15-dns)
16. [DHCP](#16-dhcp)
17. [Apache](#17-apache)
18. [Firewall](#18-firewall)
19. [Copias de seguridad](#19-copias-de-seguridad)
20. [Conclusiones](#20-conclusiones)
21. [Bibliografía](#21-bibliografía)
22. [Guías de usuario](#22-guías-de-usuario)

---

# 1. Introducción — ¿Qué estamos haciendo?

CleanFlow es una plataforma SaaS diseñada para ayudar a pequeñas y medianas empresas de servicios a gestionar su actividad desde una única aplicación.

El objetivo principal es centralizar en una misma plataforma la gestión de:

* Clientes.
* Trabajadores.
* Servicios.
* Citas.
* Presupuestos.
* Facturas.
* Pagos.
* Inventario.
* Informes.

Además, cada empresa podrá disponer de una página web pública generada automáticamente a partir de la información almacenada en CleanFlow.

---

## 2. Briefing de ideas — Lluvia de ideas

### 2.1. Idea inicial

La idea de **CleanFlow** surge de observar que muchas pequeñas empresas de servicios utilizan diferentes herramientas para gestionar su actividad diaria.

En muchos casos, utilizan una aplicación para las citas, otra para los clientes, otra para las facturas y diferentes documentos para controlar los trabajadores y el inventario.

Por este motivo, pensamos en crear una plataforma que reúna todas estas funciones en un único lugar.

### 2.2. Problemas detectados

Durante la lluvia de ideas identificamos varios problemas habituales:

* Información repartida entre diferentes programas.
* Dificultad para organizar las citas.
* Falta de control sobre los clientes.
* Problemas para controlar los trabajadores.
* Presupuestos realizados manualmente.
* Facturas difíciles de organizar.
* Falta de control del inventario.
* Pérdida de información importante.
* Dificultad para consultar el historial de un cliente.
* Poca automatización de tareas.
* Falta de informes sobre el funcionamiento del negocio.
* Dificultad para mantener actualizada la página web.

### 2.3. Lluvia de ideas

#### 👥 Clientes

* Crear y modificar clientes.
* Guardar sus datos de contacto.
* Consultar su historial.
* Ver sus citas.
* Consultar presupuestos y facturas.
* Añadir notas.
* Registrar incidencias.
* Guardar fotografías relacionadas con los servicios.

#### 👷 Trabajadores

* Crear trabajadores.
* Crear cuentas de acceso.
* Asignar servicios.
* Consultar horarios.
* Gestionar permisos.
* Ver tareas asignadas.
* Registrar el trabajo realizado.

#### 📅 Citas

* Calendario diario, semanal y mensual.
* Crear citas.
* Modificar citas.
* Cancelar citas.
* Asignar trabajadores.
* Asignar servicios.
* Gestionar diferentes estados.
* Enviar avisos y recordatorios.

#### 📄 Presupuestos

* Crear presupuestos.
* Añadir servicios y materiales.
* Aplicar descuentos.
* Calcular impuestos.
* Calcular automáticamente el precio total.
* Enviar presupuestos al cliente.
* Permitir aceptar o rechazar presupuestos.

#### 💰 Facturas y pagos

* Crear facturas.
* Consultar facturas.
* Descargar facturas.
* Controlar pagos.
* Marcar facturas como pagadas o pendientes.
* Consultar el historial de pagos.

#### 📦 Inventario

* Registrar productos.
* Controlar cantidades.
* Registrar proveedores.
* Establecer un stock mínimo.
* Avisar cuando un producto tenga poco stock.
* Consultar movimientos del inventario.

#### 🌐 Página web

Cada empresa podrá disponer de una página web pública generada desde CleanFlow.

La página podrá mostrar:

* Nombre de la empresa.
* Logotipo.
* Descripción.
* Servicios.
* Precios.
* Horarios.
* Ubicación.
* Información de contacto.
* Solicitud de presupuestos.
* Reserva de citas.
* Acceso para clientes.

### 2.4. Ideas de automatización

Para reducir el trabajo manual, planteamos:

* Recordatorios automáticos de citas.
* Avisos de facturas pendientes.
* Avisos de productos con poco stock.
* Generación automática de informes.
* Cálculo automático de presupuestos.
* Generación de facturas.
* Actualización automática de la página web.

### 2.5. Inteligencia Artificial

CleanFlow incorporará herramientas de Inteligencia Artificial para ayudar a las empresas.

El usuario podrá realizar preguntas como:

> ¿Cuántas citas tengo esta semana?

> ¿Qué presupuestos están pendientes?

La IA también podrá:

* Resumir información de la empresa.
* Crear borradores de presupuestos.
* Generar informes.
* Ayudar a redactar mensajes para clientes.
* Analizar información del negocio.
* Detectar posibles necesidades de inventario.
* Responder preguntas frecuentes.
* Funcionar como chatbot en la página web.

### 2.6. Seguridad

La protección de los datos será una parte importante del proyecto.

Se plantean las siguientes medidas:

* Inicio de sesión.
* Contraseñas protegidas.
* Diferentes tipos de usuarios.
* Permisos según el usuario.
* Separación de los datos de cada empresa.
* Protección de la base de datos.
* Conexiones mediante HTTPS.
* Copias de seguridad.
* Registro de determinadas acciones.
* Protección frente a accesos no autorizados.

### 2.7. Sistema multiempresa

CleanFlow estará diseñado para que diferentes empresas puedan utilizar la misma plataforma.

```text
                    CLEANFLOW
                        │
          ┌─────────────┼─────────────┐
          │             │             │
      Empresa A     Empresa B     Empresa C
          │             │             │
       Clientes      Clientes      Clientes
       Citas         Citas         Citas
       Facturas      Facturas      Facturas
```

Cada empresa solamente podrá acceder a sus propios datos.

Por ejemplo, **Empresa A no podrá consultar los clientes de Empresa B**.

### 2.8. Ideas futuras

Durante la lluvia de ideas también surgieron funcionalidades que podrían incorporarse en futuras versiones:

* Aplicación móvil.
* Pagos online.
* Valoraciones de clientes.
* Notificaciones mediante WhatsApp.
* Integración con Google Calendar.
* Predicción de ventas mediante IA.
* Predicción automática del inventario.
* Integración con sistemas contables.
* Aplicación móvil para trabajadores.
* Firma digital de presupuestos y documentos.

Estas funciones podrían desarrollarse posteriormente y no tienen que formar parte de la primera versión.

### 2.9. Selección de la idea final

Después de analizar las diferentes propuestas, decidimos desarrollar **CleanFlow**, una plataforma web de gestión empresarial.

La primera versión se centrará en:

1. Gestión de empresas.
2. Gestión de clientes.
3. Gestión de trabajadores.
4. Gestión de servicios.
5. Gestión de citas.
6. Gestión de presupuestos.
7. Gestión de facturas y pagos.
8. Gestión de inventario.
9. Área privada para clientes.
10. Página web pública para cada empresa.
11. Generación de informes.
12. Integración de Inteligencia Artificial.
13. Sistema multiempresa.
14. Seguridad y separación de datos.

El objetivo final de CleanFlow es ofrecer a las empresas una herramienta centralizada que les permita gestionar su actividad diaria de una forma más organizada, sencilla y eficiente.

---

# 3. Arquitectura del software

La arquitectura de CleanFlow estará dividida principalmente en diferentes componentes:

```text
┌─────────────────────┐
│       USUARIO       │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│      FRONTEND       │
│    Aplicación Web   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│       BACKEND       │
│       API REST      │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│     BASE DE DATOS   │
└─────────────────────┘
```

El frontend será responsable de la interfaz que utilizarán los usuarios.

El backend gestionará la lógica de la aplicación y las peticiones.

La base de datos almacenará la información de las empresas, usuarios, clientes, servicios, citas y demás elementos del sistema.

---

# 4. Tecnologías a utilizar

Las tecnologías definitivas se determinarán durante la fase de diseño técnico.

Se contemplan tecnologías para:

* Desarrollo frontend.
* Desarrollo backend.
* Base de datos.
* Servidor web.
* Control de versiones.
* Diseño.
* Pruebas.
* Despliegue.

### Herramientas

* Git.
* GitHub.
* Visual Studio Code.
* Docker.
* Postman.

---

# 5. Red

La infraestructura de red permitirá conectar los diferentes dispositivos y servicios necesarios para el funcionamiento de CleanFlow.

Se tendrán en cuenta:

* Router.
* Switch.
* Firewall.
* Servidores.
* Ordenadores.
* Puntos de acceso.
* Internet.
* Direccionamiento IP.
* DNS.
* DHCP.

---

# 6. Diagrama de la red

El diagrama de red representará las conexiones entre los diferentes dispositivos.

Ejemplo:

```text
                  INTERNET
                      │
                      ▼
                   ROUTER
                      │
                      ▼
                  FIREWALL
                      │
                      ▼
                    SWITCH
             ┌────────┼────────┐
             │        │        │
             ▼        ▼        ▼
          SERVIDOR   PCs    ACCESS POINT
             │
             ▼
          SERVICIOS
```

---

# 7. Mapa físico

El mapa físico mostrará la ubicación de los dispositivos dentro de la infraestructura.

Se representarán:

* Rack.
* Servidor.
* Router.
* Firewall.
* Switch.
* Ordenadores.
* Access Points.
* Cableado.
* Otros dispositivos de red.

---

# 8. Mapa lógico

El mapa lógico representará cómo está organizada la red a nivel de direccionamiento y servicios.

Se incluirán:

* Direcciones IP.
* Subredes.
* VLAN.
* Puerta de enlace.
* DNS.
* DHCP.
* Servidores.
* Reglas de comunicación.

---

# 9. Web

CleanFlow contará con una aplicación web desde la que los usuarios podrán gestionar sus empresas.

## Funcionalidades

* Gestión de empresas.
* Gestión de clientes.
* Gestión de trabajadores.
* Gestión de servicios.
* Gestión de citas.
* Gestión de presupuestos.
* Gestión de facturas.
* Gestión de pagos.
* Gestión de inventario.
* Informes.
* Área privada para clientes.
* Página pública de cada empresa.

---

# 10. Diseño

El diseño de CleanFlow buscará ofrecer una interfaz:

* Sencilla.
* Moderna.
* Profesional.
* Intuitiva.
* Responsive.

Se definirán:

* Logotipo.
* Colores.
* Tipografías.
* Iconos.
* Botones.
* Formularios.
* Menús.
* Dashboard.
* Diseño móvil.

---

# 11. Mockup

Los mockups representarán visualmente cómo será la aplicación antes de comenzar el desarrollo.

Se diseñarán pantallas como:

* Login.
* Dashboard.
* Clientes.
* Trabajadores.
* Servicios.
* Calendario.
* Presupuestos.
* Facturas.
* Inventario.
* Área del cliente.
* Página pública.

---

# 12. Mapa de navegabilidad

El mapa de navegabilidad mostrará cómo se desplaza el usuario por la aplicación.

```text
LOGIN
  │
  ▼
DASHBOARD
  │
  ├── Empresas
  │
  ├── Clientes
  │
  ├── Trabajadores
  │
  ├── Servicios
  │
  ├── Citas
  │
  ├── Presupuestos
  │
  ├── Facturas
  │
  ├── Inventario
  │
  └── Configuración
```

Los accesos disponibles dependerán del tipo de usuario y de sus permisos.

---

# 13. Base de datos

La base de datos almacenará toda la información necesaria para el funcionamiento de CleanFlow.

Se contemplan entidades como:

```text
USUARIOS
   │
   ▼
EMPRESAS
   │
   ├── CLIENTES
   │
   ├── TRABAJADORES
   │
   ├── SERVICIOS
   │
   ├── CITAS
   │
   ├── PRESUPUESTOS
   │
   ├── FACTURAS
   │
   ├── PAGOS
   │
   ├── INVENTARIO
   │
   └── INFORMES
```

La estructura deberá garantizar que los datos de cada empresa estén correctamente separados.

---

# 14. Servicios

CleanFlow utilizará diferentes servicios para funcionar.

De forma sencilla:

```text
USUARIO
   │
   ▼
WEB
   │
   ▼
APACHE
   │
   ▼
BACKEND
   │
   ▼
BASE DE DATOS
```

Cada servicio tendrá una función concreta dentro de la infraestructura.

En esta sección se explicará:

* Qué hace cada servicio.
* Para qué sirve.
* Dónde está instalado.
* Cómo se comunica con los demás servicios.
* Qué información gestiona.

---

# 15. DNS

El DNS será el encargado de traducir nombres de dominio a direcciones IP.

Ejemplo:

```text
cleanflow.es
      │
      ▼
Dirección IP del servidor
      │
      ▼
Aplicación CleanFlow
```

También se podrán utilizar subdominios para diferentes servicios.

---

# 16. DHCP

DHCP permitirá asignar automáticamente configuraciones de red a los dispositivos.

Podrá proporcionar:

* Dirección IP.
* Máscara de red.
* Puerta de enlace.
* Servidor DNS.

Ejemplo:

```text
DISPOSITIVO
     │
     ▼
   DHCP
     │
     ▼
IP + MÁSCARA + GATEWAY + DNS
```

---

# 17. Apache

Apache será utilizado como servidor web dentro de la infraestructura.

Sus funciones podrán incluir:

* Recibir peticiones HTTP/HTTPS.
* Servir contenido web.
* Gestionar dominios.
* Gestionar Virtual Hosts.
* Trabajar con HTTPS.
* Redirigir peticiones hacia los servicios correspondientes.

Ejemplo:

```text
USUARIO
   │
   ▼
HTTPS
   │
   ▼
APACHE
   │
   ▼
APLICACIÓN
```

---

# 18. Firewall

El firewall será uno de los elementos principales de seguridad de la infraestructura.

Su función será controlar el tráfico de red y permitir o bloquear conexiones según las reglas configuradas.

```text
             INTERNET
                 │
                 ▼
             FIREWALL
             /      \
            /        \
       PERMITIDO    BLOQUEADO
          │             │
          ▼             ▼
       SERVIDOR          ❌
```

Se definirán reglas para controlar:

* Tráfico entrante.
* Tráfico saliente.
* Puertos.
* Servicios.
* Accesos externos.
* Accesos internos.

---

# 19. Copias de seguridad

CleanFlow necesitará un sistema de copias de seguridad para proteger la información.

Se realizarán copias de elementos como:

* Base de datos.
* Archivos.
* Configuración.
* Documentación necesaria.

El sistema deberá contemplar:

* Frecuencia de las copias.
* Ubicación.
* Retención.
* Recuperación.
* Pruebas de restauración.

---

# 20. Conclusiones

En esta sección se analizará el resultado final del proyecto.

Se explicará:

* Si se han cumplido los objetivos.
* Qué funcionalidades se han desarrollado.
* Qué problemas han aparecido.
* Cómo se han solucionado.
* Qué conocimientos se han adquirido.
* Qué mejoras podrían realizarse en el futuro.

---

# 21. Bibliografía

En esta sección se incluirán todas las fuentes utilizadas durante el desarrollo del proyecto.

Ejemplos:

* Documentación oficial.
* Libros.
* Artículos.
* Documentación técnica.
* Tutoriales.
* Recursos educativos.

---

# 22. Guías de usuario

Se crearán diferentes guías dependiendo del tipo de usuario.

## 👨‍💼 Administrador

La guía explicará:

* Inicio de sesión.
* Configuración de la empresa.
* Gestión de clientes.
* Gestión de trabajadores.
* Gestión de servicios.
* Gestión de citas.
* Presupuestos.
* Facturas.
* Pagos.
* Inventario.
* Informes.

## 👷 Trabajador

La guía explicará:

* Inicio de sesión.
* Consulta de servicios.
* Calendario.
* Servicios asignados.
* Actualización de trabajos.
* Creación de informes.
* Subida de fotografías.

## 👤 Cliente

La guía explicará:

* Creación de cuenta.
* Inicio de sesión.
* Consulta de citas.
* Consulta de servicios.
* Presupuestos.
* Facturas.
* Pagos.
* Informes.
* Incidencias.

---

# 🚧 Estado del proyecto

**En desarrollo**

Actualmente CleanFlow se encuentra en fase de planificación y diseño.

---

# 👨‍💻 Autor

**Mario**

Proyecto de desarrollo de una plataforma SaaS de gestión empresarial.
