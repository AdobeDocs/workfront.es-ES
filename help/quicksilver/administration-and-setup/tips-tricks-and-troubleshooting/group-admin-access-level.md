---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Los administradores del grupo deben tener un acceso más alto que los que administran
description: Si un administrador de grupo tiene permisos en su nivel de acceso inferiores a los que administra, no podrá ver, modificar ni asignar niveles de acceso inferiores.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Los administradores del grupo deben tener un acceso más alto que los que administran

Si un administrador de grupo tiene permisos en su nivel de acceso inferiores a los que administra, no podrá ver, modificar ni asignar niveles de acceso inferiores.

## Problema

Si a un administrador de grupo se le asigna un nivel de acceso de Planificador modificado con permisos de Vista para Equipos, pero a algunos usuarios se les asigna un nivel de acceso de Trabajador con permisos de Edición para Equipos, el administrador de grupo no podrá interactuar con el nivel de acceso de Trabajador modificado.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Esta lógica también se aplica al menú desplegable Ajustar la configuración . Ambos niveles de acceso pueden tener acceso de edición, pero la configuración del menú desplegable Ajustar la configuración debe ser mayor para el administrador del grupo.
> ![](assets/fine-tune-your-settings.png)

## Solución

Los administradores de grupos deben tener permisos más altos en todas las áreas del nivel de acceso que en las que administran.