---
title: Crear un equipo desde el área Configuración
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Como administrador de Adobe Workfront, puede crear un equipo desde el área Configuración .
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# Crear un equipo desde el área Configuración

Como administrador de Adobe Workfront, puede crear un equipo desde el área Configuración . Para obtener información sobre los equipos, consulte [Información general sobre equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un administrador de grupos puede crear un equipo para un grupo que administre desde el área Configuración. Para obtener más información, consulte [Crear y modificar los equipos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un usuario con una licencia Plan también puede crear un equipo desde el área Personas. Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
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

## Crear un equipo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Equipos** y haga clic en **Nuevo equipo**.

1. En el **Nuevo equipo** que se muestra, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de equipo</td> 
      <td>Escriba un nombre para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo</td> 
      <td> <p>Si desea asociar el equipo con un grupo, empiece a escribir el nombre del grupo y, a continuación, seleccione el nombre cuando aparezca.</p> <p>Puede asegurarse de que está asociando el grupo correcto al equipo pasando el ratón por encima de él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Esto muestra información sobre herramientas acerca del grupo, como la jerarquía de grupos por encima de él y sus administradores.</p> <p><b>NOTA</b>: Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores del grupo pueden ir al área Equipos desde el menú principal y hacer clic en la flecha Cambiar equipos <img src="assets/switch-team-icon.png" alt="Icono Cambiar equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Miembros del equipo</td> 
      <td> <p>Empiece a escribir el nombre de un usuario que formará parte del equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable. Repita este proceso para agregar varios usuarios al equipo.</p> <p>No hay límite en cuanto a la cantidad de usuarios que puede agregar a un equipo. Sin embargo, se recomienda no tener un número excesivamente grande de usuarios en un equipo, ya que la gestión del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción para el equipo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calendario</td> 
      <td>Elija la ficha de calendario que aparecerá para este equipo.</td> 
     </tr> 
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Este es un equipo Agile</td> 
      <td>Seleccione este elemento si desea configurar este nuevo equipo para que sea un equipo ágil. Para obtener más información sobre los equipos ágiles, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo ágil</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trabajar en ello</td> 
      <td>Cambie el botón Trabajar en él a un botón Inicio . Cuando un usuario hace clic en Inicio, el estado del elemento se actualiza automáticamente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botón Listo</td> 
      <td>Seleccione el estado que desea establecer para los elementos cuando haga clic en el botón Listo .</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Crear equipo**.

## Propietarios del equipo

Al crear un equipo, se convierte en el propietario del equipo, de forma predeterminada.

Cuando cree un informe para equipos, puede ver los propietarios de los equipos de todos los equipos e incluir el campo Nombre del propietario en el informe. (Para obtener más información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
