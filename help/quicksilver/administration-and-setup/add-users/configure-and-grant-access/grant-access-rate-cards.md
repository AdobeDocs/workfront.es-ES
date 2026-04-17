---
title: Conceder acceso a las tarjetas de tarifas
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede definir el acceso de un usuario a los datos financieros en Workfront a través de su nivel de acceso.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
exl-id: b21e65d3-3c9f-4f3d-95d3-de4c09199622
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 49%

---

# Conceder acceso a las tarjetas de tarifa

Como administrador de Adobe Workfront, puede definir el acceso de un usuario a las tarjetas de tarifa a través del nivel de acceso del usuario, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Para obtener información sobre las tarjetas de tarifas, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Estándar</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para conceder acceso a las tarjetas de tarifa

Tenga en cuenta lo siguiente al conceder a los usuarios acceso a las tarjetas de clasificación en Workfront:

* Los usuarios deben tener acceso de edición a las tarjetas de tarifas, los proyectos y los datos financieros para adjuntar una tarjeta de tarifas a un proyecto.
* Los usuarios sin acceso a las tarjetas de tarifas y acceso de edición a los datos financieros no pueden adjuntar una tarjeta de tarifas a un proyecto, pero pueden editar otras tarifas de facturación en el proyecto que provengan de otras fuentes.

## Configurar el acceso de los usuarios a las tarjetas de clasificación mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haz clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de las tarjetas de tarifa y, a continuación, selecciona las facultades que deseas conceder en **Ajustar la configuración**.

   ![Ajustar el acceso a la tarjeta de tarifas](assets/rate-card-access-fine-tune.png)

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a tarjetas de tarifas compartidas

Puede compartir una tarjeta de tarifa con otros usuarios otorgándoles permisos, tal como se explica en [Compartir una tarjeta de tarifa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md).

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario sobre él se determinan mediante una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* Configuración del nivel de acceso del destinatario para el tipo de objeto
