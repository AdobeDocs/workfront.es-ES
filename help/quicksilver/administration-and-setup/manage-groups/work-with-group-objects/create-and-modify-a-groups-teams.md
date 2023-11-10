---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Crear y modificar los equipos de un grupo
description: Cuando visualice un grupo que administre en el área de Grupos, podrá visualizar y trabajar con los equipos asociados al grupo y a cualquiera de sus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 6f9eddd46430990e11d5d661ea09f0595a9acebc
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# Crear y modificar los equipos de un grupo

Cuando visualice un grupo que administre en el área de Grupos, podrá visualizar y trabajar con los equipos asociados al grupo y a cualquiera de sus subgrupos.

Si hay grupos por encima de su grupo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener información sobre cómo los usuarios con una licencia de planificación pueden crear un equipo, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Para obtener información sobre cómo un administrador de Workfront puede crear un equipo, consulte [Cree un equipo desde el área de Configuración](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Vea, trabaje con y cree equipos para su grupo desde el área de Grupos

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar equipos.
1. En el panel izquierdo, haga clic en **Equipos** ![](assets/teams.png) para enumerar los equipos asociados con el grupo y con los subgrupos que pueda tener.

1. Realice una de las siguientes acciones:

   * **Agregar un equipo**: haga clic en **Nuevo equipo** y, a continuación, utilice las siguientes opciones para configurarlo:

   <!-- WRITER please check table below. I stripped out wonky conditions-->

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
       <td> <p> El sistema rellena el campo Grupo del nuevo equipo con el grupo que está visualizando. Si desea asociar el equipo con otro grupo, empiece a escribir el nombre del grupo y, a continuación, seleccione el nombre cuando aparezca.</p> <p>Puede asegurarse de que está asociando el grupo correcto con el equipo pasando el puntero sobre él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a ella. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.</p> <p><b>NOTA</b>: cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores del grupo pueden ir al área de Equipos desde el menú principal y hacer clic en la flecha para cambiar de equipo <img src="assets/switch-team-icon.png" alt="Icono Cambiar equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Miembros del equipo</td> 
       <td> <p>Empiece a escribir el nombre de un usuario para que esté en el equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable. Repita este proceso para agregar varios usuarios al equipo.</p> <p>No hay límite en cuanto a la cantidad de usuarios que puede añadir a un equipo. Sin embargo, se recomienda no tener un número excesivamente grande de usuarios en un equipo, ya que la administración del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descripción</td> 
       <td>Escriba una descripción para el equipo.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Calendario</td> 
       <td>Elija la ficha de calendario que aparecerá para este equipo.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Trabajar en ello</td> 
       <td>Cambie el botón Trabajar en ello por el botón Iniciar. Cuando un usuario hace clic en Inicio, el estado del elemento se actualiza automáticamente.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Botón Listo</td> 
       <td>Seleccione el estado que desea establecer para los elementos cuando se haga clic en el botón Listo.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Editar equipos**: seleccione al menos un equipo y haga clic en **el** Icono Editar ![](assets/edit-icon.png)y, a continuación, utilice las siguientes opciones para configurarlo:

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
       <td> <p>Asocie el equipo a un grupo. Empiece a escribir el nombre del grupo y, a continuación, selecciónelo cuando aparezca.</p> <p>Puede asegurarse de que está asociando el grupo correcto con el equipo pasando el puntero sobre él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a ella. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.</p> <p><b>NOTA</b>: cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores del grupo pueden ir al área de Equipos desde el menú principal y hacer clic en la flecha para cambiar de equipo <img src="assets/switch-team-icon.png" alt="Icono Cambiar equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Propietario</td> 
       <td>Seleccione un propietario para el equipo.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Miembros del equipo</td> 
       <td> <p>Agregar y agregar integrantes del equipo. Empiece a escribir el nombre de un usuario y, a continuación, seleccione el nombre cuando aparezca. Repita este proceso para agregar varios usuarios al equipo.</p> <p><b>SUGERENCIA</b>: no hay límite en cuanto a la cantidad de usuarios que puede añadir a un equipo. Sin embargo, se recomienda no tener un número excesivamente grande de usuarios en un equipo, ya que la administración del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descripción</td> 
       <td>Escriba una descripción para el equipo.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Plantilla de diseño</td> 
       <td> <p>Comience a escribir el nombre de la plantilla de diseño que desea que utilice el equipo y, a continuación, haga clic en ella cuando aparezca.</p> <p>Al designar el equipo con esta plantilla de diseño como el equipo de inicio de los usuarios, todos los usuarios de este equipo verán las personalizaciones de esta plantilla de diseño.<br>La configuración individual de la plantilla de diseño anula la configuración de la plantilla de diseño del equipo de inicio. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Especifique si se trata de un equipo Agile. Para obtener información sobre los equipos Agile y cómo administrar su trabajo, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo Agile</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Trabajar en ello</td> 
       <td> <p>Cambie el botón Trabajar en ello por el botón Iniciar. Cuando un usuario hace clic en Inicio, el estado del elemento se actualiza automáticamente.</p> <p>Para obtener más información sobre cómo configurar el botón Start, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Iniciar</a>.</p> </td> 
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

   * **Eliminar equipos**: seleccione al menos un equipo y haga clic en el icono Eliminar ![](assets/delete.png).
   * **Exportar la lista de equipos**: haga clic en **Exportar** ![](assets/export.png), luego seleccione el formato de archivo que desee para la lista exportada.
