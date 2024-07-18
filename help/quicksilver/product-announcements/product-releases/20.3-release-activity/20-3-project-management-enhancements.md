---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Mejoras en la gestión de proyectos
description: Esta página describe todas las mejoras realizadas en la administración de proyectos con la versión 20.3 en el entorno de producción. Estas mejoras estuvieron disponibles en el entorno de producción la semana del 10 de agosto de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 20.3 Mejoras en la gestión de proyectos

Esta página describe todas las mejoras realizadas en la administración de proyectos con la versión 20.3 en el entorno de producción. Estas mejoras estuvieron disponibles en el entorno de producción la semana del 10 de agosto de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.3, consulte [Descripción general de la versión 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Formato de campo personalizado en listas

>[!NOTE]
>
>Esta función solo es compatible con la nueva experiencia de Adobe Workfront. Está disponible para algunas listas en Adobe Workfront Classic, pero no es compatible con Adobe Workfront Classic.

Ahora, cuando el administrador del sistema crea campos de formulario personalizados configurados para dar formato, puede dar formato al texto en los campos en los que más los utiliza: en listas en Workfront. En lugar de ir al área de Detalles para dar formato al texto en el formulario personalizado, puede hacer clic en un campo de una lista y aplicar negrita, cursiva y subrayado al texto.

Tenga en cuenta que esta funcionalidad solo está disponible en las listas actualizadas. Para obtener más información sobre las listas actualizadas, consulte [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Apariencia actualizada de varios encabezados globales

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Las áreas globales de Proyectos, Portfolio, Programas y Plantillas ahora tienen un encabezado actualizado que aprovecha mejor el espacio en pantalla. Esta actualización proporciona más espacio para la información con la que trabaja y en la que debe centrarse.

Se ha eliminado el vínculo Plantillas del área Proyectos. Puede seguir accediendo al área Plantillas desde el menú principal.

## Nuevo cuadro de diálogo Editar proyecto

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Como parte de la actualización del aspecto de la nueva experiencia de Workfront, hemos rediseñado el cuadro Editar proyecto. Puede tener acceso al nuevo cuadro Editar proyecto desde un proyecto individual o al editar un solo proyecto de una lista.

Además de una apariencia y presentación actualizadas, las siguientes mejoras están disponibles en el cuadro Editar proyecto:

* Personalice la plantilla de diseño una vez y refleje esas personalizaciones tanto en la página Detalles como en el cuadro Editar objeto.
* Los nombres de formulario personalizados individuales ahora están disponibles en el panel izquierdo dentro del cuadro Editar proyecto y puede acceder rápidamente a cada formulario desde allí.
* La funcionalidad de comentarios se elimina de la pantalla de edición del proyecto para eliminar la redundancia con la sección Actualizaciones.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

Para obtener información acerca del nuevo cuadro Editar proyecto, vea [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Nuevo panel de resumen y mejoras de actualizaciones para la lista de documentos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

El nuevo panel de resumen a la derecha de la lista de documentos ya está disponible con un diseño mejorado en la nueva experiencia de Workfront. Este panel proporciona las mismas acciones e información disponible en el panel de la derecha cuando selecciona un documento en Workfront Classic, incluidos los detalles del documento, las actualizaciones, el Forms personalizado, las aprobaciones y las versiones de los documentos.

Algunas acciones no están disponibles actualmente, pero se añadirán en una versión futura. Estas acciones incluyen el flujo de trabajo de revisión.

Para obtener más información, consulte [Resumen de documentos](../../../documents/managing-documents/summary-for-documents.md).

## Mejoras en los detalles del documento

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Busque las siguientes mejoras en la página Detalles del documento:

* Las opciones de la nueva versión se movieron a un menú desplegable cerca del panel izquierdo, lo que facilita el acceso.
* El icono Abrir prueba ha cambiado a una etiqueta Abrir prueba, lo que facilita su visualización en la página.
* Miniatura de vista previa más grande, que permite identificar fácilmente el documento
* Se ha añadido el icono Editar global, que permite editar varios campos a la vez.

Para obtener más información, vea [Información general sobre los detalles del documento](../../../documents/managing-documents/document-details-overview.md).

## Para administradores: establezca las preferencias del proyecto en el nivel de grupo

>[!NOTE]
>
>Esta funcionalidad no está disponible temporalmente para la mayoría de los clientes de los clústeres 1, 2, 3 y 5. Esta página se actualizará cuando se restablezca la funcionalidad para todos los clientes.

Para dar más autonomía a los administradores del grupo y permitir una mayor personalización de los flujos de trabajo a nivel de grupo, ahora puede definir las preferencias del proyecto en el nivel de grupo, para los grupos que administre. Al crear un proyecto, las preferencias del grupo surtirán efecto antes que las del sistema.

Todas las preferencias del proyecto se pueden personalizar en el nivel de grupo, excepto Cálculos de cronología y Trimestres personalizados.

Para obtener más información acerca de las Preferencias del proyecto de grupo, vea [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## Nuevo para administradores: cree campos de formulario personalizados donde los usuarios puedan dar formato al texto

En un formulario personalizado, ahora puede crear campos que incluyan botones de formato de texto. Cuando los usuarios escriben estos campos, pueden resaltar y organizar el texto con negrita, cursiva y subrayado. El límite alto de caracteres de 15 000 permite texto y formato abundantes.

Para obtener más información, consulte Crear un formulario personalizado en la nueva experiencia de Workfront.

## Nuevo para administradores: cree un nombre interno y una etiqueta orientada al usuario para un campo de formulario personalizado

Para ofrecerle más flexibilidad a la hora de etiquetar y volver a etiquetar campos de formulario personalizados, ahora puede crear un *nombre* interno para un campo, además de la *etiqueta* orientada al usuario que ha estado utilizando. Esto le proporciona la libertad de cambiar la etiqueta del campo que ven los usuarios sin cambiar el nombre del campo que ve el sistema.

En el pasado, la etiqueta se mostraba encima del campo para los usuarios y el sistema la utilizaba para identificar el campo. Por lo tanto, al cambiar la etiqueta para los usuarios, el campo fallaba dondequiera que se usara porque el sistema ya no podía identificarlo.


