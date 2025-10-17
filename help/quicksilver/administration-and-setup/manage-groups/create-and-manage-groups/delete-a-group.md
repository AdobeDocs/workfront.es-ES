---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Eliminar un grupo
description: Puede eliminar un grupo que administre. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f92eb1f5-fe98-4c7e-8ef7-8ed7134db8d4
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 77%

---

# Eliminar un grupo

Puede eliminar un grupo que administre. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener información sobre la eliminación de un subgrupo, consulte [Administrar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md).

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

## Eliminar un grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Seleccione el grupo que desee eliminar y, a continuación, haga clic en el icono Eliminar ![Eliminar](assets/delete.png).

   >[!IMPORTANT]
   >
   >Cuando elimine un grupo o subgrupo, deberá conservar los usuarios, los elementos de trabajo y los subgrupos que estén asignados a él en ese momento. Para ayudarle a asegurarse de que se conservan, un mensaje le pedirá que reasigne los objetos del grupo a un grupo diferente en el paso siguiente.

1. En el cuadro **Eliminar grupo** que aparece, empiece a escribir y, a continuación, seleccione el nombre del grupo al que desea mover los miembros, elementos de trabajo y subgrupos del grupo que está eliminando.

   Para asegurarse de que está seleccionando el grupo correcto, pase el puntero sobre él y haga clic en el icono de información ![Icono de información](assets/info-icon.png) que se muestra junto a él. Esta acción muestra la ayuda contextual con información sobre el grupo, como la jerarquía de los grupos que tiene por encima y sus administradores.

1. Haga clic en **Eliminarlos**.
