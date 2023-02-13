---
title: Conceder acceso a la Administración de recursos
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a la Gestión de recursos en Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# Conceder acceso a la Administración de recursos

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a la Administración de recursos, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acceso

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuración del acceso de los usuarios a las herramientas de Administración de recursos mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono del engranaje ![](assets/gear-icon-settings.png) en el **Ver** o **Editar** a la derecha de Administración de recursos, luego seleccione las capacidades que desee conceder en **Ajustar la configuración**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Editar prioridades y horas presupuestadas en el Planificador</td> 
      <td> <p>Permite a los usuarios con esta licencia hacer lo siguiente:</p> <p>Priorice los proyectos en el Planificador de recursos.</p> <p>Asignación del presupuesto para recursos en las herramientas de planificación de recursos (la sección Planificador de recursos y Presupuestación de recursos en el Caso de negocio de un proyecto).</p> <p>Esta opción está activada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrar conjuntos de recursos</td> 
      <td> <p>Permite a los usuarios con esta licencia crear, editar y eliminar grupos de recursos. Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Actualizar horas planificadas en el Distribuidor de cargas de trabajo</span> </td> 
      <td> <p>Permite a los usuarios con esta licencia actualizar los elementos de horas de trabajo planificadas cuando actualizan las asignaciones de usuario en el equilibrador de carga de trabajo. El número total de horas asignadas se convierte en las horas previstas de los elementos de trabajo.</p> <p>Esta opción está desactivada de forma predeterminada.</p> <p> Para obtener más información, consulte <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Para configurar las opciones de acceso de otros objetos y áreas del nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando haya terminado, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a la administración de recursos por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con la Administración de recursos, consulte la sección [Gestión de recursos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a problemas compartidos

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Cuando comparte un objeto con otro usuario, los derechos del destinatario para presupuestar o ver la asignación de recursos en él están determinados por una combinación de 3 cosas:

* La configuración de nivel de acceso del destinatario para la Administración de recursos
* El acceso del usuario a los datos financieros, tal como se explica en [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Permisos para datos financieros que el usuario que comparte haya concedido para el objeto

Para obtener información sobre los permisos que los usuarios pueden conceder a los datos financieros de un objeto al compartirlo, consulte [Compartir permisos financieros en un objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
