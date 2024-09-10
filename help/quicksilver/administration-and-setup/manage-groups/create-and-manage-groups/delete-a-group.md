---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Eliminar un grupo
description: Puede eliminar un grupo que administre. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f92eb1f5-fe98-4c7e-8ef7-8ed7134db8d4
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 2%

---

# Eliminar un grupo

Puede eliminar un grupo que administre. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener información acerca de cómo eliminar un subgrupo, vea [Administrar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar un grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Seleccione el grupo que desea eliminar y haga clic en el icono Eliminar ![](assets/delete.png).

   >[!IMPORTANT]
   >
   >Cuando elimine un grupo o subgrupo, deberá conservar los usuarios, los elementos de trabajo y los subgrupos que estén asignados a él en ese momento. Para ayudarle a asegurarse de que se conservan, un mensaje le pedirá que reasigne los objetos del grupo a un grupo diferente en el paso siguiente.

1. En el cuadro **Eliminar grupo** que aparece, empiece a escribir y, a continuación, seleccione el nombre del grupo al que desea mover los miembros, elementos de trabajo y subgrupos del grupo que está eliminando.

   Para asegurarse de que está seleccionando el grupo correcto, pase el puntero sobre él y haga clic en el icono de información ![](assets/info-icon.png) que se muestra al lado. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.

1. Haga Clic En **Eliminarlos**.
