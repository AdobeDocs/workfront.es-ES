---
user-type: administrator
product-area: system-administration;user-management
keywords: añadir,usuarios,grupo,añadir,otro,asignar,administrador,eliminar,usuario,vista,funciones,miembros,exportar,pertenencia,datos
navigation-topic: create-and-manage-groups
title: Ver y administrar las suscripciones de un grupo
description: Como administrador de Adobe Workfront, puede ver, agregar, quitar, exportar, activar y desactivar miembros de cualquier grupo que administre. También puede editar sus perfiles, agregar actualizaciones a sus perfiles y asignarlos como administradores de grupo adicionales para el grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# Ver y administrar las suscripciones de un grupo

Como administrador de Adobe Workfront, puede ver, agregar, quitar, exportar, activar y desactivar miembros de cualquier grupo que administre. También puede editar sus perfiles, agregar actualizaciones a sus perfiles y asignarlos como administradores de grupo adicionales para el grupo.

Si hay algún grupo por encima de su grupo, sus administradores también pueden hacer esto por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Ver y administrar las suscripciones de un grupo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos**.

   En la lista que se muestra, los administradores de Workfront pueden ver todos los grupos y subgrupos. Los administradores de grupos solo pueden ver los grupos y subgrupos que administran.

1. Haga clic en el nombre del grupo que desee editar.
1. En la página que aparece, con **Miembros del grupo** seleccionado en el menú de la izquierda, realice una de las acciones siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar un usuario al grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Haga clic en <strong>Agregar miembros</strong> <img src="assets/add-icon-plus-in-circle.png">, empiece a escribir el nombre del usuario y, a continuación, selecciónelo cuando aparezca.</li> 
        <li value="2"> <p>Repita este proceso para cualquier otro usuario que desee agregar.</p> <p>Puede hacer clic en la X a la derecha de un nombre si decide no agregar ese usuario.</p> </li> 
        <li value="3">Haga clic en <strong>Listo</strong> cuando haya terminado.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar un usuario del grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione uno o varios nombres de usuario y haga clic en <strong>Quitar miembro</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Haga clic en <strong>Eliminar</strong> en el mensaje de advertencia que aparece.</p> <p>Puede encontrar el usuario que desea eliminar de la lista haciendo clic en <strong>Buscar personas y grupos en la lista</strong>, escriba su nombre en el cuadro y haga clic en el nombre cuando aparezca.</p> <p><b>NOTA</b>:  
          <ul> 
           <li>Si este grupo es el grupo principal de un usuario que desea eliminar, primero debe asignar otro grupo en el perfil del usuario. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Información general sobre los grupos de inicio</a> y <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a>.</li> 
           <li>Si el grupo solo tiene un administrador de grupo y necesita quitarlo del grupo, primero debe asignar otro administrador de grupo al grupo.</li> 
           <li>Un usuario puede pertenecer individualmente a un subgrupo, así como al grupo principal. Cuando elimina a alguien de un subgrupo, sigue formando parte del grupo principal. Del mismo modo, cuando los elimine del grupo principal, seguirán formando parte del subgrupo. Si no desea que un usuario tenga el acceso permitido para el grupo principal, debe quitar el usuario tanto de los subgrupos como del grupo principal, si están enumerados individualmente en ambos lugares.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Edición de la información de perfil de un usuario</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione uno o varios nombres de usuario y haga clic en <strong>Editar</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Cambie la información de perfil del usuario.</p> <p>Para obtener información sobre los cambios que puede realizar, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edición del perfil de un usuario</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar datos de pertenencia de usuario</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione uno o varios nombres de usuario y haga clic en <strong>Exportar</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exporte los datos como un archivo delimitado por PDF, Excel o tabulaciones.</p> <p>Para obtener más información sobre la exportación de datos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar datos</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver y editar las funciones de grupo de los miembros</td> 
      <td> <p>La variable <strong>Función del grupo</strong> enumera la función de cada miembro. Como administrador de grupo, puede hacer doble clic en la función de un miembro para cambiarla.</p> <p>Para los miembros del grupo que no son administradores de grupo, esta columna no es editable.</p> <p>Los administradores de grupos siempre están en la parte superior de la lista.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar un comentario a los miembros del grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione uno o varios nombres de usuario y haga clic en <strong>Actualizar</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Escriba el comentario.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activación de un usuario en Workfront</td> 
      <td>Seleccione uno o varios usuarios inactivos y haga clic en <strong>Activar usuario</strong> para activarlos en Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desactivación de un usuario en Workfront</td> 
      <td>Seleccione uno o varios usuarios activos y haga clic en <strong>Desactivar usuario</strong><img src="assets/deactivate-user.png"> para desactivarlos en Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordenar por columna</td> 
      <td>Haga clic en el encabezado de una columna para ordenar la lista según el contenido de dicha columna.</td> 
     </tr> 
    </tbody> 
   </table>
