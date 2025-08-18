---
user-type: administrator
product-area: system-administration;user-management
keywords: add,users,group,add,another,assign,administrator,remove,user,view,roles,members,export,membership,data
navigation-topic: create-and-manage-groups
title: Ver y administrar las suscripciones de un grupo
description: Como administrador de Adobe Workfront puede ver, añadir, quitar, exportar, activar y desactivar miembros de cualquier grupo que administre. También puede editar y añadir actualizaciones a sus perfiles y asignarlos como administradores del grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: 2096cfa0fd4d0e7eeb85dbf00668dc1dd7fb1d99
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 91%

---

# Ver y administrar los miembros de un grupo

Como administrador de Adobe Workfront puede ver, añadir, quitar, exportar, activar y desactivar miembros de cualquier grupo que administre. También puede editar y añadir actualizaciones a sus perfiles y asignarlos como administradores del grupo.

Si hay grupos por encima del suyo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

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
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver y administrar los miembros de un grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.

   En la lista que se muestra, los administradores de Workfront pueden ver todos los grupos y subgrupos. Los administradores de grupos solo pueden ver los grupos y subgrupos que administran.

1. Haga clic en el nombre del grupo que desea editar.
1. En la página que aparece, con **Miembros del grupo** seleccionados en el menú de la izquierda, realice una de las siguientes acciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Añadir un usuario al grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Haga clic en <strong>Añadir miembros</strong> <img src="assets/add-icon-plus-in-circle.png">, escriba el nombre del usuario y selecciónelo cuando aparezca.</li> 
        <li value="2"> <p>Repita esto para cualquier otro usuario que desee añadir.</p> <p>Puede hacer clic en la X a la derecha de un nombre de usuario si decide no añadirlo.</p> </li> 
        <li value="3">Haga clic en <strong>Listo</strong> cuando termine.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quitar un usuario del grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione uno o varios nombres de usuario y haga clic en <strong>Quitar miembro</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Haga clic en <strong>Quitar</strong> en el mensaje de advertencia que aparece.</p> <p>Puede encontrar un usuario que desee quitar de la lista haciendo clic en <strong>Buscar personas y grupos en la lista</strong> si escribe su nombre en el cuadro y hace clic en él cuando aparezca.</p> <p><b>NOTA</b>:  
          <ul> 
           <li>Si este grupo es el de inicio del usuario que desea quitar, primero debe asignar otro Grupo de inicio en el perfil del usuario. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Información general sobre los grupos de inicio</a> y <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</li> 
           <li>Si el grupo solo tiene un administrador de grupos y necesita quitarlo, primero debe asignar otro administrador al grupo.</li> 
           <li>Un usuario puede pertenecer individualmente a un subgrupo, así como al grupo principal. Cuando quita a alguien de un subgrupo, este sigue formando parte del grupo principal. Asimismo, cuando los quita del grupo principal, siguen formando parte del subgrupo. Si no desea que se permita el acceso de un usuario al grupo principal, debe quitarlo de los subgrupos y el grupo principal, si aparece en ambos lugares.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar la información de perfil de un usuario</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione uno o más nombres de usuario y luego haga clic en <strong>Editar</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Cambiar la información de perfil del usuario.</p> <p>Para obtener información sobre los cambios que puede realizar, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar datos de abono de usuario</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione uno o varios nombres de usuario y, a continuación, haga clic en <strong>Exportar</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exporte los datos como un archivo PDF, Excel o delimitado por tabuladores.</p> <p>Para obtener más información sobre cómo exportar los datos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar datos</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver y editar las funciones de grupo de los abonados</td> 
      <td> <p>La columna <strong>Función de grupo</strong> enumera la función de cada abonado. Como administrador de grupos, puede hacer doble clic en la función de un abonado para cambiarla.</p> <p>Para los abonados del grupo que no son administradores de grupos, esta columna no se puede editar.</p> <p>Los administradores de grupos siempre están en la parte superior de la lista.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar un comentario a los abonados del grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Seleccione al menos un miembro del grupo y luego haga clic en <strong>Enviar actualización al usuario</strong> en la barra de herramientas.</li> 
        <li value="2"><p>Escriba el comentario que desee enviar a los usuarios y al área de Actualizaciones de sus perfiles de usuario.</p>
        <p>Para obtener más información, vea <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Enviar mensajes directos a otros usuarios</a>.</p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activar un usuario en Workfront</td> 
      <td>Seleccione uno o más usuarios inactivos y haga clic en <strong>Activar usuario</strong> para activarlos en Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desactivar un usuario en Workfront</td> 
      <td>Seleccione uno o más usuarios activos y haga clic en <strong>Desactivar usuario</strong><img src="assets/deactivate-user.png"> para desactivarlos en Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordenar por columna</td> 
      <td>Haga clic en el encabezado de una columna para ordenar la lista por el contenido de esa columna.</td> 
     </tr> 
    </tbody> 
   </table>
