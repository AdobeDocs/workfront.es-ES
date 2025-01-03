---
title: Crear un equipo desde el área de configuración
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Como administrador de Adobe Workfront, puede crear un equipo desde el área Configuración.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 6409f8fa5072413444545d2d3a80935dc6e04b4c
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 96%

---

# Crear un equipo desde el área de configuración

Como administrador de Adobe Workfront, puede crear un equipo desde el área Configuración. Para obtener información sobre los equipos, consulte [Información general sobre los equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un administrador de grupos puede crear un equipo para un grupo que administre desde el área de configuración. Para obtener más información, consulte [Crear y modificar los equipos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un usuario con una licencia Standard o Plan también puede crear un equipo desde el área de Equipos. Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

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

## Crear un equipo

{{step-1-to-setup}}

1. Haga clic en **Equipos** y, a continuación, haga clic en **Nuevo equipo**.

1. En el cuadro **Nuevo equipo** que aparece, especifique la siguiente información:

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
      <td> <p>Si desea asociar el equipo con un grupo, empiece a escribir el nombre del grupo y, a continuación, selecciónelo cuando aparezca.</p> <p>Puede asegurarse de que está asociando el grupo correcto con el equipo, pasando el puntero por encima de él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Esta acción muestra la ayuda contextual con información sobre el grupo, como la jerarquía de los grupos que tiene por encima y sus administradores.</p> <p><b>NOTA</b>: Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupos de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores de grupos pueden ir al área de Equipos del menú principal y hacer clic en la flecha para cambiar de equipo <img src="assets/switch-team-icon.png" alt="Icono Cambiar de equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Este es un equipo Agile</td> 
      <td>Seleccione este elemento si desea configurar este nuevo equipo para que sea un equipo Agile. Para obtener más información sobre los equipos Agile, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Crear un equipo Agile</a>.</td> 
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

1. Seleccione **Crear equipo**.

## Propietarios de equipo

Cuando crea un equipo, se convierte en el propietario del equipo de forma predeterminada.

Puede ver los propietarios de todos los equipos cuando cree un informe para los equipos e incluya el campo Nombre del propietario en el informe. (Para obtener más información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
