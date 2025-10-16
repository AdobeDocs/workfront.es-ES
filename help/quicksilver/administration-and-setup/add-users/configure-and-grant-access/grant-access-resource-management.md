---
title: Conceder acceso a la administración de recursos
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a la administración de recursos en Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 35%

---

# Conceder acceso a Administración de recursos

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a la administración de recursos, como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el acceso de los usuarios a las herramientas de Administración de recursos mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** a la derecha de Administración de recursos y, a continuación, seleccione las capacidades que desea conceder en **Ajustar la configuración**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Editar prioridades y horas presupuestadas en el Planificador</td> 
      <td> <p>Permite a los usuarios con esta licencia hacer lo siguiente:</p> <p>Priorizar proyectos en el Planificador de recursos.</p> <p>Asignación presupuestaria para recursos en las herramientas de Planificación de recursos (el Planificador de recursos y la sección de Presupuestación de recursos en el Caso comercial de un proyecto).</p> <p>Esta opción está habilitada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrar conjuntos de recursos</td> 
      <td> <p>Permite a los usuarios con esta licencia crear, editar y eliminar conjuntos de recursos. Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Actualizar horas planificadas en el Distribuidor de cargas de trabajo</span> </td> 
      <td> <p>Permite a los usuarios con esta licencia actualizar las horas planificadas de los elementos de trabajo cuando actualizan las asignaciones de usuarios en el Distribuidor de cargas de trabajo. El número total de horas asignadas se convierte en las horas planificadas de los elementos de trabajo.</p> <p>Esta opción está desactivada de forma predeterminada.</p> <p> Para obtener más información, consulte <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a Administración de Recursos por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con la administración de recursos, vea la sección [Administración de recursos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a problemas compartidos

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Cuando comparte un objeto con otro usuario, los derechos del destinatario para presupuestar o ver la asignación de recursos en él están determinados por una combinación de tres cosas:

* Configuración del nivel de acceso del destinatario para la administración de recursos
* El acceso del usuario a los datos financieros, tal como se explica en [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Cualquier permiso para datos financieros que el usuario que comparte haya concedido para el objeto

Para obtener información acerca de los permisos que los usuarios pueden conceder a los datos financieros de un objeto al compartirlo, vea [Compartir permisos financieros en un objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
