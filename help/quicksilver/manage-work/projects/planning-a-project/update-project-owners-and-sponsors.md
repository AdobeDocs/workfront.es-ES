---
product-area: projects
navigation-topic: plan-a-project
title: Actualizar propietarios y patrocinadores de proyectos
description: Al crear un proyecto en Adobe Workfront, se establece automáticamente como Propietario del proyecto. Puede actualizar este campo con otro usuario. También puede actualizar el campo Patrocinador de proyecto de un proyecto.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YqTw5b0p4p605v7O0wVx99A7gLvJYF8xEPtthwW0CWc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 88%

---

# Actualizar propietarios y patrocinadores de proyectos

<!--Audited: 07/2024-->

Al crear un proyecto en Adobe Workfront, se establece automáticamente como Propietario del proyecto. Puede actualizar este campo con otro usuario. También puede actualizar el campo Patrocinador de proyecto de un proyecto.

Para obtener información acerca de los propietarios y patrocinadores de proyectos, consulte [Información general sobre los propietarios y patrocinadores de proyectos](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>Puede identificar a un propietario y a un patrocinador para una plantilla. Cuando crea un proyecto a partir de esa plantilla, el propietario de la plantilla se convierte en el propietario del proyecto y el patrocinador de la plantilla se convierte en el patrocinador del proyecto.
>
>Si la plantilla no tiene un Propietario, el usuario que crea el proyecto a partir de la plantilla se convierte en el Propietario del proyecto.
>
>Para obtener información sobre cómo editar plantillas, consulte [Editar plantillas del proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Edición de permisos en un proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Actualizar el propietario del proyecto de un proyecto

Cuando se añade un usuario como Propietario del proyecto de un proyecto, Workfront le otorga automáticamente permisos para ver el proyecto.

1. Vaya al proyecto que desee actualizar.
1. Haga clic en **Detalles del proyecto** en el panel de navegación izquierdo.
1. Haga clic en el icono **Editar** ![Editar icono](assets/qs-edit-icon.png) en la esquina superior derecha del área de Detalles del proyecto y, a continuación, haga clic en **Información general**.

1. Especifique el nombre de un usuario para el campo **Propietario del Proyecto**.

   Solo los usuarios activos pueden especificarse como Propietarios del proyecto.

1. Haga clic en **Guardar cambios**.

   El Propietario del proyecto se actualiza en el encabezado del proyecto y en el área Detalles del proyecto.

   ![Propietario destacado de las partes interesadas del proyecto](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Actualizar el Patrocinador del Proyecto de un proyecto.

Cuando añada un usuario como patrocinador del proyecto de un proyecto, Workfront le otorga automáticamente permisos para ver el proyecto.

>[!TIP]
>
>Si el usuario que añadir como patrocinador del proyecto es administrador del sistema, no se añadirá a la lista de uso compartido del proyecto.

1. Vaya al proyecto que desee actualizar.
1. Haga clic en **Detalles del proyecto** en el panel de navegación izquierdo.
1. Haga clic en el icono **Editar** ![Editar icono](assets/qs-edit-icon.png) en la esquina superior derecha del área de Detalles del proyecto y, a continuación, haga clic en **Información general**.

1. Especifique el nombre de un usuario para el campo **Patrocinador de proyecto**.

   Solo los usuarios activos pueden ser especificados como patrocinadores del proyecto.

1. Haga clic en **Guardar cambios**.

   El patrocinador del proyecto se actualiza en el área de Detalles del proyecto.

   ![Se destacó el patrocinador de las partes interesadas del proyecto](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
