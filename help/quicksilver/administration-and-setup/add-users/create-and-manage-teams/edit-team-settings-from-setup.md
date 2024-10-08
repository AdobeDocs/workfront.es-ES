---
title: Editar la configuración de un equipo desde el área de configuración
description: Como administrador de Adobe Workfront, puede editar la configuración de un equipo desde el área de Configuración. Puede agregar usuarios a un equipo, establecer la plantilla de diseño de un equipo y establecer cómo se registra el estado cuando un equipo completa los elementos de trabajo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---

# Editar la configuración de un equipo desde el área de Configuración

Como administrador de Adobe Workfront, puede editar la configuración de un equipo desde el área de Configuración. Puede agregar usuarios a un equipo, establecer la plantilla de diseño de un equipo y establecer cómo se registra el estado cuando un equipo completa los elementos de trabajo.

Para obtener información sobre los equipos, vea [Información general de los equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un administrador de grupo puede editar la configuración de un equipo para un grupo que administre. Para obtener más información, vea [Crear y modificar los equipos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un usuario con una licencia de planificación puede editar la configuración de un equipo desde el área Personas. Para obtener más información, consulte [Editar la configuración del equipo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
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
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar la configuración de un equipo

{{step-1-to-setup}}

1. Haga clic en **Equipos** en el panel izquierdo.
1. Seleccione un equipo y luego haga clic en **Editar** ![](assets/edit-icon.png).

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
       <td>Esta opción está habilitada de forma predeterminada para los equipos nuevos y existentes. Desactívela para desactivar el equipo. Para obtener más información, vea <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Desactivar un equipo</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Grupo</td> 
      <td> <p>Asocie el equipo a un grupo. Empiece a escribir el nombre del grupo y, a continuación, selecciónelo cuando aparezca.</p> <p><b>NOTA</b>: cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores del grupo pueden ir al área Equipos desde el menú principal y hacer clic en la flecha para cambiar de equipo <img src="assets/switch-team-icon.png" alt="Icono Cambiar equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> <p>Puede asegurarse de que está asociando el grupo correcto con el equipo pasando el puntero sobre él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propietario</td> 
      <td>Seleccione un propietario para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Miembros del equipo</td> 
      <td> <p>Agregar y agregar integrantes del equipo. Empiece a escribir el nombre de un usuario y, a continuación, seleccione el nombre cuando aparezca. Repita este proceso para agregar varios usuarios al equipo.</p> 
      <p><b>SUGERENCIA</b>: puede agregar cualquier número de usuarios a un equipo. Sin embargo, le recomendamos que no agregue un número demasiado grande en un equipo, ya que la administración del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Plantilla de diseño</td> 
      <td> <p>Comience a escribir el nombre de la plantilla de diseño que desea que utilice el equipo y, a continuación, haga clic en ella cuando aparezca.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Especifique si se trata de un equipo Agile. Para obtener información sobre los equipos Agile y cómo administrar su trabajo, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo Agile</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Trabajar en ello</td> 
      <td> <p>Cambie el botón Trabajar en ello por el botón Iniciar. Cuando un usuario hace clic en Inicio, el estado del elemento se actualiza automáticamente.</p> <p>Para obtener más información sobre cómo configurar el botón Inicio, vea <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Inicio</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botón Listo</td> 
      <td> <p>Personalice el botón Listo. Para obtener más información, consulte:</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configurar el botón Listo para las tareas</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configurar el botón Listo para problemas</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar cambios**.
