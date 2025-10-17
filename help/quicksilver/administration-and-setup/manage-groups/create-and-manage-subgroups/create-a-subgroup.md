---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Crear un subgrupo
description: Puede crear un subgrupo en un grupo que administre para organizar usuarios y proyectos y para asignar derechos de acceso dentro de Adobe Workfront. Normalmente, los administradores de grupos administran grupos y subgrupos. Pueden utilizar la página Grupos para administrar sus grupos y subgrupos en un solo lugar.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 60%

---

# Crear un subgrupo

Puede crear un subgrupo en un grupo que administre para organizar usuarios y proyectos y para asignar derechos de acceso dentro de Adobe Workfront.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Sin embargo, normalmente los administradores de grupos administran grupos y subgrupos. Pueden utilizar la página Grupos para administrar sus grupos y subgrupos en un solo lugar. Para obtener información sobre cómo funcionan los grupos y subgrupos en Workfront, consulte [Información general de grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md) y [Información general de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Añadir un subgrupo

{{step-1-to-setup}}

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Seleccione el grupo o subgrupo existente al que desee añadir un nuevo subgrupo.
1. Haga clic en **Nuevo subgrupo**.
1. En el cuadro **Nuevo subgrupo** que aparece, escriba un **Nombre de grupo** para el subgrupo.
1. (Opcional) Introduzca la siguiente información:

   * **Descripción**: escriba una descripción para el subgrupo. Puede escribir hasta 512 caracteres.
   * **Está activo**: Esta opción está habilitada de manera predeterminada y hace que el grupo esté activo en la instancia de Workfront.

     En campos de escritura anticipada como el que se muestra a continuación, cuando los usuarios normales buscan un grupo para adjuntarlo a un objeto o compartirlo, solo se muestran en la lista los grupos activos.

     ![Campo de escritura anticipada para un grupo](assets/typeahead-for-group.png)

     Para optimizar esto para los usuarios, puede deshabilitar la opción **Está activo** para los grupos que no están actualmente en uso.

     Puede ver, filtrar y agrupar fácilmente la lista Grupos en función del estado activo o inactivo mediante este campo. Para obtener información acerca del uso de vistas, filtros y agrupaciones en listas, consulte [Elementos para la creación de informes: filtros, vistas y agrupaciones](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   * **Coordinador empresarial**: puede asignar un usuario como coordinador empresarial para un subgrupo que usted administre. Un coordinador empresarial es alguien que toma decisiones empresariales para el subgrupo. Para más información, consulte [Información general sobre el Coordinador empresarial](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

     Si la persona aún no es miembro del subgrupo, al añadir su nombre a este campo también se añade al grupo.

     >[!NOTE]
     >
     >* Para poder quitar al coordinador empresarial de un subgrupo, debe quitar su nombre del campo Coordinador empresarial.
     >* Si quita el nombre del campo Coordinador empresarial, ese usuario seguirá siendo miembro del subgrupo a menos que lo quite de él. Para obtener instrucciones sobre cómo quitar a alguien de un grupo, vea [Ver y administrar las pertenencias de un grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

   * **Miembros del grupo y administradores del grupo**: Para agregar usuarios y grupos como miembros del subgrupo, empiece a escribir el nombre de un usuario o grupo existente que desee agregar y, a continuación, seleccione el nombre cuando aparezca.

     Los usuarios y grupos que añada tendrán acceso a todos los objetos compartidos con el grupo.

     Un subgrupo hereda los administradores de grupo del grupo sobre él, por lo que es opcional especificar un usuario como administrador de grupo para un subgrupo. Puede asignar un miembro del grupo como administrador del grupo mediante el menú desplegable situado a la derecha del nombre del usuario.

   * **Buscar personas y grupos en la lista**: Si necesita encontrar un usuario o grupo ya asignado a este subgrupo, puede escribir su nombre aquí y seleccionarlo cuando aparezca.

1. Haga clic en **Guardar**.
