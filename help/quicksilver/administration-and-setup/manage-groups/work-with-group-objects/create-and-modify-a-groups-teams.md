---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Crear y modificar los equipos de un grupo
description: Cuando visualiza un grupo que administre en el área de Grupos, puede visualizar y trabajar con los equipos asociados al grupo y a cualquiera de sus subgrupos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 89%

---

# Crear y modificar los equipos de un grupo

Cuando visualiza un grupo que administre en el área de Grupos, puede visualizar y trabajar con los equipos asociados al grupo y a cualquiera de sus subgrupos.

Si hay grupos por encima del suyo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener información sobre cómo los usuarios con una licencia de Plan pueden crear un equipo, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Para obtener información sobre cómo un administrador de Workfront puede crear un equipo, consulte [Crear un equipo desde el área de configuración](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

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
   <td role="rowheader">Licencia de Adobe Workfront</td>
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver, trabajar con y crear equipos para su grupo desde el área de Grupos

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea crear o modificar equipos.
1. En el panel izquierdo, haga clic en **Equipos** ![Equipos](assets/teams.png) para ver una lista de los equipos asociados con el grupo y con los subgrupos que pueda tener.

1. Realice una de las siguientes acciones:

   * **Añadir un equipo**: haga clic en **Nuevo equipo** y, a continuación, utilice las siguientes opciones para configurarlo:

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
       <td> <p> El sistema rellena el campo Grupo del nuevo equipo con el grupo que está visualizando. Si desea asociar el equipo a un grupo diferente, empiece a escribir el nombre del grupo y, a continuación, seleccione el nombre cuando aparezca.</p> <p>Puede asegurarse de que está asociando el grupo correcto al equipo, pasando el puntero por encima de él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Esta acción muestra la ayuda contextual con información sobre el grupo, como la jerarquía de los grupos que tiene por encima y sus administradores.</p> <p><b>NOTA</b>: Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupos de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores de grupos pueden ir al área de Equipos del menú principal y hacer clic en la flecha para cambiar de equipo <img src="assets/switch-team-icon.png" alt="Icono Cambiar de equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Integrantes del equipo</td> 
       <td> <p>Empiece a escribir el nombre de un usuario que desea incluir en el equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable. Repita este proceso para añadir varios usuarios al equipo.</p> <p>No hay límite en cuanto a la cantidad de usuarios que puede añadir a un equipo. Sin embargo, recomendamos no tener un número excesivamente grande de usuarios en un equipo, ya que la administración del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
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
       <td>Seleccione el estado que desea establecer para los elementos cuando se hace clic en el botón Listo.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Editar equipos**: selecciona al menos un equipo, haz clic en **el icono de edición** ![Editar icono](assets/edit-icon.png) y, a continuación, usa las siguientes opciones para configurarlo:

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
       <td> <p>Asocie el equipo a un grupo. Empiece a escribir el nombre del grupo y, a continuación, selecciónelo cuando aparezca.</p> <p>Puede asegurarse de que está asociando el grupo correcto al equipo, pasando el puntero por encima de él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Esta acción muestra la ayuda contextual con información sobre el grupo, como la jerarquía de los grupos que tiene por encima y sus administradores.</p> <p><b>NOTA</b>: Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupos de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores de grupos pueden ir al área de Equipos del menú principal y hacer clic en la flecha para cambiar de equipo <img src="assets/switch-team-icon.png" alt="Icono Cambiar de equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Propietario</td> 
       <td>Seleccione un propietario para el equipo.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Integrantes del equipo</td> 
       <td> <p>Añada los integrantes del equipo. Empiece a escribir el nombre de un usuario y, a continuación, seleccione el nombre cuando aparezca. Repita este proceso para añadir varios usuarios al equipo.</p> <p><b>SUGERENCIA</b>: No hay límite en cuanto a la cantidad de usuarios que puede añadir a un equipo. Sin embargo, recomendamos no tener un número excesivamente grande de usuarios en un equipo, ya que la administración del trabajo del equipo puede llegar a ser demasiado compleja.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descripción</td> 
       <td>Escriba una descripción para el equipo.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Plantilla de diseño</td> 
       <td> <p>Comience a escribir el nombre de la plantilla de diseño que desea que utilice el equipo y, a continuación, haga clic en él cuando aparezca.</p> <p>Al designar el equipo con esta plantilla de diseño como el equipo de inicio de los usuarios, todos los usuarios de este equipo verán las personalizaciones de esta plantilla de diseño.<br>Su configuración de plantilla de diseño individual anulará la configuración de la plantilla de diseño del equipo de inicio. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Especifique si se trata de un equipo ágil. Para obtener información sobre los equipos ágiles y cómo administrar su trabajo, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo ágil</a>.</td> 
       </tr> 
       <tr> 
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

   * **Eliminar equipos**: Seleccione al menos un equipo y haga clic en el icono Eliminar ![Icono Eliminar](assets/delete.png).
   * **Exporte la lista de equipos**: Haga clic en **Exportar** ![Icono de exportación](assets/export.png) y, a continuación, seleccione el formato de archivo que desee para la lista exportada.
