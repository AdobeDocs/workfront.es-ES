---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Eliminar perfiles de plantilla de horas
description: Puede eliminar un perfil de hoja de horas que ya no sea relevante.
author: Alina
feature: Timesheets
exl-id: 1fb39f74-205b-485e-9e8b-a2ab3f9f1ac4
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 29%

---

# Eliminar perfiles de plantilla de horas

<!--Audited:6/2025-->

Crear y asignar perfiles de hojas de horas a los usuarios garantiza la coherencia en la forma en que Adobe Workfront crea sus hojas de horas.

Puede eliminar un perfil de hoja de horas que ya no sea relevante.

Para obtener información sobre los perfiles de plantilla de horas, consulte [Crear, editar y asignar perfiles de plantilla de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar</p>
   O
   <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener acceso administrativo a las plantillas de horas. </p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminar perfiles de plantilla de horas

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Si está eliminando un perfil de hoja de horas a nivel de sistema, haga clic en **Hoja de horas y horas**.

   O

   Si está eliminando un perfil de hoja de horas de un grupo, haga clic en **Grupos** > haga clic en el nombre del grupo y, a continuación, haga clic en **Perfiles de hoja de horas**.
1. Seleccione al menos un perfil de hoja de horas que desee eliminar y luego haga clic en el icono **Más** ![](assets/more-icon.png) > **Eliminar** para el perfil de hoja de horas de todo el sistema

   O

   Haga clic en **Más** > **Eliminar** para el perfil de hoja de horas de nivel de grupo.
1. (Condicional) Si el perfil de hoja de horas ya está asignado a los usuarios, se muestra el cuadro **Perfil de hoja de horas de reemplazo**. Haga lo siguiente:
   1. Seleccione otro perfil de hoja de horas en la lista desplegable. El perfil de hoja de horas que está eliminando será reemplazado por el perfil de hoja de horas con el que lo reemplaza para todos los usuarios asignados. Las plantillas de horas se generarán según el perfil recién asignado en el siguiente ciclo de generación de plantillas de horas.
   1. Haga clic en **Eliminarlo** para confirmar la eliminación.
1. (Condicional) Si el perfil de hoja de horas no está asignado a los usuarios, se muestra el cuadro **Eliminar hoja de horas**.

   Haga clic en **Eliminar** para confirmar la eliminación.
