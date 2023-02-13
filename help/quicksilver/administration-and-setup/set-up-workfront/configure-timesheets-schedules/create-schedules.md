---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Crear una programación
description: Puede definir las semanas de trabajo de los usuarios mediante programas. Puede asociar una programación con un usuario o un proyecto. Esto permite que [!DNL Workfront] para calcular las cronologías y la disponibilidad del usuario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Crear una programación

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Como [!DNL Adobe Workfront] administrador, puede definir la semana laboral mediante programas. Puede asociar una programación con un usuario o un proyecto. Esto permite que [!DNL Workfront] para calcular las cronologías y la disponibilidad del usuario.

Cuando tiene usuarios que trabajan en zonas horarias diferentes, la creación de una programación en cada una de las zonas horarias y su asociación con esos usuarios garantiza que su trabajo se registre en [!DNL Workfront] en tiempo real y que su disponibilidad es siempre precisa según el momento de su trabajo.

Para obtener información sobre cómo asociar programaciones con usuarios y proyectos, consulte los siguientes artículos:

* [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md)

Los administradores de grupos también pueden crear programaciones asociadas a los grupos que administran. Para obtener más información, consulte [Crear y modificar las programaciones de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Para obtener información sobre el uso de programaciones para ayudar a los usuarios a colaborar en [!DNL Workfront] en zonas horarias, consulte [Trabajo en zonas horarias](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de [!UICONTROL Adobe Workfront]</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Crear una programación

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).
1. Haga clic en **[!UICONTROL Programaciones]**.
1. Haga clic en **[!UICONTROL Nueva programación]**.
1. Especifique un nombre para la programación.
1. (Opcional) Seleccione **[!UICONTROL Programación predeterminada]** para identificar esta programación como la predeterminada.

   Puede tener más de una programación en [!DNL Workfront], pero solo puede tener una programación predeterminada.

   Debe tener al menos una programación en [!DNL Workfront]. Si solo tiene uno, se designa como la programación predeterminada.

   >[!NOTE]
   >
   >No puede designar una programación como la programación predeterminada si es un administrador de grupo. Solo un [!DNL Workfront] el administrador puede designar una programación como predeterminada para el sistema.

   ![](assets/new-schedule.png)

1. En el **[!UICONTROL Programación]** , seleccione una programación diaria arrastrando el contorno azul a lo largo de bloques de hora para resaltarlos.

   Se recomienda seleccionar 8 bloques de una hora durante un período de tiempo de 9 horas. Se puede comer o disfrutar de otras pausas.

   ![](assets/new-schedule-with-exceptions.png)

1. En el **[!UICONTROL Detalles]** especifique la siguiente información:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Grupo con acceso de administración]</td>
     <td><p>Indique el grupo cuyos administradores tienen permiso para editar esta programación.</p>
     <p><b>IMPORTANTE</b>:</p>
      <ul>
       <li>
       <p>Si es un administrador de grupo que crea una programación, este campo es obligatorio.</p>
       <p>Como administrador de grupos, puede crear una programación solo si está designada para un grupo o subgrupo para el que esté designado como administrador.</p>
       <p>Si administra solo un grupo, ese grupo se selecciona en este campo de forma predeterminada.</p>
       <p>Si administra varios grupos, debe seleccionar un grupo en este campo antes de guardar la programación.</p></li>
       <li>Si es [!DNL Workfront] administrador creando una programación, este campo es opcional. Cuando se crea una programación sin asociarla a un grupo, se guarda como una programación a nivel de sistema y no puede ser administrada por un administrador de grupo de ningún grupo.
       <p>Los programas asignados a cuentas o proyectos son visibles para todos los usuarios que pueden editar estos objetos. Esto se aplica tanto a las programaciones de nivel de sistema como de grupo.</p>
       </li>
       <p>Al especificar un grupo con acceso de administración para una programación, no se asigna la programación a los usuarios del grupo; solo permite a los administradores de grupos del grupo editar, eliminar y copiar la programación.</p>
       <p>Los administradores de grupo no pueden editar, eliminar ni copiar programas a nivel de sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Grupos con acceso de vista]</td>
     <td><p>Seleccione los grupos con acceso a [!UICONTROL View] para los que esta programación es visible.</p>
     <p>Solo los usuarios de los grupos especificados aquí pueden encontrar la programación en el menú desplegable cuando la asignan a usuarios o proyectos.</p></tr>
    <tr>
     <td>[!UICONTROL Huso horario]</td>
     <td><p>Seleccione la zona horaria de la programación.</p>
     <p>Si asocia la programación con un usuario, recomendamos que la zona horaria de la programación coincida con la del usuario. Para obtener información sobre las zonas horarias del usuario, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario.
     </td>
    </tr>
   </table>


1. En el **[!UICONTROL Excepciones]** especifique las excepciones a la programación.

   Las excepciones son días completos o medios que deben excluirse de la programación, como días festivos o eventos de la empresa.

   >[!NOTE]
   >
   >Si ya sabe cuáles son las excepciones de programación recurrentes, puede definir las excepciones de programación para muchos años en el futuro.

   Los días completos o parciales pueden excluirse del programa de trabajo. Haga clic en la fecha para seleccionarla como excepción y, a continuación, seleccione la **[!UICONTROL Todo el día]** para indicar si la excepción es un día completo o no.

   ![](assets/schedule-adding-an-all-day-exception.png)

1. Especifique la hora de inicio y finalización para las excepciones de día parcial.

   ![día parcial-excepción-en-programaciones.png](assets/partial-day-exception-on-schedules.png)

1. Haga clic en **[!UICONTROL Guardar]** y haga clic en **[!UICONTROL Guardar] Cambios**.

1. (Opcional) Asocie la programación a un usuario.

   Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Opcional) Asocie la programación a un proyecto.

   Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).
