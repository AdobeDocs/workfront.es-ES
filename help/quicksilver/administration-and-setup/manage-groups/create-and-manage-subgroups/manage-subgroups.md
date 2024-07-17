---
user-type: administrator
product-area: system-administration;user-management
keywords: administrar, subagrupar, editar
navigation-topic: create-and-manage-subgroups
title: Administración de un subgrupo
description: Como administrador de grupo de un subgrupo, puede crear, mover, ver, editar, copiar, cambiar el nombre, exportar y eliminar el subgrupo. También puede convertir un subgrupo en un grupo de nivel superior eliminándolo de su grupo principal.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 1%

---

# Administración de un subgrupo

Como administrador de grupo de un subgrupo, puede crear, mover, ver, editar, copiar, cambiar el nombre, exportar y eliminar el subgrupo.

También puede convertir un subgrupo en un grupo de nivel superior eliminándolo de su grupo principal.

Si hay grupos por encima de su grupo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener más información acerca de los subgrupos, vea [Información general sobre los subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Crear, mover, ver, editar, copiar, cambiar el nombre, exportar o eliminar un subgrupo

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo que contiene el subgrupo en el que desea trabajar.

   O

   Si está moviendo uno o más subgrupos, haga clic en el nombre del grupo de destino (en un paso posterior, especificará qué subgrupos desea mover).

1. En el menú de la izquierda, haga clic en **Subgrupos**.

1. Realice una de las siguientes acciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Creación de un nuevo subgrupo</td> 
      <td> <p>Si desea crear el nuevo subgrupo un nivel por debajo del grupo que está viendo, haga clic en <strong>Agregar subgrupo</strong>.</p> <p>O bien, si desea crear el nuevo subgrupo debajo de otro subgrupo de la lista, selecciónelo y haga clic en <strong>Agregar s</strong><strong>subgrupo</strong>.</p> <p>Para obtener información acerca de las opciones que puede usar para configurar el subgrupo, vea la tabla en <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Crear un subgrupo</a>.</p> <p>Una jerarquía de grupo no puede superar los 15 niveles, pero un solo nivel puede tener un número ilimitado de grupos paralelos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Movimiento de un subgrupo </td> 
      <td> <p>Puede mover los subgrupos existentes a otro grupo que administre.</p> <p>Una jerarquía de grupo no puede superar los 15 niveles, pero un solo nivel puede tener un número ilimitado de grupos paralelos.</p> 
       <ol> 
        <li value="1"> <p>(Opcional) Seleccione un subgrupo para convertirlo en el grupo de destino.</p> <p>Si omite este paso, el grupo seleccionado en el paso 3 es el grupo de destino.</p> </li> 
        <li value="2">Haga clic en <strong>Agregar subgrupo</strong> &gt; <strong>Grupo existente</strong>.</li> 
        <li value="3"> <p>En el cuadro <strong>Grupo existente</strong> que aparece, empiece a escribir el nombre del subgrupo que desea mover.</p> <p>Los resultados que se muestran no contienen grupos por encima del grupo de destino.</p> <p>Para asegurarse de que está seleccionando el grupo correcto, pase el puntero sobre él y haga clic en el icono de información <img src="assets/info-icon.png"> que se muestra al lado. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.</p> </li> 
        <li value="4"> <p>Haga clic en el nombre del subgrupo que desee mover cuando vea que se muestra en la lista.</p> </li> 
        <li value="5"> <p>Repita los pasos c-d para cualquier otro subgrupo que desee mover al grupo de destino</p> </li> 
        <li value="6">Haga clic en <strong>Guardar</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Edición de un subgrupo</td> 
      <td> <p>Seleccione el subgrupo que desea editar y haga clic en el icono Editar <img src="assets/edit-icon.png">.</p> <p>Para obtener información acerca de las opciones que puede usar para configurar el subgrupo, vea la tabla de <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Crear un grupo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar uno o varios subgrupos</td> 
      <td> 
       <ol> 
        <li value="1">Seleccione el subgrupo o subgrupos que desee exportar.</li> 
        <li value="2">Haga clic en el icono Exportar <img src="assets/export.png"> y, a continuación, seleccione el formato de archivo que desee.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar un subgrupo para crear un nuevo grupo de nivel superior</td> 
      <td> <p>(Disponible solo para administradores de Workfront). Al copiar un subgrupo, se convierte en un grupo principal. Todos los miembros y subgrupos del grupo se copian con él. Los miembros del grupo conservan las asignaciones que tenían en el grupo original.</p> <p>Para obtener más información sobre cómo copiar un subgrupo, consulte <a href="#about-copying-a-subgroup" class="MCXref xref">Acerca de la copia de un subgrupo</a> en este artículo.</p> 
       <ol> 
        <li value="1">Seleccione un subgrupo y haga clic en el icono Copiar <img src="assets/copy-icon.png"> para crear un nuevo grupo de nivel superior basado en el grupo seleccionado.</li> 
        <li value="2"> <p>Configure las opciones del nuevo grupo.</p> <p>Para obtener ayuda con esta configuración, vea la tabla de la sección <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Crear un grupo de nivel superior copiando un grupo o subgrupo existente</a> en el artículo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Crear un grupo de nivel superior copiando un grupo o subgrupo existente</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminación de un subgrupo</td> 
      <td> <p><b>IMPORTANTE</b>: cuando elimine un grupo o subgrupo, deberá conservar los usuarios, los elementos de trabajo y los subgrupos que estén asignados a él en ese momento. Para ayudarle a asegurarse de que se conservan, un mensaje le pedirá que reasigne los objetos del grupo a un grupo diferente en el paso siguiente.</p> 
       <ol> 
        <li value="1">Seleccione el subgrupo y haga clic en el icono Eliminar <img src="assets/delete.png">.</li> 
        <li value="2">En el cuadro <strong>Eliminar grupo</strong> que aparece, empiece a escribir y, a continuación, seleccione el nombre del grupo al que desea mover los miembros, elementos de trabajo y subgrupos del grupo que está eliminando.</li> 
        <li value="3">Haga Clic En <strong>Eliminarlos</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Al administrar un grupo que contiene subgrupos, resulta útil poder identificar y filtrar los datos de todo el grupo y de todos sus subgrupos. Para ello, utilice el campo Identificador de elemento principal superior de un informe o lista.
>
>Por ejemplo, imaginemos que administra un departamento de marketing grande y desea una lista de todos los proyectos en los que está trabajando todo el departamento.
>
>En Workfront, este departamento de marketing está representado por un grupo denominado Marketing, con 3 subgrupos llamados Marketing de campo, Marketing de producto y Marketing digital. Para enumerar los proyectos que pertenecen a todo el departamento de marketing (los 4 grupos), puede crear un filtro para el área de proyectos con la siguiente regla de filtro:
>
>```
>Group: Top Parent ID > Equal > Marketing
>```
>
>También puede utilizar el campo Nombre principal superior para identificar los datos asociados con un grupo de nivel superior, pero solo en Vistas, no en Filtros o Agrupaciones.

## Eliminar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior

Puede convertir un subgrupo en un grupo de nivel superior eliminándolo de su grupo principal.

>[!TIP]
>
>Cuando desactiva un grupo que tiene subgrupos debajo de él, esos subgrupos también quedan inactivos. Si desea que uno de ellos esté activo, puede utilizar estas instrucciones para eliminarlo de su grupo principal y luego reactivarlo.
>
>Para obtener instrucciones sobre cómo desactivar y reactivar grupos, consulte las secciones [Ver y administrar los detalles de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) y [Ver y administrar los detalles de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) en el artículo [Ver y administrar los detalles de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Seleccione el grupo principal del grupo que desea convertir en un grupo de nivel superior y, a continuación, haga clic en el icono Editar ![](assets/edit-icon.png).
1. En el cuadro **Editar grupo** que aparece, en **Miembros del grupo y Administradores del grupo**, empiece a escribir el nombre del subgrupo que desea convertir en grupo de nivel superior y, a continuación, haga clic en la X a la derecha de su nombre cuando aparezca.
1. Haga clic en **Guardar**.

## Ver y administrar los miembros del subgrupo de un grupo

Cuando está viendo la página principal de un grupo que administra, puede ver y administrar todos los usuarios de los subgrupos del grupo. Para obtener instrucciones, vea [Ver y administrar miembros de subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Copia de un subgrupo {#about-copying-a-subgroup}

Tenga en cuenta lo siguiente cuando copie un subgrupo.

* Si un subgrupo que copia tiene sus propios subgrupos, estos se incluyen en la copia y sus nombres tienen el siguiente formato:

  ```
  Original subgroup name (Copy)
  ```

* Cualquier subgrupo que pertenezca a un grupo público también es público, por lo que cualquier usuario con acceso de edición de usuario, dentro o fuera del grupo, puede agregar usuarios al subgrupo.
