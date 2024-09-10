---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Crear un horario
description: Puede definir las semanas laborables de los usuarios con horarios. Puede asociar una programación a un usuario o proyecto. Esto permite a [!DNL Workfront] calcular las escalas de tiempo y la disponibilidad del usuario.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Crear programación

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Como administrador de [!DNL Adobe Workfront], puede definir su semana laboral con horarios. Puede asociar una programación a un usuario o proyecto. Esto permite que [!DNL Workfront] calcule las escalas de tiempo y la disponibilidad del usuario.

Cuando tiene usuarios que trabajan en zonas horarias diferentes, la creación de una programación en cada una de ellas y su asociación con esos usuarios garantizan que su trabajo se registre en [!DNL Workfront] en tiempo real y que su disponibilidad sea siempre precisa según el momento en el que trabajen.

Para obtener información acerca de cómo asociar programaciones con usuarios y proyectos, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) y [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Los administradores de grupos también pueden crear programaciones asociadas a los grupos que administran. Para obtener más información, vea [Crear y modificar las programaciones de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Para obtener información acerca del uso de programaciones para ayudar a los usuarios a colaborar en [!DNL Workfront] en diferentes zonas horarias, vea [Trabajar en diferentes zonas horarias](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Para obtener información acerca de cómo se usan las programaciones en la planificación de recursos, vea [Información general sobre las programaciones](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) y [Información general del Planificador de recursos](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
       <p>O</p>
       <p>Actual: [!UICONTROL plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>  
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear programación

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Horarios]**.
1. Haga clic en **[!UICONTROL Nuevo horario]**.
1. Introduzca un nombre para la programación.
1. (Opcional) Seleccione **[!UICONTROL Horario predeterminado]** para identificar este horario como el predeterminado.

   Debe haber al menos una programación en [!DNL Workfront]. Si solo tiene uno, se designa como el horario predeterminado.

   Puede tener más de una programación, pero solo puede tener una predeterminada.

   >[!NOTE]
   >
   >No puede designar una programación como predeterminada si es administrador de un grupo. Solamente un administrador de [!DNL Workfront] puede designar una programación como predeterminada para el sistema.

   ![Nueva programación](assets/new-schedule.png)

1. En la ficha **[!UICONTROL Horario]**, seleccione un horario diario arrastrando el contorno azul a través de bloques de horas para resaltarlos.

   Le recomendamos que seleccione 8 bloques de una hora durante un periodo de 9 horas. Este alojamiento sirve almuerzos y otras pausas.

   ![Bloques de tiempo en una programación](assets/new-schedule-with-exceptions.png)

1. En la ficha **[!UICONTROL Detalles]**, escriba la siguiente información:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Grupo con acceso de administración]</td>
     <td><p>Seleccione el grupo cuyos administradores tengan permisos para editar esta programación.</p>
     <p><b>IMPORTANTE</b>:</p>
      <ul>
       <li>
       <p>Si es administrador de un grupo y crea una programación, este campo es obligatorio.</p>
       <p>Como administrador de grupo, puede crear una programación sólo si está designada para un grupo o subgrupo para el que está designado como administrador.</p>
       <p>Si administra un solo grupo, ese grupo se selecciona en este campo de forma predeterminada.</p>
       <p>Si administra varios grupos, debe seleccionar un grupo en este campo antes de guardar la programación.</p></li>
       <li>Si es administrador de [!DNL Workfront] y está creando una programación, este campo es opcional. Cuando crea una programación sin asociarla a un grupo, se guarda como una programación de nivel de sistema y no puede ser administrada por un administrador de grupo de ningún grupo.
       <p>Los programas asignados a cuentas o proyectos son visibles para todos los usuarios que pueden editar estos objetos. Esto es así tanto para las programaciones de nivel de sistema como para las de nivel de grupo.</p>
       </li>
       <p>Especificar un grupo con acceso de administración para una programación no asigna la programación a los usuarios del grupo; sólo permite a los administradores del grupo editar, eliminar y copiar la programación.</p>
       <p>Los administradores de grupo no pueden editar, eliminar ni copiar programaciones de nivel de sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Grupos con acceso de visualización]</td>
     <td><p>Seleccione los grupos con acceso a [!UICONTROL View] que puedan ver esta programación.</p>
     <p>Solo los usuarios de los grupos especificados aquí pueden encontrar la programación en el menú desplegable cuando la asignan a usuarios o proyectos.</p></tr>
    <tr>
     <td>[!UICONTROL Zona horaria]</td>
     <td><p>Seleccione la zona horaria de la programación.</p>
     <p>Si asocia la programación con un usuario, le recomendamos que la zona horaria de la programación coincida con la del usuario. Para obtener información acerca de las zonas horarias del usuario, vea <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario.
     </td>
    </tr>
   </table>


1. En la ficha **[!UICONTROL Excepciones]**, especifique las excepciones a la programación.

   Las excepciones son días completos o medios que deben excluirse del horario, como festivos o eventos de la empresa.

   >[!NOTE]
   >
   >Si ya sabe cuáles son las excepciones de programación recurrentes, puede definir las excepciones de programación para muchos años en el futuro.

   Los días completos o parciales pueden excluirse del horario de trabajo. Haga clic en la fecha para seleccionarla como excepción y, a continuación, seleccione el campo **[!UICONTROL Todo el día]** para indicar si la excepción es un día completo o no.

   ![Excepción de todo el día](assets/schedule-adding-an-all-day-exception.png)

1. Introduzca la hora de inicio y finalización para las excepciones de día parciales.

   ![Excepción parcial de día](assets/partial-day-exception-on-schedules.png)

1. Haga clic en **[!UICONTROL Guardar]** y luego en **[!UICONTROL Guardar] cambios**.

1. (Opcional) Asocie la programación a un usuario.

   Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Opcional) Asocie la programación a un proyecto.

   Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).
