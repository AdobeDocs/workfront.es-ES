---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiar una plantilla de proyecto
description: Además de crear una plantilla de proyecto desde cero, también puede copiar una existente y modificarla.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 46%

---

# Copiar una plantilla de proyecto

<!--Audited: 5/2025-->

Además de crear una plantilla de proyecto desde cero, también puede copiar una existente y modificarla en Adobe Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

Debe tener el siguiente acceso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a las plantillas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores de una plantilla</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Consideraciones sobre la copia de plantillas

Los siguientes elementos siempre se copian de una plantilla existente a una nueva:

* Tareas de plantilla
* Información de valor predeterminado de la tarea de plantilla (proceso de aprobación predeterminado de tarea, formularios personalizados predeterminados de tarea)
* Formularios personalizados
* Riesgos
* Información de configuración de cola
* Portafolio y programa
* Rutas de aprobación
* Documentos
* Los días de las tareas de plantilla originales se transfieren a la nueva plantilla. Debe cambiar el día de inicio o finalización de la plantilla (según su modo de programación) para actualizar los días de las tareas de plantilla, si es necesario.

Los siguientes elementos nunca se copian de una plantilla existente a una nueva:

* Tarifas de facturación
* Comentarios del usuario

## Copiar una plantilla

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Vaya a la plantilla que desea copiar.
1. Haga clic en el icono **Más** del menú ![Más](assets/qs-more-icon-on-an-object.png) a la derecha del nombre de la plantilla en el encabezado, luego haga clic en **Copiar**.

   Se abre el cuadro **Copiar plantilla**.

   ![Copiar cuadro de plantilla](assets/copy-template-box.png)

1. Especifique un nombre para la plantilla en el campo **Nuevo nombre de plantilla**.

   De manera predeterminada, Workfront establece el nuevo nombre con este formato: `Copy of Original template name`.

1. Seleccione la opción **Conservar asignaciones de usuarios en tareas y plantillas** si desea transferir todas las asignaciones de tareas y plantillas de la plantilla original a la nueva. Las asignaciones de tareas de plantilla, el Propietario de la plantilla y el Patrocinador se transfieren a la plantilla copiada.
1. Haga clic en **Guardar** para crear una copia de la plantilla.

   La nueva plantilla se muestra en la lista de plantillas del área de Plantilla de Workfront.
