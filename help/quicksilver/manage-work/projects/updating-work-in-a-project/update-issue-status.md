---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar estado del problema
description: Puede actualizar el estado de un problema para informar a otros sobre dónde se encuentra y cómo progresa.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 99%

---

# Actualizar el estado de un problema

<!--Audited: 01/2024-->

Puede actualizar el estado de un problema para informar a otros sobre dónde se encuentra y cómo progresa.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para el problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Estados de los problemas

Los siguientes son los estados predeterminados para los problemas en Workfront:

* Nuevo
* En curso
* Esperando comentarios
* En espera
* No se puede resolver
* Vuelto a abrir
* Cerrado
* Resuelto

El administrador de Adobe Workfront puede añadir estados personalizados para los problemas de su organización. También pueden hacer que los estados estén disponibles según el tipo de problema.

Para obtener más información sobre los estados personalizados y los tipos de problemas, consulte los siguientes artículos:

* [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Crear problemas](../../../manage-work/issues/manage-issues/create-issues.md)

Puede actualizar manualmente los estados de los problemas o dejar que Workfront los actualice automáticamente cuando se realicen determinadas acciones.

## Actualizar el estado del problema manualmente

Puede actualizar el estado del problema en las siguientes áreas de Workfront:

* El encabezado del problema en la página de tareas.
* El cuadro Editar problema, al editar un problema.
* La sección Detalles en la página del problema.
* En una lista de problemas o un informe, cuando el campo Estado esté visible en la vista.
* En el panel Resumen del problema.

Para actualizar de forma manual el estado del problema en el encabezado del mismo:

1. Vaya a un problema en el que desee actualizar el estado.
1. Haga clic en el campo **Estado** en el encabezado del problema y seleccione un nuevo estado.
1. Para proporcionar una indicación visual de la finalización del problema, arrastre o haga doble clic en la burbuja bajo **Porcentaje completado** en el encabezado del problema

   O

   Haga clic dentro de la burbuja en el encabezado del problema para introducir un porcentaje.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Opcional) Realice una de las siguientes acciones para proporcionar información adicional sobre la actualización:

   * Para añadir una nota sobre la actualización, vaya a la sección **Actualizaciones**, haga clic en **Nuevo comentario** y luego escriba una nota.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Para notificar la actualización a determinados usuarios, escriba sus nombres en el campo **Etiquetar personas o equipos** que aparece al escribir un comentario. Para obtener más información, consulte [Etiquetar a otros en las actualizaciones](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Para actualizar el estado de la fecha de confirmación del problema, haga clic en **Detalles del problema** y, a continuación, edite el campo **Fecha de confirmación**. Para obtener más información, consulte [Editar problemas](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Solo las personas asignadas al problema pueden actualizar la fecha de confirmación.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## Actualizar el estado del problema automáticamente

Workfront actualiza automáticamente el estado existente de un problema a un estado diferente cuando se producen las acciones enumeradas en la siguiente tabla.

>[!NOTE]
>
>Los estados de la tabla siguiente son estados de sistema predeterminados. El administrador de grupos o de Workfront puede cambiar el nombre de los estados de su instancia de Workfront. Para obtener información sobre cómo crear y administrar estados en Workfront, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Acción</b></td> 
   <td><b>Estado original</b></td> 
   <td><b>Nuevo estado</b></td> 
  </tr> 
  <tr> 
   <td>Actualizar el porcentaje completado del problema al 100 %</td> 
   <td>Nuevo o En curso</td> 
   <td>Cerrado</td> 
  </tr> 
  <tr> 
   <td>Actualizar el porcentaje completado del problema del 100 % a un número inferior</td> 
   <td>Cerrado </td> 
   <td>En curso</td> 
  </tr> 
  <tr> 
   <td>Actualizar el estado de un objeto de resolución adjunto al problema</td> 
   <td>Varios estados</td> 
   <td> <p>Varios estados</p> <p>Para obtener información sobre la resolución de objetos y cómo afectan al estado de los problemas, consulte la sección “Sincronizar el estado del objeto solucionable con el del objeto solucionable” en el artículo <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Haga clic en el botón Iniciar problema para aceptar trabajar en un problema que se le haya asignado</span> </td> 
   <td><span>Nuevo</span> </td> 
   <td> <p>Cualquier estado asociado con el botón Iniciar problema en la configuración del equipo de inicio. </p> <p>Para obtener información acerca de cómo reemplazar el botón Trabajar en ello por un botón Iniciar problema, consulte <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Inicio</a></span><span>.</span> </p> <p>Sugerencia: al hacer clic en <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">el botón Deshacer</span> después de hacer clic en Iniciar problema, se revierte el estado a Nuevo. </p> </td> 
  </tr> 
 </tbody> 
</table>
