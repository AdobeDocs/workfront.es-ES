---
content-type: release-notes
title: Actividad de la versión del tercer trimestre de 2026 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el tercer trimestre de 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 12552dfefc58a664c278598496097f1b30d3cf0e
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 2%

---

# Actividad de la versión del tercer trimestre de 2026 para Adobe Workfront Planning

<!--take the next sentence out when we start listing features-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del tercer trimestre de 2026.

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).



<!--

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## API de Workfront Planning versión 2

>[!NOTE]
>
>Disponible para todos los clientes: 28 de mayo de 2026>[!BADGE horario inadecuado]{type=Neutral}

La versión 2 de la API de Workfront Planning ya está disponible y amplía considerablemente las capacidades de la versión 1.

En la versión 2 de se incluyen las siguientes mejoras:

* Cree, actualice y elimine espacios de trabajo, tipos de registro y campos mediante programación.

* Administrar registros por completo.
* Mejoras en la estructura de la URL, control de errores, paginación, filtrado y permisos.
* Incluye actualizaciones parciales mediante PATCH
* Incluye operaciones de registro en masa.

La versión 1 sigue disponible, aunque le recomendamos que cambie a la versión 2.

>[!NOTE]
>
>El conector de Workfront Planning para Fusion no se ha actualizado a la versión 2 de la API y seguirá utilizando la versión 1 hasta nuevo aviso.

Para obtener más información, consulte [Conceptos básicos de la API de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

Para ver las especificaciones de la API de Workfront Planning, consulte la [documentación para desarrolladores de la API de Workfront Planning](https://developer.adobe.com/wf-planning/).

## Conceder permisos a registros

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Ahora puede ajustar permisos de registro individuales para controlar quién puede administrarlos dentro de un tipo de registro.

Los usuarios heredan los permisos de registro del espacio de trabajo y el tipo de registro de forma predeterminada. Para conceder sólo a usuarios seleccionados con permisos de tipo de registro y permisos de administración sólo a determinados registros, puede deshabilitar los permisos heredados en registros seleccionados y conceder sólo a esos usuarios acceso de administración a esos registros. Puede ajustar los permisos para un registro o para varios registros al mismo tiempo, de forma masiva.

Puede otorgar a los usuarios los siguientes niveles de permisos:

* Ver
* Administrar

>[!NOTE]
>
>* Los permisos de nivel de registro de un usuario no pueden superar sus permisos de tipo de registro. Por ejemplo, a un usuario con acceso de Vista a un tipo de registro no se le puede otorgar acceso de Administración a registros individuales de ese tipo.
>* En este momento no se pueden quitar los permisos de un usuario de un registro. Cualquier usuario con al menos acceso de Vista al tipo de registro puede ver todos los registros de ese tipo.

Para obtener más información, consulte [Compartir registros](/help/quicksilver/planning/access/share-records.md).

## Adición optimizada del tipo de registro global

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Para reducir los clics y ayudarle a encontrar rápidamente los tipos de registros que necesita, hemos mejorado la experiencia de agregar registros para que sea más rápido e intuitivo al agregar tipos de registros globales a otro espacio de trabajo.

Cuando decida agregar un registro de tipos de registros existentes, ahora verá inmediatamente una lista de todos los tipos de registros globales disponibles.

Puede seleccionar y agregar uno o varios tipos de registros globales al mismo tiempo directamente desde esta pantalla.

Para obtener más información, vea [Agregar tipos de registros existentes desde otro área de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).


## Sincronización de metadatos de Planning a AEM Assets

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de la producción: 28 de mayo de 2026>Producción para todos: 28 de mayo de 2026>[!BADGE Fuera de horario]{type=Neutral}

Para mejorar la integridad de los datos, hemos lanzado una sincronización de metadatos fluida entre los tipos de registros de GenStudio for Performance Marketing y los AEM Assets cuando los AEM Assets están vinculados a tipos de registros de GenStudio en Workfront Planning.

Se pueden conectar los siguientes tipos de registros de GenStudio for Performance Marketing a los AEM Assets: Campaign, Product, Persona, Region y Channel.

La información agregada a un tipo de registro de GenStudio en Workfront Planning se muestra en una pestaña de Campaign independiente de un recurso de AEM en AEM. La información sobre el producto, el persona, la región y el canal de esa campaña también se muestra en esa pestaña en modo de solo lectura.

Con esta versión, los metadatos clave son coherentes en ambas plataformas y reflejan las actualizaciones en tiempo casi real, lo que reduce la reconciliación manual.

Para obtener más información, consulte [Administrar el espacio de trabajo de GenStudio en Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).

## Sincronizar metadatos de Planning a fragmentos de contenido de AEM

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de la producción: 28 de mayo de 2026>Producción para todos: 28 de mayo de 2026>[!BADGE Fuera de horario]{type=Neutral}

Para mejorar la integridad de los datos, hemos lanzado una sincronización de metadatos fluida entre los tipos de registros de Planning en el espacio de trabajo de GenStudio y los fragmentos de contenido de AEM cuando los fragmentos de contenido están vinculados a campañas de GenStudio for Performance Marketing.

La información de la campaña de GenStudio ahora se muestra en la pestaña Metadatos de un fragmento de contenido en AEM.  La información sobre el producto, el persona, la región y el canal de esa campaña también se muestra en esa pestaña en modo de solo lectura.

Con esta versión, los metadatos clave son coherentes en ambas plataformas y reflejan las actualizaciones en tiempo casi real, lo que reduce la reconciliación manual.

Para obtener más información, consulte [Administrar el espacio de trabajo de GenStudio en Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).


## Actualizaciones de vista de lista

>[!NOTE]
>
>Vista previa: 27 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Se han actualizado varios tipos de campos en la vista de lista para incluir la navegación mediante el teclado y otras mejoras.

Los campos Múltiple, Selección única y Usuario asignado ahora ofrecen navegación mediante el teclado en la vista de lista:

* Utilice las flechas arriba y abajo del teclado para desplazarse por la lista de personas.

* Pulse la barra espaciadora para seleccionar una persona o para eliminar una persona seleccionada.

En campos de selección única y múltiple en la vista de lista:

* Puede añadir nuevas opciones directamente desde el editor cuando no se encuentren resultados. Tenga en cuenta que esta función puede no estar disponible en todas las listas.

* La interacción de campo ahora es accesible mediante el teclado. Esto incluye la navegación entre las etiquetas, las opciones de búsqueda y la lista mediante las flechas arriba y abajo. Pulse la barra espaciadora para seleccionar un elemento o quitar un elemento seleccionado.

Los campos de referencia, como los campos de escritura anticipada y búsqueda externa, han recibido algunas mejoras en la interfaz.

Además, cuando está disponible, la experiencia de arrastrar y soltar columnas se ha mejorado visualmente.

Para obtener más información, consulte [Administrar la vista de lista en Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md).

## Los campos de referencia de Workfront se habilitan como campos de búsqueda para las conexiones de Planning

>[!NOTE]
>
>Vista previa: 27 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026\
>Producción para todos: 16 de julio de 2026

Ahora puede agregar campos de referencia de Workfront como campos de búsqueda al conectar un tipo de registro de Planning con un tipo de objeto de Workfront.

Por ejemplo, puede agregar la información de Portfolio, Programa, Grupo o Empresa del objeto Proyecto a un campo de conexión de proyecto de una campaña en Planning.

Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

## Nuevos filtros para la función de desglose de vista de cronología

>[!NOTE]
>
>Vista previa: 27 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Ahora puede filtrar la información en la vista de la cronología en función de criterios que coincidan con los objetos incluidos en el desglose de los registros.

Antes de esta mejora, solo se podían aplicar filtros para los registros principales en la vista de cronología.

Para obtener más información, consulte [administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Nueva indicación de que los campos editados y eliminados afectan a los formularios de solicitud

>[!NOTE]
>
>Vista previa: 27 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Se ha agregado un recordatorio de que los campos de registro que edita o elimina pueden afectar a los formularios de solicitud que contienen esos campos. Ahora tendrá la oportunidad de revisar los formularios afectados y asegurarse de que los cambios que desee realizar en los campos no afecten a la información existente.

Para obtener más información, consulte [Editar configuración de campo](/help/quicksilver/planning/fields/edit-fields.md).

## Editar solicitudes de Planning enviadas

>[!NOTE]
>
>Vista previa: 27 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Ahora puede editar las solicitudes de Planning después de enviarlas, antes de crear un registro a partir de la solicitud.

Los siguientes usuarios pueden editar una solicitud enviada:

* El creador de la solicitud
* Administradores de Workspace para el espacio de trabajo donde se envió la solicitud
* Administradores del sistema

Antes de esta mejora, no se podían editar las solicitudes enviadas.

Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Nueva ventana de vista previa para fragmentos de contenido de AEM

>[!NOTE]
>
>Vista previa: 14 de mayo de 2026>Versión rápida de producción: 14 de mayo de 2026>Producción para todos: 14 de mayo de 2026>[!BADGE Fuera de horario]{type=Neutral}

Para obtener una mejor visibilidad al trabajar con fragmentos de contenido de AEM conectados a registros de Workfront Planning, se ha agregado una ventana de vista previa que muestra información sobre los fragmentos en Workfront Planning.

Esta funcionalidad estaba disponible anteriormente para los recursos de AEM y ahora se ha añadido a los fragmentos de contenido.

Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Los campos de búsqueda ya están disponibles para los fragmentos de contenido de AEM en Workfront Planning

>[!NOTE]
>
>Vista previa: 14 de mayo de 2026>Versión rápida de producción: 14 de mayo de 2026>Producción para todos: 14 de mayo de 2026>[!BADGE Fuera de horario]{type=Neutral}

Ahora puede agregar los siguientes campos de búsqueda al conectar un tipo de registro de Planning a un fragmento de contenido de AEM:

* Creado por
* Creado el
* Modificado por
* Modificado el

Antes de esta mejora, los campos de búsqueda solo estaban disponibles para carpetas y recursos de AEM.

Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).



## Vistas personalizadas para la página Detalles de un registro

>[!NOTE]
>
>Vista previa: 14 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Para permitir una mejor flexibilidad de visualización de la información en la página de detalles de un registro, hemos introducido la capacidad de crear vistas personalizadas para esta página.

Además de agregar dos vistas de página de detalles ya creadas que contienen todos los campos de registros o sólo los campos visibles en la vista de tabla, ahora puede crear vistas personalizadas para las páginas de detalles de un registro. Las vistas que cree serán visibles para todos los usuarios que tengan acceso al registro.

Esta actualización elimina la configuración **Mostrar todos los campos** y la reemplaza por vistas de detalles personalizadas.

Para obtener más información, consulte [Administrar la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).

## Agregar agrupaciones a una página de registros conectados de proyectos

>[!NOTE]
>
>Vista previa: 14 de mayo de 2026\
>Producción rápida: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Ahora puede agrupar la información en la página de registros conectados de proyectos de un registro en Workfront Planning. Esta capacidad no existía en esta área antes de esta mejora.

Para obtener más información, consulte [Administrar la vista de lista](/help/quicksilver/planning/views/manage-the-list-view.md).
