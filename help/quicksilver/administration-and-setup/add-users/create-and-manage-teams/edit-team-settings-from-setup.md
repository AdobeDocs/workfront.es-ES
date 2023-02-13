---
title: Editar la configuración de un equipo desde el área Configuración
description: Como administrador de Adobe Workfront, puede editar la configuración de un equipo desde el área Configuración. Puede agregar usuarios a un equipo, establecer la plantilla de diseño de un equipo y establecer cómo se registra el estado cuando un equipo completa los elementos de trabajo.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 2%

---

# Editar la configuración de un equipo desde el área Configuración

Como administrador de Adobe Workfront, puede editar la configuración de un equipo desde el área Configuración. Puede agregar usuarios a un equipo, establecer la plantilla de diseño de un equipo y establecer cómo se registra el estado cuando un equipo completa los elementos de trabajo.

Para obtener información sobre los equipos, consulte [Información general sobre equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un administrador de grupo puede editar la configuración de un equipo para un grupo que administra. Para obtener más información, consulte [Crear y modificar los equipos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un usuario con una licencia de Plan puede editar la configuración de un equipo desde el área Personas. Para obtener más información, consulte [Editar configuración de equipo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
>


## Requisitos de acceso

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Editar la configuración de un equipo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Equipos** en el panel izquierdo.
1. Seleccione un equipo y haga clic en **Editar** ![](assets/edit-icon.png).

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
       <td>Esta opción está habilitada de forma predeterminada para equipos nuevos y existentes. Desactívelo para desactivar el equipo. Para obtener más información, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Desactivación de un equipo</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Grupo</td> 
      <td> <p>Asocie el equipo a un grupo. Comience a escribir el nombre del grupo y, a continuación, seleccione el nombre cuando aparezca.</p> <p><b>NOTA</b>: Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores del grupo pueden ir al área Equipos desde el menú principal y hacer clic en la flecha Cambiar equipos <img src="assets/switch-team-icon.png" alt="Icono Cambiar equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> <p>Puede asegurarse de que está asociando el grupo correcto al equipo pasando el ratón por encima de él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Esto muestra información sobre herramientas acerca del grupo, como la jerarquía de grupos por encima de él y sus administradores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propietario</td> 
      <td>Seleccione un propietario para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Miembros del equipo</td> 
      <td> <p>Agregar y integrantes del equipo. Comience a escribir el nombre de un usuario y, a continuación, seleccione el nombre cuando aparezca. Repita este proceso para agregar varios usuarios al equipo.</p> 
      <p><b>SUGERENCIA</b>: Puede agregar cualquier número de usuarios a un equipo. Sin embargo, le recomendamos que no agregue un número excesivamente grande en un equipo, ya que la gestión del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Plantilla de diseño</td> 
      <td> <p>Empiece a escribir el nombre de la plantilla de diseño que desea que utilice el equipo y, a continuación, haga clic en ella cuando aparezca.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Especifique si se trata de un equipo ágil. Para obtener información sobre los equipos ágiles y cómo administrar su trabajo, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo ágil</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Trabajar en ello</td> 
      <td> <p>Cambie el botón Trabajar en él a un botón Inicio . Cuando un usuario hace clic en Inicio, el estado del elemento se actualiza automáticamente.</p> <p>Para obtener más información sobre cómo configurar el botón Inicio, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en él con un botón Inicio</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botón Listo</td> 
      <td> <p>Personalice el botón Listo . Para obtener más información, consulte:</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configuración del botón Listo para tareas</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configuración del botón Listo para problemas</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar cambios**.
