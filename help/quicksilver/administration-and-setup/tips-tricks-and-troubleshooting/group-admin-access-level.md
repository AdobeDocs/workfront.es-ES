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
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 59%

---

# Los administradores de grupo deben tener un acceso mayor que los que administran

Si un administrador de grupo tiene permisos en su nivel de acceso inferiores a los que administra, no podrá ver, modificar ni asignar niveles de acceso inferiores.

## Problema

Si a un administrador de grupos se le asignase un nivel de acceso de Planificador modificado con permisos de Visualización para Teams, pero a ciertos usuarios se les asignase un nivel de acceso de Trabajador con permisos de Edición para Teams, el administrador de grupos no podrá interactuar con el nivel de acceso de Trabajador modificado.

![Acceso modificado por el administrador del grupo](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Esta lógica también se aplica al menú desplegable Ajustar la configuración. Ambos niveles de acceso podrán tener acceso de Edición, pero la configuración del menú desplegable Ajustar la configuración deberá ser superior para el administrador de grupos.
> ![Ajustar la configuración](assets/fine-tune-your-settings.png)

## Solución

Los administradores de grupos deben tener permisos más altos en todas las áreas del nivel de acceso que los de aquellos que administran.
