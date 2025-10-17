---
user-type: administrator
product-area: system-administration;user-management
keywords: administrar, subagrupar, editar
navigation-topic: create-and-manage-subgroups
title: Administrar un subgrupo
description: Como administrador de grupo de un subgrupo, puede crear, mover, ver, editar, copiar, cambiar el nombre, exportar y eliminar el subgrupo. También puede convertir un subgrupo en un grupo de nivel superior eliminándolo de su grupo principal.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 52%

---

# Administrar un subgrupo

Como administrador de grupo de un subgrupo, puede crear, mover, ver, editar, copiar, cambiar el nombre, exportar y eliminar el subgrupo.

También puede convertir un subgrupo en un grupo de nivel superior eliminándolo de su grupo principal.

Si hay grupos por encima del suyo, sus administradores también pueden hacer estas cosas por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener más información acerca de los subgrupos, consulte [Información general sobre los subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

>[!TIP]
>
>Al administrar un grupo que contiene subgrupos, resulta útil poder identificar y filtrar los datos de todo el grupo y de todos sus subgrupos. Para ello, utilice el campo Identificador de elemento principal superior de un informe o lista.
>
>Por ejemplo, imaginemos que administra un departamento de marketing grande y desea una lista de todos los proyectos en los que está trabajando todo el departamento.
>
>En Workfront, este departamento de marketing está representado por un grupo denominado Marketing, con 3 subgrupos llamados Marketing de campo, Marketing de producto y Marketing digital. Para enumerar los proyectos que pertenecen a todo el departamento de marketing (los 4 grupos), puede crear un filtro para el área de proyectos con la siguiente regla de filtro:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>También puede utilizar el campo Nombre principal superior para identificar los datos asociados a un grupo de nivel superior, pero solo en vistas, no en filtros o agrupaciones.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un subgrupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo al que desee agregar un subgrupo.
1. En el menú de la izquierda, haga clic en **Subgrupos**.
1. Para crear un nuevo subgrupo un nivel por debajo del grupo que está viendo, haga clic en **Agregar subgrupo**.

   O bien, si desea crear el nuevo subgrupo debajo de otro subgrupo de la lista, selecciónelo y haga clic en **Agregar subgrupo**.

   Para obtener información sobre las opciones que puede usar para configurar el subgrupo, vea [Crear un subgrupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

   Una jerarquía de grupo no puede superar los 15 niveles, pero un solo nivel puede tener un número ilimitado de grupos paralelos.

## Mover un subgrupo

Puede mover los subgrupos existentes a otro grupo que administre.

Una jerarquía de grupo no puede superar los 15 niveles, pero un solo nivel puede tener un número ilimitado de grupos paralelos.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo de destino (en un paso posterior, especificará qué subgrupos desea mover).
1. En el menú de la izquierda, haga clic en **Subgrupos**.
1. (Opcional) Seleccione un subgrupo para convertirlo en el grupo de destino.

   Si omite este paso, el grupo seleccionado en el paso 3 es el grupo de destino.

1. Haga clic en **Agregar subgrupo > Grupo existente**.
1. En el cuadro **Grupo existente** que aparece, empiece a escribir el nombre del subgrupo que desea mover.

   Los resultados que se muestran no contienen grupos por encima del grupo de destino.

   Para asegurarse de que está seleccionando el grupo correcto, pase el puntero sobre él y haga clic en el icono de información ![icono de información](assets/info-icon.png) que se muestra junto a él. Esta acción muestra la ayuda contextual con información sobre el grupo, como la jerarquía de los grupos que tiene por encima y sus administradores.

1. Seleccione el nombre del subgrupo que desee mover cuando lo encuentre en la lista.
1. Repita los pasos del 7 al 8 para cualquier otro subgrupo que desee mover al grupo de destino.
1. Haga clic en **Guardar**.

## Editar un subgrupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo que contiene el subgrupo que desea editar.
1. En el menú de la izquierda, haga clic en **Subgrupos**.
1. Seleccione el subgrupo que desee editar y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).

   Para obtener información sobre las opciones que puede usar para configurar el subgrupo, vea [Crear un subgrupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Copia de un subgrupo

>[!NOTE]
>
>Solamente un administrador del sistema puede copiar un subgrupo.

Al copiar un subgrupo, se convierte en un grupo principal. Todos los miembros y subgrupos del grupo se copian con él. Los miembros del grupo conservan todas las asignaciones que tenían en el grupo original.

Tenga en cuenta lo siguiente al copiar un subgrupo:

* Si un subgrupo que copia tiene sus propios subgrupos, estos se incluyen en la copia y sus nombres tienen el siguiente formato:

  `Original subgroup name (Copy)`

* Cualquier subgrupo que pertenezca a un grupo público también es público, por lo que cualquier usuario con acceso para editar usuarios, dentro o fuera del grupo, puede agregar usuarios al subgrupo.

Para copiar un subgrupo:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo que contiene el subgrupo que desea copiar.
1. En el menú de la izquierda, haga clic en **Subgrupos**.
1. Seleccione un subgrupo y luego haga clic en el icono **Copiar** ![Copiar icono](assets/copy-icon.png) para crear un nuevo grupo de nivel superior basado en el grupo seleccionado.
1. Configure las opciones del nuevo grupo.

   Para obtener ayuda con esta configuración, consulte [Crear un grupo de nivel superior copiando un grupo o subgrupo existente](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) en el artículo [Crear un grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Haga clic en **Crear grupo**.

## Exportación de un subgrupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo que contiene el subgrupo que desea exportar.
1. En el menú de la izquierda, haga clic en **Subgrupos**.
1. Seleccione el subgrupo o subgrupos que desee exportar.
1. Haga clic en el icono **Exportar** ![Icono de exportar](assets/export.png) y, a continuación, seleccione el formato de archivo que desee.

## Eliminar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior

Puede convertir un subgrupo en un grupo de nivel superior eliminándolo de su grupo principal.

>[!TIP]
>
>Cuando desactiva un grupo que tiene subgrupos debajo de él, esos subgrupos también quedan inactivos. Si desea que uno de ellos esté activo, puede utilizar estas instrucciones para eliminarlo de su grupo principal y luego reactivarlo.
>>Para obtener instrucciones sobre cómo desactivar y reactivar grupos, consulte [Desactivar o reactivar un grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).
1. Seleccione el grupo principal del subgrupo que desea convertir en un grupo de nivel superior y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).
1. En el cuadro **Editar grupo** que aparece, empiece a escribir el nombre del subgrupo que desea que sea un grupo de nivel superior en el campo **Buscar** (en **Miembros del grupo y Administradores del grupo**) y, a continuación, haga clic en la X a la derecha de su nombre cuando aparezca.
1. Haga clic en **Guardar**.

## Eliminar un subgrupo

>[!IMPORTANT]
>
>Cuando elimine un grupo o subgrupo, deberá conservar los usuarios, los elementos de trabajo y los subgrupos que estén asignados a él en ese momento. Para ayudarle a asegurarse de que se conservan, un mensaje le pedirá que reasigne los objetos del grupo a un grupo diferente.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo que contiene el subgrupo que desea eliminar.
1. En el menú de la izquierda, haga clic en **Subgrupos**.
1. Seleccione el subgrupo y haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png).

   En el cuadro **Eliminar grupo** que aparece, empiece a escribir y, a continuación, seleccione el nombre del grupo al que desea mover los miembros, elementos de trabajo y subgrupos del grupo que está eliminando.

1. Haga clic en **Eliminarlo**.

## Ver y administrar los miembros del subgrupo de un grupo

Cuando está viendo la página principal de un grupo que administra, puede ver y administrar todos los usuarios de los subgrupos del grupo. Para obtener instrucciones, consulte [Ver y administrar miembros de subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

