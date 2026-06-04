---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Los Administradores De Grupo Deben Tener Más Acceso Que Los Que Administran
description: Si un administrador de grupo tiene permisos en su nivel de acceso inferiores a los que administra, no podrá ver, modificar ni asignar niveles de acceso inferiores.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 157
ht-degree: 47%

---

# Los administradores de grupo deben tener un acceso mayor que los que administran

Si un administrador de grupo tiene permisos en su nivel de acceso inferiores a los que administra, no podrá ver, modificar ni asignar niveles de acceso inferiores.

## Problema

Si a un administrador de grupos se le asignase un nivel de acceso de Planificador modificado con permisos de Visualización para Teams, pero a ciertos usuarios se les asignase un nivel de acceso de Trabajador con permisos de Edición para Teams, el administrador de grupos no podrá interactuar con el nivel de acceso de Trabajador modificado.

![Acceso modificado por el administrador del grupo](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Esta lógica también se aplica al menú desplegable Ajustar la configuración. Ambos niveles de acceso pueden tener acceso de edición, pero la configuración del menú desplegable Ajustar la configuración debe ser superior para el administrador del grupo.
> ![Ajustar la configuración](assets/fine-tune-your-settings.png)

## Solución

Los administradores de grupos deben tener permisos más altos en todas las áreas del nivel de acceso que los de aquellos que administran.
