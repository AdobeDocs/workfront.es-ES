---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Mejoras en la gestión de proyectos
description: En esta página se describen todas las mejoras en la administración de proyectos realizadas con la versión 20.3 en el entorno Producción. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 10 de agosto de 2020.
author: Luke
feature: Product Announcements
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 20.3 Mejoras en la gestión de proyectos

En esta página se describen todas las mejoras en la administración de proyectos realizadas con la versión 20.3 en el entorno Producción. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 10 de agosto de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.3, consulte [Información general sobre la versión 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Formato de campo personalizado en listas

>[!NOTE]
>
>Esta función solo es compatible con la nueva experiencia de Adobe Workfront. Está disponible para algunas listas en Adobe Workfront Classic, pero no es compatible con Adobe Workfront Classic.

Ahora, cuando el administrador del sistema crea campos de formulario personalizados que están configurados para el formato, puede dar formato al texto en los campos en los que más los utilice: en listas a través de Workfront. En lugar de ir al área Detalles para dar formato al texto del formulario personalizado, puede hacer clic en un campo de una lista y aplicar negrita, cursiva y subrayado al texto.

Tenga en cuenta que esta funcionalidad solo está disponible en las listas actualizadas. Para obtener más información sobre listas actualizadas, consulte [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Para obtener información sobre cómo un administrador de Workfront crea campos de texto con formato, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Aspecto actualizado de varios encabezados globales

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Las áreas globales de Proyectos, Portfolio, Programas y Plantillas ahora tienen un encabezado actualizado que hace un mejor uso del espacio en la pantalla. Esta actualización proporciona más espacio para la información con la que debe centrarse.

Se ha eliminado el vínculo Plantillas del área Proyectos . Puede seguir accediendo al área Plantillas desde el menú principal.

## Nueva casilla Editar proyecto

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Como parte de la actualización del aspecto de la nueva experiencia de Workfront, hemos rediseñado el cuadro Editar proyecto . Puede acceder al nuevo cuadro Editar proyecto desde un proyecto individual o al editar un proyecto individual desde una lista.

Además de una apariencia actualizada, las siguientes mejoras están disponibles en el cuadro Editar proyecto :

* Personalice la plantilla de diseño una vez y refleje esas personalizaciones tanto en la página Detalles como en el cuadro Editar objeto .
* Los nombres de formulario personalizados individuales ahora están disponibles en el panel izquierdo dentro del cuadro Editar proyecto y puede acceder rápidamente a cada formulario desde allí.
* La funcionalidad de comentarios se elimina de la pantalla del proyecto de edición para eliminar la redundancia con la sección Actualizaciones .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

Para obtener información sobre el nuevo cuadro Editar proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Nuevo panel Resumen y mejoras de Actualizaciones para la lista de documentos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

El nuevo panel Resumen a la derecha de la lista de documentos ya está disponible con un diseño mejorado en la nueva experiencia de Workfront. Este panel proporciona las mismas acciones e información disponible en el panel de la derecha cuando selecciona un documento en Workfront Classic, incluidos detalles del documento, actualizaciones, Forms personalizado, aprobaciones y versiones del documento.

Algunas acciones no están disponibles actualmente, pero se agregarán en una versión futura. Estas acciones incluyen el flujo de trabajo de prueba.

Para obtener más información, consulte [Resumen de los documentos](../../../documents/managing-documents/summary-for-documents.md).

## Mejoras en los detalles del documento

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Busque las siguientes mejoras en la página Detalles del documento :

* Las nuevas opciones de versión se han movido a un menú desplegable cerca del panel izquierdo, lo que facilita el acceso.
* El icono Abrir prueba cambió a una etiqueta Abrir prueba , lo que facilita su visualización en la página.
* Vista previa en miniatura más grande, lo que permite identificar fácilmente el documento
* Se ha añadido el icono Editar global, que permite editar varios campos a la vez.

Para obtener más información, consulte [Información general sobre detalles del documento](../../../documents/managing-documents/document-details-overview.md).

## Para administradores: defina las preferencias del proyecto en el nivel de grupo

>[!NOTE]
>
>Esta funcionalidad no está disponible temporalmente para la mayoría de los clientes de los clústeres 1, 2, 3 y 5. Esta página se actualizará cuando se restablezca la funcionalidad para todos los clientes.

Para dar más autonomía a los administradores del grupo y permitir una mayor personalización de los flujos de trabajo a nivel de grupo, ahora puede definir las preferencias del proyecto a nivel de grupo para los grupos que administra. Al crear un proyecto, las preferencias del grupo surtirán efecto antes que las del sistema.

Todas las preferencias del proyecto se pueden personalizar en el nivel del grupo, excepto en los cálculos de línea de tiempo y en los trimestres personalizados.

Para obtener más información sobre las preferencias de grupo de proyectos, consulte [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## Novedades para administradores: Crear campos de formulario personalizados donde los usuarios pueden dar formato al texto

En un formulario personalizado, ahora puede crear campos que incluyan botones de formato de texto. Cuando los usuarios escriben en estos campos, pueden resaltar y organizar su texto con negrita, cursiva y subrayado. El límite de caracteres alto de 15.000 permite un montón de texto y formato.

Para obtener más información, consulte Creación de un formulario personalizado en la nueva experiencia de Workfront.

## Novedades para administradores: Cree un nombre interno y una etiqueta de cara al usuario para un campo de formulario personalizado

Para proporcionar más flexibilidad al etiquetar y volver a etiquetar campos de Formulario personalizado, ahora puede crear un *name* para un campo además de la cara del usuario *label* has estado usando. Esto le da la libertad de cambiar la etiqueta de campo que ven los usuarios sin cambiar el nombre de campo que ve el sistema.

En el pasado, la etiqueta se mostraba encima del campo para los usuarios y la utilizaba el sistema para identificar el campo. Por lo tanto, al cambiar la etiqueta de los usuarios, el campo no funcionaba correctamente dondequiera que se usara porque el sistema ya no podía identificarlo.

Para obtener más información, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

