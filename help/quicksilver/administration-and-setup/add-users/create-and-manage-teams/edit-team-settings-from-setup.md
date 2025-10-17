---
title: Editar la configuración de un equipo desde el área Configuración
description: Como persona con la función de administrador de Adobe Workfront, puede editar la configuración de un equipo desde el área de configuración. Puede añadir usuarios a un equipo, establecer la plantilla de diseño de un equipo y establecer cómo se registra el estado cuando un equipo completa los elementos de trabajo.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 95%

---

# Editar la configuración de un equipo desde el área Configuración

Como persona con la función de administrador de Adobe Workfront, puede editar la configuración de un equipo desde el área de configuración. Puede añadir usuarios a un equipo, establecer la plantilla de diseño de un equipo y establecer cómo se registra el estado cuando un equipo completa los elementos de trabajo.

Para obtener información sobre los equipos, consulte [Información general sobre los equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Una persona con la función de administrador de grupos puede editar la configuración de un equipo para un grupo que administre. Para obtener más información, consulte [Crear y modificar los equipos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un usuario con una licencia Standard o Plan puede editar la configuración de un equipo desde el área de Equipos. Para obtener más información, consulte [Editar la configuración del equipo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar la configuración de un equipo

{{step-1-to-setup}}

1. Haga clic en **Equipos** en el panel izquierdo.
1. Seleccione un equipo y luego haga clic en **Editar** ![Editar icono](assets/edit-icon.png).

1. Realice cualquiera de los siguientes cambios:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de equipo</td> 
      <td>Escriba un nombre para el equipo.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Activo </td> 
       <td>Esta opción está habilitada de forma predeterminada para los equipos nuevos y existentes. Deshabilítela para desactivar el equipo. Para obtener más información, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Desactivar un equipo</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Grupo</td> 
      <td> <p>Asocie el equipo a un grupo. Empiece a escribir el nombre del grupo y, a continuación, selecciónelo cuando aparezca.</p> <p><b>NOTA</b>: Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupos de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores del grupo pueden ir al área Equipos desde el menú principal y hacer clic en la flecha de cambio de equipo <img src="assets/switch-team-icon.png" alt="Icono Cambiar de equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> <p>Para asegurarse de estar asociando el grupo correcto al equipo, pase el puntero por encima y haga clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Esta acción muestra la ayuda contextual con información sobre el grupo, como la jerarquía de los grupos que tiene por encima y sus administradores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propietario</td> 
      <td>Seleccione un propietario para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Integrantes del equipo</td> 
      <td> <p>Añada los integrantes del equipo. Empiece a escribir el nombre de un usuario y, a continuación, seleccione el nombre cuando aparezca. Repita este proceso para añadir varios usuarios al equipo.</p> 
      <p><b>SUGERENCIA</b>: Puede añadir cualquier número de usuarios a un equipo. Sin embargo, le recomendamos que no añada un número demasiado alto en un equipo, ya que la administración del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Plantilla de diseño</td> 
      <td> <p>Comience a escribir el nombre de la plantilla de diseño que desea que utilice el equipo y, a continuación, haga clic en él cuando aparezca.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Especifique si se trata de un equipo ágil. Para obtener información sobre los equipos ágiles y cómo administrar su trabajo, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo ágil</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Trabajar en ello</td> 
      <td> <p>Cambie el botón Trabajar en ello por el botón Iniciar. Cuando un usuario hace clic en Inicio, el estado del elemento se actualiza automáticamente.</p> <p>Para obtener más información sobre cómo configurar el botón Iniciar, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Iniciar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botón Listo</td> 
      <td> <p>Personalice el botón Listo. Para obtener más información, consulte:</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configurar el botón Listo para tareas</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configurar el botón Listo para problemas</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar cambios**.
