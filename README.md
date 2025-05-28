# SIDETEAM
Aquí tienes el texto revisado y mejorado para mayor claridad y profesionalismo, manteniendo toda la información original:

¿Qué es SIDE?

SIDE es una plataforma web integral diseñada para la gestión de eventos y la compra de entradas. Este sistema soporta dos tipos principales de usuarios con funcionalidades específicas:

Asistentes a eventos: Pueden explorar eventos, comprar entradas, gestionar sus eventos favoritos y completar transacciones de manera sencilla.
Organizadores de eventos: Tienen la capacidad de crear, editar y gestionar eventos, incluyendo la carga de imágenes y la edición de los detalles específicos de cada evento.
La plataforma SIDE funciona como una moderna Aplicación de Página Única (SPA - Single Page Application). Su arquitectura se basa en un frontend desarrollado con Vue.js que se comunica eficientemente con un backend construido con Node.js/Express a través de una API REST. Toda la información y las transacciones se gestionan y persisten en una base de datos MySQL.

Pila Tecnológica y Componentes Clave:

La plataforma SIDE se apoya en tecnologías modernas de desarrollo web, organizadas en pilas frontend y backend para optimizar su funcionamiento:

Frontend Framework: Vue.js 3.5.13
Propósito: Framework de interfaz de usuario basado en componentes.
Enrutamiento: Vue Router 4.5.0
Propósito: Gestión de la navegación del lado del cliente.
Cliente HTTP: Axios 1.9.0
Propósito: Comunicación con la API del backend.
Frontend Framework: Bootstrap 5.3.5
Propósito: Diseño y componentes responsivos para la interfaz de usuario.
Backend Framework: Express.js
Propósito: Servidor de API REST.
Base de datos: MySQL con controlador MySQL2
Propósito: Persistencia de datos.
Autenticación: JWT (jsonwebtoken + jwt-decode)
Propósito: Autenticación sin estado para usuarios.
Subida de archivos: Multer
Propósito: Procesamiento y almacenamiento de imágenes.
Seguridad: bcryptjs, helmet, cors
Propósito: Hashing de contraseñas y configuración de encabezados de seguridad.
Generación de PDF: pdfkit, puppeteer
Propósito: Generación de facturas en formato PDF.
Componentes del Frontend:

El frontend de Vue.js está estructurado en componentes a nivel de página, cada uno gestionando flujos de trabajo específicos del usuario:

SIDEHome.vue: Página de inicio que presenta un carrusel de eventos y una visualización en cuadrícula de los eventos disponibles.
EventDetail.vue: Muestra información individual de un evento y sirve como punto de entrada para la selección de entradas.
CompraBoletas.vue: Permite la selección de la cantidad de entradas y su adición al carrito de compra.
Cart.vue: Facilita la revisión y modificación de los ítems en el carrito de compra.
FormularioCompra.vue: Gestiona el proceso de pago y la gestión de transacciones.
CrearEventos.vue: Provee el formulario para que los organizadores creen nuevos eventos.
EditarEvento.vue: Ofrece la interfaz para que los organizadores editen eventos existentes.
Estructura de la API del Backend:

El backend de Express.js expone APIs RESTful organizadas por dominio funcional para una gestión clara y eficiente de las solicitudes:

/api/auth: Gestiona la autenticación de usuarios y las sesiones.
/api/events: Permite operaciones CRUD (Crear, Leer, Actualizar, Borrar) sobre eventos, además de búsqueda y filtrado.
/api/carrito: Se encarga de la gestión del carrito de compra.
/api/compra: Procesa las compras y la generación de facturas.
/api/favoritos: Administra los eventos marcados como favoritos por el usuario.
/uploads/*: Servicio para archivos estáticos, específicamente imágenes subidas.
Guía de Configuración y Ejecución Local:

Esta guía proporciona instrucciones detalladas para configurar y ejecutar la plataforma de gestión de eventos SIDE localmente. Cubre los prerrequisitos necesarios, el proceso de instalación, la configuración inicial y los pasos para ejecutar los componentes frontend y backend del sistema.

Para una comprensión más profunda de la arquitectura general del sistema y la pila tecnológica, se recomienda consultar la Arquitectura del sistema. Para documentación detallada de la API, esencial durante el desarrollo, consulte la Referencia de la API.

Prerrequisitos:

Antes de configurar la plataforma SIDE, asegúrese de tener instalados los siguientes componentes en su equipo de desarrollo:

Requisito	Versión Sugerida	Propósito
Node.js	16.x o superior	Entorno de ejecución para frontend y backend.
npm	8.x o superior	Gestor de paquetes.
MySQL	8.x o superior	Servidor de bases de datos.
GitHub	Última versión	Control de versiones.

Aquí tienes el texto revisado y mejorado para mayor claridad y profesionalismo, manteniendo toda la información original:

¿Qué es SIDE?

SIDE es una plataforma web integral diseñada para la gestión de eventos y la compra de entradas. Este sistema soporta dos tipos principales de usuarios con funcionalidades específicas:

Asistentes a eventos: Pueden explorar eventos, comprar entradas, gestionar sus eventos favoritos y completar transacciones de manera sencilla.
Organizadores de eventos: Tienen la capacidad de crear, editar y gestionar eventos, incluyendo la carga de imágenes y la edición de los detalles específicos de cada evento.
La plataforma SIDE funciona como una moderna Aplicación de Página Única (SPA - Single Page Application). Su arquitectura se basa en un frontend desarrollado con Vue.js que se comunica eficientemente con un backend construido con Node.js/Express a través de una API REST. Toda la información y las transacciones se gestionan y persisten en una base de datos MySQL.

Pila Tecnológica y Componentes Clave:

La plataforma SIDE se apoya en tecnologías modernas de desarrollo web, organizadas en pilas frontend y backend para optimizar su funcionamiento:

Frontend Framework: Vue.js 3.5.13
Propósito: Framework de interfaz de usuario basado en componentes.
Enrutamiento: Vue Router 4.5.0
Propósito: Gestión de la navegación del lado del cliente.
Cliente HTTP: Axios 1.9.0
Propósito: Comunicación con la API del backend.
Frontend Framework: Bootstrap 5.3.5
Propósito: Diseño y componentes responsivos para la interfaz de usuario.
Backend Framework: Express.js
Propósito: Servidor de API REST.
Base de datos: MySQL con controlador MySQL2
Propósito: Persistencia de datos.
Autenticación: JWT (jsonwebtoken + jwt-decode)
Propósito: Autenticación sin estado para usuarios.
Subida de archivos: Multer
Propósito: Procesamiento y almacenamiento de imágenes.
Seguridad: bcryptjs, helmet, cors
Propósito: Hashing de contraseñas y configuración de encabezados de seguridad.
Generación de PDF: pdfkit, puppeteer
Propósito: Generación de facturas en formato PDF.
Componentes del Frontend:

El frontend de Vue.js está estructurado en componentes a nivel de página, cada uno gestionando flujos de trabajo específicos del usuario:

SIDEHome.vue: Página de inicio que presenta un carrusel de eventos y una visualización en cuadrícula de los eventos disponibles.
EventDetail.vue: Muestra información individual de un evento y sirve como punto de entrada para la selección de entradas.
CompraBoletas.vue: Permite la selección de la cantidad de entradas y su adición al carrito de compra.
Cart.vue: Facilita la revisión y modificación de los ítems en el carrito de compra.
FormularioCompra.vue: Gestiona el proceso de pago y la gestión de transacciones.
CrearEventos.vue: Provee el formulario para que los organizadores creen nuevos eventos.
EditarEvento.vue: Ofrece la interfaz para que los organizadores editen eventos existentes.
Estructura de la API del Backend:

El backend de Express.js expone APIs RESTful organizadas por dominio funcional para una gestión clara y eficiente de las solicitudes:

/api/auth: Gestiona la autenticación de usuarios y las sesiones.
/api/events: Permite operaciones CRUD (Crear, Leer, Actualizar, Borrar) sobre eventos, además de búsqueda y filtrado.
/api/carrito: Se encarga de la gestión del carrito de compra.
/api/compra: Procesa las compras y la generación de facturas.
/api/favoritos: Administra los eventos marcados como favoritos por el usuario.
/uploads/*: Servicio para archivos estáticos, específicamente imágenes subidas.
Guía de Configuración y Ejecución Local:

Esta guía proporciona instrucciones detalladas para configurar y ejecutar la plataforma de gestión de eventos SIDE localmente. Cubre los prerrequisitos necesarios, el proceso de instalación, la configuración inicial y los pasos para ejecutar los componentes frontend y backend del sistema.

Para una comprensión más profunda de la arquitectura general del sistema y la pila tecnológica, se recomienda consultar la Arquitectura del sistema. Para documentación detallada de la API, esencial durante el desarrollo, consulte la Referencia de la API.

Prerrequisitos:

Antes de configurar la plataforma SIDE, asegúrese de tener instalados los siguientes componentes en su equipo de desarrollo:

Requisito	Versión Sugerida	Propósito
Node.js	16.x o superior	Entorno de ejecución para frontend y backend.
npm	8.x o superior	Gestor de paquetes.
MySQL	8.x o superior	Servidor de bases de datos.
GitHub	Última versión	Control de versiones.

Enlaces de Documentación de SIDE TEAM:

GitDiagram: https://gitdiagram.com/andybd2703/admininfo
DeepWiki: https://deepwiki.com/andybd2703/admininfo/1-overview
Trello: https://trello.com/b/VGFZEcfc/side-team
