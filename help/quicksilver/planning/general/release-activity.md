---
title: Actividad de la versión de Adobe Workfront Planning para 2024
description: Actualmente, las funcionalidades de Adobe Workfront Planning están disponibles para todos los clientes. Debe adquirir una licencia de Workfront Planning, además de una licencia de Workfront, para poder acceder a estas funciones.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 718ed3efd56c532693d26cc067041bedbc71cca0
workflow-type: tm+mt
source-wordcount: '7386'
ht-degree: 9%

---


# Actividad de la versión de Adobe Workfront Planning para 2024

<!--this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page-->

Este artículo enumera las funciones que se lanzaron durante la fase inicial de Workfront Planning en 2024, antes del lanzamiento general de disponibilidad el 28 de agosto de 2024.

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Cronología de la versión de Workfront Planning

<!-- this section is also duplicated in the 2023 release notes article-->

La siguiente tabla muestra la cronología de la versión de Workfront Planning:

| Hora | Versión |
|--------------------|-----------------------------------------|
| De agosto a diciembre de 2023 | Versión beta de Workfront Planning* |
| Enero-agosto de 2024 | Versión anticipada de Workfront Planning* |
| jueves, 28 de agosto de 2024 | Disponibilidad general de Workfront Planning |

*Las fases beta y de lanzamiento anticipado estaban disponibles para un grupo limitado de clientes.

<!--Workfront Planning has temporarily been removed from the Preview and Sandbox environments since January 2024. All features documented in this articles are currently available in Production. -->

## Semana del martes, 26 de agosto de 2024

### Disponibilidad general de Adobe Workfront Planning

Versión de vista previa y producción: 28 de agosto de 2024

Workfront Planning está disponible para todos los clientes que adquirieron una licencia de Workfront Planning, además de su licencia de Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre la compra de Workfront Planning.

Para obtener información sobre las características lanzadas después del 28 de agosto de 2024 en Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

### Workfront Planning ya está disponible en Vista previa

Vista previa: 28 de agosto de 2024

Con el lanzamiento de Workfront Planning a disponibilidad general, las funciones de Workfront Planning ahora se incluyen en el entorno de vista previa.

### Nuevos paquetes de Adobe Workfront Planning y limitaciones de objetos

Vista previa y producción: jueves, 28 de agosto de 2024

Hemos implementado nuevas limitaciones para los objetos de Workfront Planning, de acuerdo con los dos paquetes siguientes:

* Workfront Planning le permite tener:

   * Espacios de trabajo ilimitados

   * 25.000 registros por espacio de trabajo

   * 500 000 registros totales para su instancia

* Workfront Planning Plus le permite tener:

   * Espacios de trabajo ilimitados

   * 500 000 registros por espacio de trabajo

   * 2 millones de registros totales para su instancia.

Para obtener más información, consulte [Resumen de la limitación de objetos de Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).

### Habilitar notificaciones de Workfront Planning para solicitudes de acceso

Vista previa y producción: jueves, 28 de agosto de 2024

Al solicitar acceso a un espacio de trabajo o a una vista, el usuario desde el que se solicita acceso recibe una notificación por correo electrónico sobre la solicitud. Una vez concedida la solicitud, recibirá una notificación por correo electrónico con una confirmación de que se ha aprobado.

Puede acceder a la vista o al espacio de trabajo desde la notificación por correo electrónico, cuando se haya concedido el permiso.  <!--see if they also get an in-app notification-->

>[!NOTE]
>
>Su organización debe incorporarse a la experiencia unificada de Adobe para que los usuarios puedan solicitar y conceder permisos a una vista o a un espacio de trabajo desde una solicitud de permiso.


Para obtener más información, consulte [Solicitar permisos para una vista o un área de trabajo](/help/quicksilver/planning/access/request-permissions.md).

### Definir el formato para los valores de campo de fórmula

Vista previa y producción: jueves, 28 de agosto de 2024

Como administrador de espacio de trabajo, ahora puede definir el formato para los valores mostrados en un campo de fórmula. Puede elegir entre los siguientes formatos:

* Texto de línea única
* Número
* Porcentaje
* Divisa
* Fecha
* Etiquetas

Para obtener más información, consulte la sección &quot;Fórmula&quot; del artículo [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

### Indicadores de presencia en tiempo real en una vista de registros

Vista previa y producción: jueves, 28 de agosto de 2024

Para comprender qué información editan otros usuarios al trabajar en una vista, hemos introducido indicadores de presencia en tiempo real para esta área de la planificación de Workfront.

El campo editado por otro usuario ahora se resalta en la vista de tabla y los avatares de otros usuarios se pueden ver en la esquina superior derecha de todas las vistas.

Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

### Creación de registros enviando una solicitud

Vista previa: 21 de agosto de 2024

Producción: 28 de agosto de 2024

Ahora puede crear registros enviando una solicitud a un formulario de solicitud asociado a un tipo de registro.

En esta actualización se incluyen las siguientes capacidades:

* Como administrador del espacio de trabajo, puede crear un formulario de solicitud y asociarlo a un tipo de registro. Puede compartir un vínculo a este formulario con otras personas, incluidos usuarios externos.

* Cuando los usuarios acceden al formulario, lo completan y envían la solicitud, se crea un registro para el tipo de registro asociado al formulario de solicitud.

* Según la configuración, el formulario de solicitud puede mostrar todos los campos del tipo de registro, excepto los campos de los siguientes tipos:

   * Personas
   * Campos conectados (incluye conexiones con recursos de Experience Manager)
   * Campos de búsqueda conectados
   * Fórmula

Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

### Se puede hacer referencia a los registros de Workfront Planning a través de un campo externo

Vista previa y producción: jueves, 28 de agosto de 2024

Con el lanzamiento de la API pública de Workfront Planning, ahora puede hacer referencia a los registros de Planning en campos externos en formularios personalizados de Workfront.

Para obtener más información, consulte los siguientes artículos:

* [Ejemplos del campo de búsqueda externa en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)
* [Conceptos básicos de la API de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md)

### Menú Nueva configuración en la vista Calendario

Vista previa y producción: jueves, 28 de agosto de 2024

Hay una nueva opción de configuración con la que puede personalizar el aspecto de las barras de registros en la vista Calendario. Puede hacer lo siguiente:

* Actualizar la fecha y la hora de los registros

* Actualizar el estilo de barra

* Cambie el color de las barras de registros o sus agrupaciones para que coincida con una de las siguientes opciones:

   * El color del tipo de registro

   * El color del campo que seleccione

   * El color de la agrupación

   * Sin color (predeterminado)

Al hacer coincidir colores con un campo determinado, solo puede seleccionar campos con opciones codificadas por colores.

Para obtener más información, consulte [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

### El Asistente de IA se ha vuelto a habilitar para Workfront Planning

Vista previa y producción: jueves, 28 de agosto de 2024

El Asistente de IA de Workfront se ha vuelto a habilitar para el área de Workfront Planning.

Para obtener más información sobre el Asistente de IA de Workfront Planning, consulte [Descripción general del Asistente de IA de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

### Funcionalidades de creación de informes para Workfront Planning con el panel de lienzo

Vista previa y producción: jueves, 28 de agosto de 2024

Ahora puede ver la información de Workfront Planning en un informe mediante el panel de lienzo de Workfront. Para obtener más información, consulte [Información general sobre paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md).

## Semana del martes, 19 de agosto de 2024

### Mejoras en la página principal de Workfront Planning

Producción: 20 de agosto de 2024

Vista previa: por determinar

Hemos realizado las siguientes mejoras en la página principal del área de Planning:

* Para los administradores del sistema, los espacios de trabajo que no han creado se han movido de la pestaña &quot;Otros espacios de trabajo&quot; a la pestaña &quot;Espacios de trabajo en los que estoy&quot;. Se ha eliminado la pestaña Mis espacios de trabajo.

* Hemos añadido un menú &quot;Más&quot; para cada tarjeta de espacio de trabajo para facilitar la edición o eliminación del espacio de trabajo de la página principal.

* Hemos añadido los vínculos &quot;Mostrar todo&quot; y &quot;Mostrar menos&quot; para controlar el número de espacios de trabajo que se muestran en la página principal. Cuando hay más de dos filas de tarjetas de espacio de trabajo enumeradas en la página principal, se muestra el vínculo Mostrar todo para permitirle mostrar todos los espacios de trabajo, solo si es necesario.

Para obtener más información, consulte [Edición de espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

### Conectar tipos de registros en varios espacios de trabajo

Producción: 20 de agosto de 2024

Vista previa: por determinar

Ahora puede conectar tipos de registros que pertenezcan a diferentes espacios de trabajo.

Los administradores del sistema ahora pueden configurar tipos de registros para que se conecten desde otros espacios de trabajo. Después de esto, un administrador de espacios de trabajo puede conectarse a estos tipos de registros desde un espacio de trabajo designado o desde todos los espacios de trabajo del sistema.

Antes de esta mejora, sólo se podían conectar tipos de registros que pertenecían al mismo espacio de trabajo, junto con tipos de objetos de otras aplicaciones.

Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

### Visualización de registros conectados en la vista de cronología mediante la función Desglose

Producción: 22 de agosto de 2024

Vista previa: por determinar

Como administrador de vista Cronología, ahora puede ver las relaciones entre los registros conectados mediante el desglose de registros en jerarquías visuales en la vista Cronología.

Por ejemplo, cuando visualiza Campañas en la vista de cronología que están vinculadas a Productos y los Productos tienen asociaciones con Proyectos, ahora puede mostrar Productos en Campañas y Proyectos en sus respectivos Productos.

Esto le permite navegar sin problemas por varios niveles de relaciones, todo dentro de la misma vista de cronología.

No es una jerarquía real (ningún objeto es superior a otro). Es una jerarquía visual que muestra los tipos de registros conectados en una vista de escala de tiempo.

Puede mostrar hasta 5 niveles de tipos de registros en la misma escala de tiempo para un registro.

Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

### Nueva pestaña Conexiones en el área de detalles del registro

Producción: 22 de agosto de 2024

Vista previa: por determinar

Hemos añadido una nueva pestaña en las áreas de vista previa y página del registro. Ahora, al hacer clic en el nombre del registro en una vista, la vista previa del registro y la página del registro muestran las siguientes pestañas:

* **Detalles**: muestra todos los campos de registro, miniaturas y portada. Puede editar los campos en la pestaña Detalles.

* **Conexiones**: muestra todos los tipos de registros u objetos y sus registros u objetos conectados. Puede agregar más registros desde la pestaña Conexiones.

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

### Crear registros, proyectos y portafolios a medida que los conecta

Producción: 22 de agosto de 2024

Vista previa: por determinar

Ahora puede crear registros, proyectos y portafolios a medida que los conecta a registros existentes.

Por ejemplo, si conecta campañas de Workfront Planning con proyectos de Workfront y determina que un proyecto en particular no existe, puede agregarlo como un proyecto nuevo en el campo de registro conectado. A continuación, se agrega el proyecto a Workfront. Los registros recién agregados se agregan a sus respectivas páginas de tipo de registro en la vista de tabla.

En este momento, puede crear lo siguiente al conectar registros:

* Registros de Workfront Planning
* Proyectos Workfront sin plantilla
* Portafolios Workfront

No se pueden crear otros objetos de Workfront o recursos de Experience Manager conectados al conectarlos a un registro.

Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

### Exportar detalles de registro a Word

Producción: 22 de agosto de 2024

Vista previa: por determinar

Ahora puede exportar la página de detalles de un registro o obtener una vista previa de un documento de Word (.docx).

Para obtener más información, vea [Exportar los detalles de un registro](/help/quicksilver/planning/records/export-the-record-page.md).

### Agregar opciones de tipo de conexión

Producción: 22 de agosto de 2024
Vista previa: por determinar

Ahora, al configurar una conexión entre dos tipos de registro, puede definir si los usuarios pueden conectar registros individuales o múltiples en cada uno de los tipos de registro de la conexión. Esto garantiza que pueda diseñar de forma fiable los flujos de trabajo de su equipo y garantizar que los usuarios solo seleccionen la información esperada según sus procesos.

Ahora puede elegir entre los siguientes tipos de conexiones al vincular dos tipos de registros:

* Muchos a muchos. Al seleccionar este tipo de conexión, no es posible cambiarlo después de guardarlo.
* Uno a muchos
* Uno a uno
* Muchos a uno.

Esto permite definir cuántos registros de los tipos de registros conectados pueden conectar los usuarios cuando se establece una conexión.

Los nuevos tipos de conexión no son compatibles con las siguientes conexiones de tipo de registro:

* Al conectar tipos de registros con recursos de Experience Manager
* Cuando conecta tipos de registros que no pertenecen al mismo espacio de trabajo

Para obtener más información, consulte [Información general sobre los tipos de registros de Connect](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Semana del martes, 12 de agosto de 2024

### El Asistente de IA se ha eliminado temporalmente

Producción: 12 de agosto de 2024
Vista previa: por determinar

El asistente de Workfront AI se ha eliminado temporalmente y estará disponible en una fecha posterior. Para obtener más información sobre el Asistente de IA, consulte [Descripción general del Asistente de IA de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

### Conservar el último lapso de tiempo visualizado en la vista de cronología

Producción: 14 de agosto de 2024

Vista previa: por determinar

Ahora, cuando abre una vista de escala de tiempo y se desplaza a una fecha del pasado o del futuro, la fecha que seleccione se conserva después de actualizar la página. Antes de esta mejora, la página mostraba la fecha de hoy.

Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Semana del martes, 29 de julio de 2024

### Ya está disponible la API pública de Adobe Workfront Planning

Producción: 30 de julio de 2024

Vista previa: por determinar

Ya está disponible la API pública de Adobe Workfront Planning.

Para obtener más información, consulte [Conceptos básicos de la API de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

### Insertar y duplicar registros en la vista de tabla

Producción: 1 de agosto de 2024
Vista previa: por determinar

Hemos introducido las siguientes capacidades al trabajar con registros en la vista de tabla:

* Duplicar registros: puede crear rápidamente un registro duplicando uno existente.  Se crea un registro idéntico. Esta capacidad solo está disponible en la vista de tabla.

* Puede insertar un nuevo registro encima o debajo de un registro existente en la vista de tabla. Antes de esta mejora, sólo se agregan registros en la parte inferior de la vista de tabla.

Puede realizar las nuevas funciones desde las siguientes áreas:

* El menú Más de un registro

* La nueva barra de herramientas que se ha agregado a la parte inferior de la página de registro en la vista de tabla

Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md)

### Compartir vistas de Workfront Planning públicamente

Producción: 2 de agosto de 2024

Vista previa: por determinar

Para trabajar sin problemas con partes interesadas externas, ahora puede compartir vistas de registros con otras personas fuera de su organización. Puede compartir un vínculo público a la vista a la que desee que otras personas tengan acceso.

Esta actualización incluye las siguientes funciones:

* Comparta la vista de una página de tipo registro con un vínculo público que caduque en una fecha específica.

* Cualquier persona que no pertenezca a su empresa puede acceder al vínculo compartido durante un tiempo limitado, indicado por la fecha de caducidad. No se requiere iniciar sesión para ver la vista compartida.

* Las personas que acceden a la vista desde el vínculo público no pueden crear otras vistas, editar la vista compartida ni agregar, eliminar o editar la información de registro.

Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

## Semana del martes, 08 de julio de 2024

### Abrir objeto conectado directamente en Workfront

Producción: 9 de julio de 2024

Vista previa: por determinar

Hemos eliminado un paso al acceder a objetos de Workfront conectados a registros de Workfront Planning.

Ahora, al hacer clic en el nombre de un objeto de Workfront desde el registro de Planning conectado a él, se abre la página de objetos de Workfront. Antes de esta mejora, se abría una página de solo lectura de Workfront Planning para el objeto de Workfront conectado desde la que se podía navegar más lejos hasta la página de objetos de Workfront.

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

### Solo los usuarios con licencia Standard o Plan pueden crear vistas

Producción: 11 de julio de 2024

Vista previa: por determinar

Hemos cambiado los tipos de usuarios que pueden crear vistas. Ahora, solo los usuarios con licencia Standard o Plan pueden crear vistas. Todos los demás usuarios tienen acceso de solo vista a las vistas que se comparten con ellos. Antes de esta actualización, los usuarios con licencia Light y Worker podían crear vistas.

Para obtener más información, consulte [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

### Ordenar y agrupar registros por campos de búsqueda con varios valores

Producción: 11 de julio de 2024

Vista previa: por determinar

Ahora puede ordenar y agrupar registros en cualquier vista utilizando campos de búsqueda con varios valores que no están resumidos. Antes de esta mejora, solo se podía ordenar y agrupar los campos de búsqueda resumidos.

Si el campo de búsqueda contiene varios valores, tenga en cuenta lo siguiente:

* La ordenación se realiza según el primer valor

* Los registros se agrupan según cada combinación única de valores de campo

* La cronología se crea en función del primer valor de fecha.

Para obtener más información, consulte los siguientes artículos:

* [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).


## Semana del martes, 24 de junio de 2024

### El Asistente de IA de Workfront (versión beta) ya está disponible para Workfront Planning

El asistente de IA (versión beta) ya está disponible para Workfront Planning.

El asistente de IA funciona en el contexto de la página seleccionada y con su nivel de acceso y permisos para realizar las siguientes acciones: generar, actualizar, eliminar o restaurar registros.

El asistente de IA se encuentra actualmente en fase beta y está disponible para clientes seleccionados. Póngase en contacto con el representante de cuentas para saber si cumple los requisitos para participar en esta fase.

Para obtener más información, consulte [Descripción general del Asistente de IA de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

### Nuevo cuadro de búsqueda al seleccionar un espacio de trabajo o un tipo de registro

Producción: viernes, 27 de junio de 2024

Vista previa: por determinar

Para facilitar la navegación entre espacios de trabajo o entre tipos de registro, ahora puede buscar un espacio de trabajo o un tipo de registro en el menú desplegable situado a la derecha de su nombre en el encabezado de la página.

Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

### Insertar un nuevo campo a la derecha o a la izquierda de uno existente en la vista de tabla

Producción: viernes, 27 de junio de 2024

Vista previa: por determinar

Para mejorar y acelerar su experiencia en la vista de tabla de registros, hemos añadido la capacidad de agregar un nuevo campo entre dos columnas, insertándolo a la derecha o a la izquierda de uno existente.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Semana del martes, 17 de junio de 2024

### Apariencia actualizada de la página Detalles

Producción: martes, 17 de junio de 2024

Vista previa: por determinar

Hemos actualizado el aspecto de la página Detalles de registros. Como parte de esta actualización, se han eliminado los iconos de campo.

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

### Plantillas de Workspace actualizadas

Producción: martes, 17 de junio de 2024

Vista previa: por determinar

Hemos actualizado el aspecto y el campo de las tarjetas de plantilla del espacio de trabajo en Workfront Planning.

Esta actualización incluye las siguientes mejoras:

* Los tipos de registro que pertenecen a cada plantilla se muestran como tarjetas.

* Se ha eliminado la plantilla de administración de marketing. Se han añadido las siguientes plantillas para la administración de marketing y se recomienda utilizar la adecuada en función de la complejidad de los flujos de trabajo:

   * Básico: administración de marketing
   * Administración avanzada de marketing
   * Empresa: administración de marketing

Para obtener más información, consulte los siguientes artículos:

* [Lista de plantillas de área de trabajo](/help/quicksilver/planning/architecture/workspace-templates.md)

* [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md)

### Nueva experiencia al agregar una miniatura o una imagen de portada a un registro

Producción: martes, 17 de junio de 2024

Vista previa: por determinar

Hemos actualizado la experiencia para agregar una miniatura o una imagen de portada a un registro desde la página Detalles. Las mejoras incluyen las siguientes actualizaciones:

* Una imagen en miniatura y una imagen de portada se asignan automáticamente a un registro cuando se crea. Más adelante puede editar estas imágenes.

* Puede añadir una miniatura desde la página Detalles. Antes de esta mejora, solo se podía añadir una miniatura desde la vista de tabla.

* Puede examinar una galería de imágenes para seleccionar una imagen para la portada o para la miniatura de un registro. Antes de esta mejora, solo podía cargar su propio archivo de imagen.

Para obtener más información, consulte los siguientes artículos:

* [Agregar una imagen de portada a un registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)

* [Agregar una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

### Actualizar el título del registro en la página Detalles

Producción: martes, 17 de junio de 2024

Vista previa: por determinar

El título de la página Detalles de un registro muestra el campo principal de un registro. Antes de esta actualización, el título de la página Detalles de un registro mostraba el nombre del registro. Puede editar el título en línea, en la página Detalles, a menos que el campo principal sea de tipo fórmula.

Para obtener más información, consulte los siguientes artículos:

* [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md)

* [Editar registros](/help/quicksilver/planning/records/edit-records.md)

### Adición del vínculo &quot;Mostrar más/Mostrar menos&quot; en los campos de registro conectados

Producción: martes, 17 de junio de 2024

Vista previa: por determinar

Se ha agregado el vínculo &quot;Mostrar más/Mostrar menos&quot; en un campo de registro conectado cuando hay registros que, de lo contrario, se mostrarían en más de dos filas de la página Detalles de un registro.

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

### Rellene automáticamente el campo Nombre con el nombre del registro al conectar tipos de registros

Producción: viernes, 20 de junio de 2024

Vista previa: por determinar

Cuando se crea una conexión entre dos registros o entre un registro y un objeto de otra aplicación, el campo Nombre de la conexión se rellena automáticamente con el nombre del registro conectado. Antes de esta mejora, tenía que agregar manualmente un Nombre para el campo de conexión.

Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

### Definir cómo se muestran los registros conectados en los campos conectados

Producción: viernes, 20 de junio de 2024

Vista previa: por determinar

Ahora puede decidir cómo se muestran los registros conectados en los campos conectados. Al agregar una nueva conexión a un tipo de registro, ahora tiene la opción de mostrar el título del registro conectado y su miniatura o solo la miniatura.

El título de un registro es el nombre del registro o cualquier campo que esté establecido como campo principal en la vista de tabla del tipo de registro.

Esta mejora está disponible para registros conectados desde Workfront Planning y para recursos conectados desde Adobe Experience Manager.

Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

### Solo los usuarios con licencia Standard o Plan pueden tener permisos de administración en los espacios de trabajo (título)

Producción: sábado, 21 de junio de 2024

Vista previa: por determinar

Hemos cambiado los tipos de usuarios que pueden tener acceso completo a los espacios de trabajo. Ahora, solo los usuarios con licencia Estándar o Planificar pueden tener permisos de Administración en los espacios de trabajo. El acceso a los tipos de registro, registros y campos se hereda de un espacio de trabajo. Todos los demás usuarios tienen acceso de solo vista a los espacios de trabajo y sus tipos de objetos. Antes de esta actualización, los usuarios con licencia Light y Worker podían recibir permisos de Contribute en los espacios de trabajo.

Para obtener más información, consulte [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Semana del martes, 10 de junio de 2024

### Referencia de hasta 4 niveles para campos de búsqueda de registros

Producción: jueves, 12 de junio de 2024

Vista previa: por determinar

Ahora puede hacer referencia a campos que están hasta 4 niveles fuera del registro al crear una de las siguientes opciones:

* Filtro

* Ordenar

* Agrupación

* Campo de fórmula

Para obtener más información, consulte los siguientes artículos:

* [Crear campos](/help/quicksilver/planning/fields/create-fields.md)

* [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md)

## Semana del martes, 03 de junio de 2024

### Nueva página de aterrizaje para Workfront Planning

Producción: sábado, 07 de junio de 2024

Vista previa: por determinar

Presentamos una nueva página de aterrizaje para Workfront Planning, después de hacer clic en Planning en el menú principal.

Parte de la información de la página de aterrizaje incluye lo siguiente:

* Área que muestra los espacios de trabajo y los espacios de trabajo compartidos con usted. El propietario del espacio de trabajo se muestra en cada tarjeta de espacio de trabajo.

* Si es administrador de Workfront, se muestran las siguientes pestañas:

   * Mis espacios de trabajo: Muestra únicamente los espacios de trabajo que ha creado.

   * Otros espacios de trabajo: muestra los espacios de trabajo que ha creado o que se han compartido con usted.

* Vínculos a la documentación y actividad de la versión para Workfront Planning

* Tutorial de introducción para Workfront Planning

Para obtener más información, consulte [Información general sobre Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

### Nueva experiencia de incorporación para Workfront Planning

Producción: sábado, 07 de junio de 2024

Vista previa: por determinar

Cuando los nuevos usuarios acceden a Workfront Planning por primera vez, ahora son bienvenidos por un tutorial de incorporación autosolicitado que les guía a través de tareas sencillas y define los conceptos principales de la solución.

Puede recorrer el proceso de incorporación, completar las tareas o minimizarlo y volver a visitarlo más adelante.

## Semana del martes, 27 de mayo de 2024

### Introducción al operador de resumen UNIQUE para los campos de búsqueda

Producción: martes, 27 de mayo de 2024

Vista previa: por determinar

Se ha agregado el operador UNIQUE al agregar valores de campos de búsqueda.

El operador UNIQUE elimina los duplicados de los valores de los campos de búsqueda y solo muestra un valor único. Por ejemplo, si agrega varios registros conectados y los valores de un campo de búsqueda son idénticos entre varios registros, Workfront muestra sólo uno de los valores del campo de búsqueda del registro original.

El operador UNIQUE está disponible para todos los tipos de campo excepto para los siguientes:

* Párrafo
* Personas
* Campo de casilla

Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

### Compartir vistas con todos los miembros de un área de trabajo de forma predeterminada

Producción: viernes, 30 de mayo de 2024

Vista previa: por determinar

Ahora hemos introducido una opción en la que puede dar rápidamente permisos de Vista a una vista a todos los miembros de un espacio de trabajo. Antes de esta mejora, solo los usuarios con los que compartía específicamente una vista podían acceder a la vista. Esta opción no está habilitada de forma predeterminada.

Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

### Se ha actualizado el aspecto del icono Planificación en el menú principal

Producción: viernes, 30 de mayo de 2024

Vista previa: por determinar

Hemos actualizado el aspecto del icono del área de planificación en el menú principal. Para obtener más información, consulte [Descripción general de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

### Cambio del nombre del programa de Workfront Planning

A partir del 30 de mayo de 2024, el programa de planificación de Adobe Workfront pasará de la fase beta a una fase de acceso anticipado. Verá este cambio en la terminología de nuestra documentación.

La fase de acceso anticipado también se limita a unos pocos clientes de Workfront.

El representante de la cuenta le informará si cumple los requisitos para participar en la fase de acceso anticipado.

### Nuevo proceso para eliminar un espacio de trabajo

Producción: viernes, 30 de mayo de 2024

Vista previa: por determinar

Dado que el impacto de la eliminación de un espacio de trabajo puede ser significativo, hemos añadido un paso adicional para confirmar la eliminación. Ahora es necesario que los usuarios escriban &quot;eliminar&quot; para poder completar la eliminación permanente de un espacio de trabajo.

Los espacios de trabajo eliminados y su información no se pueden recuperar.

Para obtener más información, consulte [Eliminar espacios de trabajo](/help/quicksilver/planning/architecture/delete-workspaces.md).

### Los campos de fecha de búsqueda ahora están disponibles en la vista de cronología

Producción: sábado, 31 de mayo de 2024

Vista previa: por determinar

Ahora puede establecer las Fechas de inicio y finalización de la vista de escala de tiempo en un campo de búsqueda a partir de un registro conectado o un tipo de objeto.

Para obtener más información sobre cómo crear vistas, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

## Semana del martes, 20 de mayo de 2024

### Conexión de registros de Workfront Planning desde objetos de Workfront mediante la sección Planning

Producción: viernes, 23 de mayo de 2024

Vista previa: por determinar

Hemos agregado una nueva sección de planificación en el panel izquierdo de proyectos, portafolios y programas de Workfront. La nueva sección Planning muestra los registros de Workfront Planning conectados al objeto Workfront.

Las siguientes acciones están disponibles en la sección Planificación de Workfront:

* Ver registros de Planning conectados

* Conectar registros de Workfront Planning al objeto de Workfront

* Desconectar registros

* Abra el cuadro de vista previa de detalles o la página para ver más información sobre los registros conectados

Para obtener más información, consulte [Administrar conexiones de registro desde objetos de Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

## Semana del martes, 13 de mayo de 2024

### Actualizaciones en tiempo real en la vista de cronología después de editar registros

Producción: miércoles, 14 de mayo de 2024

Vista previa: pendiente de determinación.

Cuando un usuario actualiza la información de un registro, otros usuarios pueden ver la información actualizada en la vista de escala de tiempo del registro en tiempo real. Esto garantiza que todos los usuarios vean la información actualizada al mismo tiempo, en sincronización con el momento en que se producen los cambios.

### Agregar registro desde el encabezado de vista

Producción: miércoles, 14 de mayo de 2024

Vista previa: por determinar

Hemos añadido el botón &quot;Nuevo registro&quot; en el encabezado de una página de tipo de registro. Ahora puede crear registros desde cualquier vista. Antes de esta mejora, sólo se podían crear registros desde la vista de tabla.

Para obtener más información, consulte [Creación de registros](/help/quicksilver/planning/records/create-records.md).


### Nueva advertencia sobre la visibilidad de los objetos al conectar registros

Producción: jueves, 15 de mayo de 2024

Vista previa: por determinar

Al crear conexiones a tipos de objeto fuera de Workfront Planning, ahora se le notifica que cualquier persona que trabaje en el espacio de trabajo actual tendrá visibilidad de todos los objetos vinculados y sus campos de búsqueda, independientemente de sus permisos y niveles de acceso en la otra aplicación.

Por ejemplo, si vincula proyectos de campañas de Workfront Planning, todas las personas con acceso a Ver la campaña también tendrán acceso para ver los proyectos vinculados y la información de sus campos de búsqueda, incluso cuando no tengan permisos para los proyectos vinculados o acceso a proyectos en general. Puede obtener acceso a los registros de Planning cuando reciba permisos para espacios de trabajo.

Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

### Agregar secciones a las páginas de vista previa y detalles del registro

Producción: jueves, 15 de mayo de 2024

Vista previa: por determinar

Para organizar mejor la información en la página del registro para una legibilidad y navegación más eficientes, hemos introducido secciones en la página del registro. Los títulos de las secciones sirven como encabezados que organizan los campos en distintas categorías. Las secciones son totalmente personalizables y se pueden expandir o contraer, si es necesario.

Para obtener más información, vea [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).

### Actualizaciones en tiempo real de los cambios de configuración de los campos

Producción: viernes, 16 de mayo de 2024

Vista previa: por determinar

Cuando un usuario cambia cualquier configuración de campo (nombre, descripción, lista de opciones, etc.) en un tipo de registro, otros usuarios ven esos cambios en tiempo real. Esto garantiza que todos vean los campos correctos y su información al mismo tiempo.

>[!WARNING]
>
>Cuando cambian las expresiones de fórmula, o se añaden o eliminan opciones de un campo de tipo de selección, se perderán datos de los registros que ya tienen información almacenada en los campos cuya configuración se modifica.
>
>No se muestra ninguna advertencia ni indicación de que esta pérdida de datos pueda producirse al cambiar la configuración de los campos.
>
>No se muestra ninguna notificación a otros usuarios de que la configuración del campo haya cambiado.

Para obtener más información, consulte [Editar configuración de campo](/help/quicksilver/planning/fields/edit-fields.md).

## Semana del martes, 06 de mayo de 2024

### Apariencia actualizada de las tarjetas de tipo de registro en un espacio de trabajo

Producción: miércoles, 07 de mayo de 2024

Vista previa: por determinar

Hemos actualizado el aspecto de las tarjetas de tipo de registro al verlas en espacios de trabajo. Las actualizaciones incluyen:

* Eliminación del número de campos y conexiones para cada tipo de registro

* Adición de la descripción del tipo de registro

Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

### Activación de las notificaciones de Workfront Planning para clientes de Adobe Unified Experience

Producción: jueves, 08 de mayo de 2024

Vista previa: pendiente de determinación

Si es cliente de Adobe Unified Experience y alguien le agrega a un comentario en la página de registro, recibirá una notificación sobre el comentario en la aplicación y por correo electrónico. Puede administrar las preferencias de notificación en el área Preferencias del perfil de Adobe Experience Cloud. Para obtener más información, consulte [Preferencias y notificaciones de la cuenta](https://experienceleague.adobe.com/es/docs/core-services/interface/features/account-preferences).

Para obtener más información acerca de las notificaciones de planificación de Workfront, vea [Notificaciones de planificación de Adobe Workfront: Índice de artículos](/help/quicksilver/planning/notifications/notifications-information.md).


## Semana del lunes, 29 de abril de 2029

### Actualizaciones en tiempo real en el cuadro de detalles de registro y en la página después de editar registros en la vista de tabla

Producción: viernes, 02 de mayo de 2024

Vista previa: por determinar

Cuando un usuario actualiza la información de un registro en la vista de tabla, otros usuarios pueden ver la información actualizada en el cuadro de detalles del registro (dentro de una vista) o en la página en tiempo real. Esto garantiza que todos los usuarios vean la información actualizada al mismo tiempo, en sincronización con el momento en que se producen los cambios.

Para obtener información sobre la edición de registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

### Actualizaciones en tiempo real en la vista de calendario después de editar registros

Producción: sábado, 03 de mayo de 2024

Vista previa: pendiente de determinación.

Cuando un usuario actualiza la información de un registro, otros usuarios pueden ver la información actualizada en la vista de calendario del registro en tiempo real. Esto garantiza que todos los usuarios vean la información actualizada al mismo tiempo, en sincronización con el momento en que se producen los cambios.

## Semana del martes, 22 de abril de 2024

### Flujo de trabajo actualizado al editar un espacio de trabajo o un tipo de registro

Producción: 23 de abril de 2024

Vista previa: por determinar

Hemos actualizado el aspecto de los cuadros Editar espacio de trabajo y Editar tipo de registro.

Al editar un espacio de trabajo o un tipo de registro, ahora puede definir un nombre, una descripción y asignarles un color y un icono.

Para obtener más información, consulte los siguientes artículos:

* [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md)

* [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

## Semana del martes, 08 de abril de 2024

### Copiar el contenido de una celda y pegarlo en varias celdas seleccionadas

Producción: 10 de abril de 2024

Vista previa: por determinar

Ahora puede copiar el contenido de una celda en la vista de tabla y pegarlo en varias celdas seleccionadas. También puede copiar información de fuentes externas y pegarla en las celdas de la vista de tabla.

Esta funcionalidad es compatible con todos los tipos de campo excepto para los campos calculados.

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Semana del martes, 01 de abril de 2024

### Reordenar los campos en páginas de registro

Producción: 4 de abril de 2024

Vista previa: por determinar

Como administrador de Workspace, ahora puede reordenar los campos enumerados en la página de registro o en la vista previa. Al actualizar el orden de los campos, cambia el orden de los campos en todos los registros del mismo tipo, para todos los que ven la página de registros o la vista previa de registros.

Para obtener más información, consulte [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).


### Agregar imagen de portada a las páginas de registro

Producción: 4 de abril de 2024

Vista previa: por determinar

A medida que administra páginas de registro, ahora puede agregar, cambiar la posición y reemplazar una imagen de portada en una página de registro o vista previa para enriquecer la presentación del registro y la participación de las partes interesadas. Las imágenes de portada son visibles para todos los usuarios que ven los registros.

Para obtener más información, consulte [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).

## Semana del 25 de marzo de 2024

### Nueva organización flexible del tipo de registro para espacios de trabajo

Producción: 25 de marzo de 2024

Vista previa: por determinar

Para crear eficiencia al configurar espacios de trabajo, hemos modificado la forma de organizar los tipos de registros en un espacio de trabajo. Algunas de las mejoras incluyen las siguientes:

* Cree hasta 50 secciones de tipos de registro en cada espacio de trabajo. Las secciones Tipos de registros operativos y Taxonomías existentes permanecen en los espacios de trabajo existentes.

* Personalice completamente todos los nuevos espacios de trabajo y sus nuevas secciones para reflejar los procesos y las necesidades de la organización.

* Mueva de forma dinámica tipos de registros dentro de un espacio de trabajo arrastrándolos y soltándolos donde deban estar, incluso en diferentes secciones.

Para obtener más información, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

### Duplicar vistas

Producción: 25 de marzo de 2024

Vista previa: por determinar

Para ahorrarle tiempo y mantener la coherencia, ahora puede duplicar una vista existente a la que tiene permisos de acceso.

Al duplicar una vista, se crea una vista idéntica, con los mismos filtros, criterios de ordenación y agrupaciones. La duplicación de una vista no mantiene los permisos de la vista original.

Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

### Se ha cambiado el nombre del área Maestro en el menú principal a Planificación

Producción: 27 de marzo de 2024

Vista previa: por determinar

Hemos cambiado el nombre del área Maestro en el menú principal a Planificación.

Para obtener una descripción general de Adobe Workfront Planning, consulte [Descripción general de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

### Nueva experiencia al eliminar un tipo de registro

Producción: 27 de marzo de 2024

Vista previa: por determinar

Hemos rediseñado el cuadro de confirmación al eliminar un tipo de registro. La eliminación de un tipo de registro es impactante, ya que también elimina todos los registros, sus campos, la información de los campos, así como las vistas asociadas con el tipo de registro. Los tipos de registros eliminados y su información eliminada no se pueden recuperar.

Por este motivo, queremos asegurarnos de que la intención del usuario sea precisa al eliminar un tipo de registro, por lo que hemos introducido un paso adicional para confirmar la eliminación. Para obtener más información, vea [Eliminar tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md).

## Semana del 18 de marzo de 2024

### Filtros disponibles en la vista de calendario

Producción: 19 de marzo de 2024

Vista previa: por determinar

Ahora puede filtrar la información en la vista de calendario. Para obtener más información, consulte [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

### Vista previa con detalles de registro agregados a las vistas de calendario y cronología

Producción: 19 de marzo de 2024

Vista previa: por determinar

Ahora puede acceder a la vista previa con detalles de registro desde las vistas de cronología y calendario. Puede editar registros en el cuadro de vista previa del registro, dentro de las vistas de calendario y cronología.

Desde la vista previa del registro, puede abrir la página del registro en una nueva pestaña del explorador.

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

### La importación de Excel del tipo de registro se ha eliminado temporalmente

Producción: 21 de marzo de 2024

Vista previa: por determinar

Se está eliminando temporalmente la importación de tipos de registros mediante un archivo de Excel o CSV. Esta funcionalidad estará disponible más adelante.

## Semana del 11 de marzo de 2024

### Los detalles de registro de un vistazo se muestran en la vista de tabla

Producción: 14 de marzo de 2024

Vista previa: por determinar

Para facilitar la visualización de información adicional sobre los registros al utilizar la vista de tabla, hemos introducido una nueva vista previa de detalles que muestra una vista rápida de los detalles del registro. A continuación se muestra parte de la información incluida en la vista previa de registros:

* Detalles de registro relevantes de un vistazo

* Capacidad para modificar la información de registro

* Un vínculo para abrir la página del registro

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

### Nuevo diseño con pestañas para vistas de registros

Producción: 14 de marzo de 2024

Vista previa: por determinar

Para una mejor navegación y facilidad de uso, hemos rediseñado la visualización de las vistas de registros. Ahora, las vistas se muestran horizontalmente, como pestañas en la página de tipo de registro, para que pueda navegar fácilmente por ellas. Antes de esta mejora, las vistas se mostraban en el menú desplegable Ver.

Las vistas se muestran cronológicamente por fecha añadida de izquierda a derecha. Las vistas compartidas también se muestran en orden cronológico de cuándo se compartieron.

Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

### Diseño dinámico de una vista de registros

Producción: 14 de marzo de 2024
Vista previa: por determinar

Hemos actualizado el aspecto de las vistas en la página de tipo de registro. Las nuevas vistas responden de forma dinámica y se ajustan rápidamente al tamaño de la pantalla. Las etiquetas de opciones de la barra de herramientas están ocultas en pantallas más pequeñas para facilitar su uso.

Para obtener más información, consulte los siguientes artículos:

* [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Administrar vista de escala de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

### Permitir que los administradores del sistema administren todas las vistas compartidas

Producción: 14 de marzo de 2024

Vista previa: por determinar

Para ser coherente con todas las demás áreas del sistema y poder mantener y controlar cualquier vista disponible para usted como administrador del sistema, ahora tiene permisos de Administración para cualquier vista compartida con usted en la página de tipo de registro. Antes de esta mejora, los creadores de vistas podrían haberle concedido permisos para Ver o Administrar la vista. Ahora, si la vista se comparte con usted y usted es administrador del sistema, tendrá permisos de administración en la vista de forma predeterminada.

Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

### Página no autorizada al compartir una vista sin permisos

Producción: 14 de marzo de 2024

Vista previa: por determinar

Cuando un usuario recibe un vínculo a un tipo de registro y tiene acceso al espacio de trabajo pero no a la vista compartida en el vínculo, se muestra una página que le notifica que no está autorizado para ver el tipo de registro.

Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).


### Nueva etiqueta para administradores de sistemas en cuadros de diálogo de uso compartido

Producción: 14 de marzo de 2024

Vista previa: por determinar

Ahora se muestra la etiqueta &quot;Admin&quot; junto al nombre del administrador del sistema en el cuadro de diálogo de uso compartido al compartir una vista o un espacio de trabajo.

Para obtener más información, vea [Información general sobre los permisos de uso compartido](/help/quicksilver/planning/access/sharing-permissions-overview.md).

### Página no autorizada al compartir una vista sin permisos

Producción: 14 de marzo de 2024

Vista previa: por determinar

Cuando un usuario recibe un vínculo a un tipo de registro y tiene acceso al espacio de trabajo pero no a la vista compartida en el vínculo, se muestra una página que le notifica que no está autorizado para ver el tipo de registro.

Debe compartir vistas además de compartir espacios de trabajo para que otros usuarios tengan acceso a la misma página de tipo de registro que comparte con un vínculo.

Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

## Semana del 4 de marzo de 2024

### Cambiar el alto de fila en la vista de tabla

Producción: 7 de marzo de 2024

Vista previa: por determinar

Ahora tiene la opción de modificar el alto de una fila al mostrar registros en la vista de tabla.

Puede actualizar el alto de fila a uno de los siguientes tamaños:

* Baja
* Media
* Alto.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

### Nueva vista de calendario para registros

Producción: 7 de marzo de 2024

Vista previa: por determinar

Ahora puede mostrar registros en una vista de calendario. Debe tener al menos dos campos de fecha en un tipo de registro para poder crear la vista de calendario.

Para obtener más información, consulte [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Semana del 26 de febrero de 2024

### Filtrar, ordenar y agrupar por registros conectados o campos de búsqueda

Producción: 28 de febrero de 2024

Vista previa: por determinar

Ahora puede filtrar, ordenar y agrupar por registros conectados o sus campos de búsqueda. Esta mejora le ayudará a organizar y visualizar de forma eficaz los datos tanto en las vistas de tabla como de cronología.

No puede filtrar, ordenar ni agrupar por campos de búsqueda que permitan conexiones con varios registros.

Para obtener más información, vea [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md) y [Administrar la vista de escala de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Semana del 5 de febrero de 2024

### Modificación de permisos según los tipos de licencia

Producción: 6 de febrero de 2024

Vista previa: por determinar

Hemos modificado los niveles de permisos para tener en cuenta los tipos de licencia de los usuarios. Antes de esta mejora, no había diferencias en los permisos del espacio de trabajo en función de los tipos de licencia de los usuarios.

Los siguientes son los niveles más altos de permisos que los usuarios pueden recibir según el tipo de licencia del usuario:

* Los usuarios con una licencia de planificación (o licencia estándar, en el nuevo modelo de licencia) pueden crear y administrar espacios de trabajo, tipos de registros y registros.

* Los usuarios con una licencia de trabajo (o Ligera, en el nuevo modelo de licencia) pueden ver y contribuir a un espacio de trabajo compartido con ellos, así como los tipos de registro y registros de ese espacio de trabajo.  Los usuarios con licencia de trabajo (o básica) también pueden crear, editar y eliminar registros en espacios de trabajo en los que tengan acceso de tipo Contribuir.

* Los usuarios con una licencia de revisión o solicitante (o colaborador, en el nuevo modelo de licencia) solo pueden ver los espacios de trabajo compartidos con ellos, así como los tipos de registro y registros de dichos espacios de trabajo. No pueden crear, editar ni eliminar tipos de registros o registros.

Para obtener información acerca del nuevo modelo de licencia, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información acerca de la conexión entre el tipo de licencia y los permisos en las funciones de Planning, consulte [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Nueva apariencia de la barra de herramientas Texto enriquecido para campos de registro

Producción: 7 de febrero de 2024

Vista previa: por determinar

Hemos actualizado el aspecto de la barra de herramientas Texto enriquecido al editar un campo de tipo Párrafo.

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

### Experiencia mejorada al editar los campos Selección única, Selección múltiple, Personas y al añadir objetos conectados

Producción: 8 de febrero de 2024

Vista previa: por determinar

Hemos rediseñado y mejorado la experiencia de agregar opciones u objetos para los siguientes tipos de campo:

* Selección única
* Selección múltiple
* Personas
* Campos de registro conectados (al conectar tipos de registros de capacidad de planificación u objetos de Workfront)

Con la nueva mejora, aparece primero un cuadro más pequeño y adaptable.

Para los campos conectados, puede agregarlos realizando una de las siguientes acciones:

* Agregue objetos al campo conectado buscándolos y seleccionándolos en una lista de la vista de tabla, mientras edita en línea el campo
* Haga clic en esta opción para abrir el cuadro Conectar objetos, que es más grande y donde puede ver todos los nombres de elementos, además de obtener más información sobre los elementos.

Las mejoras ahora están disponibles al actualizar campos en la vista de tabla de un tipo de registro.

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Semana del 29 de enero de 2024

### Uso compartido mejorado de vistas y espacios de trabajo

Producción: 30 de enero de 2024

Vista previa: por determinar

Hemos mejorado la experiencia de uso compartido para espacios de trabajo y vistas con las siguientes mejoras:

* Para aclarar qué puede hacer cada nivel de permiso cuando comparte un espacio de trabajo y una vista, se han agregado detalles para cada nivel de permisos.

* Ahora puede copiar un vínculo a un espacio de trabajo o verlo y compartirlo con otros. Los usuarios deben tener al menos permisos de visualización en el espacio de trabajo o en la vista para poder acceder a ellos desde el vínculo copiado.

Para obtener más información, consulte los siguientes artículos:

* [Compartir espacios de trabajo](/help/quicksilver/planning/access/share-workspaces.md)
* [Compartir vistas](/help/quicksilver/planning/access/share-views.md)

### Añadir miniaturas a los registros

Producción: 1 de febrero de 2024

Vista previa: por determinar

Ahora puede agregar miniaturas individuales a cada registro para distinguirlas en una vista. En la vista de tabla, puede agregar como miniaturas archivos de imagen guardados anteriormente en el equipo. Las miniaturas pueden ser únicas para cada registro y mostrarse tanto en la tabla como en las vistas de cronología de la página de tipo de registro.

Para obtener más información, consulte [Añadir una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Quitar tarjetas de tipo de registro conectadas

Producción: 1 de febrero de 2024

Vista previa: por determinar

Para evitar confusiones y simplificar la administración de los espacios de trabajo, se han eliminado las tarjetas de tipo de registro generadas automáticamente y de solo lectura para los objetos externos conectados de un espacio de trabajo.

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Semana del 22 de enero de 2024

### La nueva sección Historial muestra la actividad del sistema para los registros de capacidades de planificación

Producción: 25 de enero de 2024

Vista previa: por determinar

Para mejorar las capacidades de auditoría, hemos introducido una nueva sección en el panel derecho de un registro en la que puede revisar los cambios realizados en el registro registrado por el sistema.

La siguiente información se registra en la nueva sección Historial:

* Cualquier cambio de campo

* Los valores antiguos y nuevos de los campos, cuando cambian los valores

* El nombre completo del usuario que ha realizado el cambio

* Una marca de fecha y hora de cuando se produjo el cambio.

Para obtener más información, consulte [Información general sobre la sección Historial](/help/quicksilver/planning/records/history-section-overview.md).

### Nueva etiqueta para nuevo vínculo de registro

Producción: 25 de enero de 2024

Vista previa: por determinar

Para crear coherencia al crear registros, se ha vuelto a etiquetar el vínculo + Nuevo para crear registros como &quot;+ Nuevo registro&quot;.  Antes de esta actualización, el vínculo contenía el nombre del tipo de registro. El nuevo vínculo ya está disponible al crear registros operativos y de taxonomía. Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

## Semana del 8 de enero de 2024

### Las capacidades de Planning se eliminan de los entornos Vista previa y Zona protegida

Vista previa y zona protegida: 11 de enero de 2024

Las funcionalidades de Adobe Workfront Planning se han eliminado temporalmente de los entornos de Vista previa y Zona protegida. Se añadirán a estos entornos en una fecha posterior, que se comunicará en las notas de la versión de la actividad.

### Permisos de capacidades de Planning para espacios de trabajo y vistas

Producción: 11 de enero de 2024

Vista previa: por determinar

Ahora puede compartir un espacio de trabajo o una vista con usuarios y grupos. Puede establecer sus permisos en diferentes niveles, según la información que necesiten ver o editar.

Cuando comparte un espacio de trabajo, los usuarios tienen permisos para los tipos de registro, los registros y los campos de ese espacio.

Cuando comparte un área de trabajo, los usuarios no reciben permisos de uso compartido en las vistas asociadas con los tipos de registro del área de trabajo. Debe conceder permisos independientes a las vistas.

A continuación se muestran los niveles de permisos para espacios de trabajo:

* Ver: Los usuarios pueden ver los espacios de trabajo que se comparten con ellos. También pueden ver tipos de registros y registros del espacio de trabajo compartido.

* Contribute: los usuarios pueden crear, editar o eliminar registros en el espacio de trabajo compartido con ellos.  No pueden crear ni editar tipos de registros o espacios de trabajo que se comparten con ellos.

* Administrar: los usuarios pueden crear, editar y eliminar espacios de trabajo, tipos de registro, registros y campos en espacios de trabajo que se comparten con ellos.

A continuación se indican los niveles de permisos para las vistas de registros:

* Vista: Los usuarios pueden seleccionar la vista en el menú desplegable Ver de una página de tipo de registro.
* Administrar: los usuarios pueden editar, compartir y eliminar la vista.

Para obtener más información, consulte [Información general sobre el acceso a Adobe Planning](/help/quicksilver/planning/access/access-overview.md) y [Información general sobre los permisos de uso compartido en las funciones de Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

### Nuevo tipo de campo Fórmula

Producción: 11 de enero de 2024

Vista previa: por determinar

Ahora puede agregar un campo de tipo fórmula a un tipo de registro.

Los campos de fórmula generan un nuevo valor utilizando los valores existentes de otros campos en un tipo de registro y una función que indica cómo se deben calcular los valores existentes.

No se pueden utilizar campos de búsqueda de tipos de registros vinculados en un cálculo de fórmula. Esta funcionalidad estará disponible más adelante.

Para obtener más información, vea [Información general sobre los campos de fórmula](/help/quicksilver/planning/fields/formula-fields.md).

### Acciones Deshacer/ Rehacer al administrar registros en la vista de tabla

Producción: 11 de enero de 2024

Vista previa: por determinar

Ahora puede deshacer o rehacer los cambios al realizar las siguientes acciones en la vista de tabla:

* Copia/pegado de datos
* Editar registro
* Añadir registro
* Eliminar registro

Puede utilizar las siguientes pulsaciones de teclas para deshacer o rehacer acciones:

* Deshacer: CTRL/CMD + Z
* Rehacer: CTRL/CMD + Mayús + Z

Para obtener más información, consulte los siguientes artículos:

* [Editar registros](/help/quicksilver/planning/records/edit-records.md)

* [Eliminar registros](/help/quicksilver/planning/records/delete-records.md)

* [Crear registros](/help/quicksilver/planning/records/create-records.md)


