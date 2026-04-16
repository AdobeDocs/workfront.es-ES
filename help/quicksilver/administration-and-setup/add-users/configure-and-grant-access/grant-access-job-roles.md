---
title: Conceder acceso a los roles
description: Como administrador de Adobe Workfront, puede definir el acceso de un usuario a las funciones del puesto en Workfront a través de su nivel de acceso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a5ba79da-37f3-43f8-a7e2-4ccd75b56fef
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 34%

---

# Conceder acceso a las funciones del puesto

Como administrador de Adobe Workfront, puede definir el acceso de un usuario a los roles a través del nivel de acceso del usuario, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Para obtener información sobre los roles, consulte [Crear y administrar roles](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>   <p>Estándar</p>
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

## Configurar el acceso de los usuarios a la edición de las funciones del puesto mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de los Roles y, a continuación, seleccione las facultades que desea conceder en **Ajuste la configuración**.

   >[!NOTE]
   >
   >**Ver** es el acceso predeterminado para los roles.

   ![Ajustar el acceso al rol](assets/job-role-access-view-fine-tune.png)

   Los usuarios con acceso para **Ver** pueden ver los roles existentes y, opcionalmente, hacer lo siguiente:

   * Ver tarifas de facturación en los roles de trabajo
   * Ver tasas de costo en roles de trabajo
   * Ver campos de finanzas generales (no relacionados con las tarifas de facturación o de costo) en los roles del puesto

   Los usuarios con acceso para **Editar** pueden ver y editar los roles existentes y, opcionalmente, hacer lo siguiente:

   * Crear nuevas funciones
   * Eliminar funciones
   * Editar tarifas de facturación en roles de trabajo
   * Editar las tasas de coste en los roles
   * Editar campos de finanzas generales (no relacionados con las tarifas de facturación o de costo) en los roles del puesto
   * Ver campos de tarifas de facturación de rol, tarifas de costo y finanzas generales

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a los puestos por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con los roles, consulte la sección [Roles](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#job-roles) del trabajo en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
