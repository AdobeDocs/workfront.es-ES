---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2 2018.1 Beta 2
description: En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.1 Beta 2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 14 de diciembre de 2017. Estará disponible en el entorno de producción en marzo de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
TQID: https://experienceleague.adobe.com/6vUGOgtvkP4c4yBRo-wZTPB20tLdy-C1z28Ilg-xOok
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1304
ht-degree: 97%

---

# Actividad de la versión 2 2018.1 Beta 2

En esta página se describen todos los cambios disponibles más recientemente en el entorno de vista previa con la versión 2018.1 Beta 2. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 14 de diciembre de 2017. Estará disponible en el entorno de producción en marzo de 2018.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción.

Para ver una lista de todos los cambios realizados en 2018.1, consulte [Información general sobre la actividad de la versión 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versión 2018.1 Beta 2 contiene mejoras para administradores de Workfront y otros usuarios:

**Para los administradores**

* [Administración de grupos para usuarios y plantillas de diseño](#group-administration-for-users-and-layout-templates)

**Para todos los usuarios**

* [Pantalla panorámica en todo el sistema](#system-wide-widescreen-display)
* [Cambiar el tamaño de instantánea de cronología en el gráfico Gantt](#resize-timeline-snapshot-on-the-gantt-chart)
* [Planificador de recursos interactivos en el caso empresarial](#interactive-resource-planner-in-the-business-case)
* [Visualización en el Planificador de recursos - Gráfico de asignación de usuarios](#visualization-in-the-resource-planner-user-allocation-chart)
* [Mejoras en el área Inicio](#improvements-in-the-home-area)
* [Nuevas mejoras en el visor de corrección](#new-proofing-viewer-improvements) 

## Administración de grupos para usuarios y plantillas de diseño {#group-administration-for-users-and-layout-templates}

Ahora puede designar administradores de grupos en Workfront. Se ha cambiado el nombre del campo Propietario del grupo a administrador de grupos y los usuarios designados como administradores de grupos tienen permisos adicionales para administrar usuarios y plantillas de diseño para los grupos que administran.

* [Administración de usuarios por administrador de grupos](#user-management-by-group-administrator)
* [Administración de plantillas de diseño por administradores de grupos](#layout-template-management-by-group-administrators)

### Administración de usuarios por administrador de grupos {#user-management-by-group-administrator}

Presentamos el nuevo concepto de **administrador de grupos**. Para ello, se ha cambiado el nombre del campo **Propietario del grupo** a **administrador de grupos** y los usuarios designados como administradores de grupos tienen permisos adicionales para administrar usuarios y grupos.

Además de los permisos que el Propietario del grupo tenía anteriormente para administrar usuarios, el administrador de grupos tiene ahora el siguiente acceso adicional cuando se administra usuarios dentro de los grupos en los que están configurados como administrador de grupos:

* Inicie sesión como otro usuario que pertenezca a un grupo que administre.
* Restablezca la contraseña de otro usuario que pertenezca a un grupo que administre.
* Cree plantillas de diseño administradas por su grupo. 

Antes de este cambio, solo el administrador de Workfront podía realizar estas funciones.

Para obtener más información sobre los administradores de grupos, consulte la sección &quot;Descripción de los administradores de grupos&quot; en [Crear un grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Administración de plantillas de diseño por administradores de grupos {#layout-template-management-by-group-administrators}

Presentamos el nuevo concepto de **Grupo con acceso de administración** que puede asociar con una plantilla de diseño.

El usuario designado como administrador de grupos en este grupo tiene acceso para administrar esa plantilla de diseño y crear nuevas plantillas de diseño en las que los grupos que administra son los grupos administrativos de las plantillas. 

Antes de este cambio, solo el administrador de Workfront podía crear plantillas de diseño.

Para obtener más información sobre la creación de plantillas de diseño, consulte &quot;Creación y administración de plantillas de diseño&quot;.

## Pantalla panorámica en todo el sistema {#system-wide-widescreen-display}

Al mostrar cualquier página en Workfront, toda la ventana del explorador se rellena automáticamente y se ajusta al tamaño de la pantalla.

Antes de este cambio, solo se mostraban en pantalla panorámica las páginas asociadas con los siguientes objetos:

* Proyectos
* Tareas
* Problemas
* Informes
* Paneles de control
* Calendarios

## Cambiar el tamaño de instantánea de cronología en el gráfico Gantt {#resize-timeline-snapshot-on-the-gantt-chart}

Ahora puede expandir la instantánea de cronología para mostrar todo el proyecto en el gráfico Gantt.

Antes de esta mejora, se podía seleccionar un punto específico de la instantánea de cronología para navegar hasta él en el gráfico Gantt.

Para obtener más información sobre la configuración de la información que se muestra en el gráfico Gantt, consulte [Configurar la presentación de la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Planificador de recursos interactivos en el caso empresarial {#interactive-resource-planner-in-the-business-case}

Como persona administradora de recursos, ahora puede añadir conjuntos de recursos en la sección Presupuestación de recursos del caso empresarial. También puede presupuestar los recursos del proyecto mediante el Planificador de recursos en el nivel de proyecto. Al presupuestar los recursos para un proyecto, se genera el coste laboral presupuestado del proyecto.

Antes de este cambio, podía ver la información de presupuestación de recursos en el caso empresarial si el proyecto se había presupuestado para recursos en el Planificador de recursos global.

Para obtener más información acerca de cómo completar la presupuestación de recursos de proyecto en el caso empresarial, consulte [Presupuestar recursos en el caso empresarial](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualización en el Planificador de recursos - Gráfico de asignación de usuarios {#visualization-in-the-resource-planner-user-allocation-chart}

Ahora puede mostrar la asignación planificada general de todos los usuarios en relación con su disponibilidad en un gráfico del Planificador de recursos. El gráfico está disponible cuando se selecciona **Ver por usuario** en el Planificador de recursos.

El gráfico muestra la siguiente información:

* % de disponibilidad sin asignación excesiva para todos los usuarios
* % de asignación excesiva para todos los usuarios
* % de infrautilización para todos los usuarios
* Al menos un usuario tiene una asignación excesiva durante este período de tiempo

Antes de este cambio, podía ver la asignación y la disponibilidad de los usuarios individuales solo en formato de tabla.

Para obtener más información sobre el gráfico de asignación de usuarios en el Planificador de recursos, consulte [Información general sobre el Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Mejoras en el área Inicio {#improvements-in-the-home-area}

Ya hay varias mejoras disponibles en el área Inicio, entre ellas:

* Mejoras en la apariencia

   * El panel derecho ahora es más grande, lo que aumenta el espacio para la información de tareas y problemas.
   * Los elementos vencidos ahora se muestran en un tono rojo más claro cuando se seleccionan en el panel izquierdo.
   * Ahora se puede ver con mayor facilidad la relación entre el panel izquierdo y el derecho. El documento seleccionado en el panel izquierdo señala al panel derecho.

* Se muestran los campos predeterminados de los elementos seleccionados. 

  Para obtener más información sobre los campos predeterminados, consulte “Creación y administración de plantillas de diseño”.

* Después de hacer clic en “Trabajar en ello” en una solicitud, los campos asociados al problema se muestran en el panel derecho.

  Para obtener más información sobre el trabajo con solicitudes desde el área Inicio, consulte [Administrar solicitudes de trabajo y equipo en el área Inicio](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) en [Administrar solicitudes de trabajo y equipo en el área Inicio](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Se puede elegir un avatar de usuario en un elemento de trabajo del panel izquierdo para ver el nombre del usuario.
* Se puede expandir el área “Retrasado” en el panel izquierdo para ver todos los elementos retrasados (cuando esta área está contraída, solo se muestran los 5 primeros elementos).
* Después de marcar un elemento como completado, permanece en el panel izquierdo hasta que se selecciona otro elemento.\
  Para obtener información acerca de cómo mostrar elementos completados, consulte [Mostrar elementos en la lista de trabajos del área Inicio](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) en [Mostrar elementos en la lista de trabajos del área Inicio](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Para obtener más información acerca del uso de la nueva área Inicio, así como información que describe las diferencias de funcionalidad entre Mi trabajo e Inicio, consulte [Usar el área Inicio](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nuevas mejoras en el visor de corrección  {#new-proofing-viewer-improvements}

* [Disposición y diseño mejorados](#improved-layout-and-design)
* [Buscar comentarios por número de comentario](#search-comments-by-comment-number)
* [Opción para editar comentario junto al indicador de marcado](#option-to-edit-comment-next-to-the-markup-indicator)
* [Marcar todos los comentarios como leídos](#mark-all-comments-as-read)
* [Mejoras en el menú izquierdo](#left-menu-improvements)

### Disposición y diseño mejorados {#improved-layout-and-design}

El visor de corrección tiene una apariencia actualizada. Se han actualizado las siguientes áreas del visor de corrección:

* Área de miniaturas

  Para obtener más información sobre el uso del área de miniaturas, consulte.

* Área de comentarios\
  Para obtener más información sobre el área de comentarios, consulte.
* Área de menú izquierda

### Buscar comentarios por número de comentario {#search-comments-by-comment-number}

Ahora, cuando busque la lista de comentarios en el visor de pruebas, puede introducir el número del comentario en el campo de búsqueda. A continuación, la lista de comentarios se filtra para mostrar el comentario que ha buscado. 

Para obtener más información, consulte.

### Opción para editar comentario junto al indicador de marcado {#option-to-edit-comment-next-to-the-markup-indicator}

Ahora puede editar más fácilmente un comentario existente. Después de hacer clic en un indicador de comentario en la prueba, se muestra un icono de edición junto al globo. 

Antes de este cambio, tenía que hacer clic en el icono de edición del área Comentario.  

Para obtener más información, consulte.

### Marcar todos los comentarios como leídos {#mark-all-comments-as-read}

Al ver un documento en el visor de corrección, ahora puede marcar todos los comentarios como leídos.

### Mejoras en el menú izquierdo {#left-menu-improvements}

El menú de la izquierda del visor de corrección contiene las siguientes mejoras:

* Apariencia actualizada
* Icono en la parte superior del menú para mostrar u ocultar el menú

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* Pase el puntero por encima del menú para expandir automáticamente el menú y ver las etiquetas además de los iconos. (O bien, habilite la opción para mantener el menú siempre en la vista contraída.)
