---
title: Ver el número de licencias asignadas y utilizadas en un grupo
description: Como administrador de Adobe Workfront, puede ver los recuentos de los tipos individuales de licencias que se utilizan actualmente en su grupo y en sus subgrupos. Esto resulta útil cuando necesita evaluar si desea redistribuir licencias.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Ver el número de licencias asignadas y utilizadas en un grupo

Como administrador de Adobe Workfront, puede ver los recuentos de los tipos individuales de licencias que se utilizan actualmente en su grupo y en sus subgrupos. Esto resulta útil cuando necesita evaluar si desea redistribuir licencias.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!IMPORTANT]
>
>La licencia de un usuario se cuenta en un grupo en particular solo si el grupo es el grupo de inicio del usuario.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver el número de licencias utilizadas en un grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo.
1. En la página que se muestra, en el área del encabezado cerca de la esquina superior derecha, vea el área de **Licencias en uso** para ver el número de licencias de **Plan** y **Trabajo** que se están usando actualmente.

   Si está viendo un grupo de nivel superior y el administrador de Workfront ha definido un número máximo de cada tipo de licencia para el grupo, también se muestran estos números. Por ejemplo, en el grupo siguiente, un máximo de 10 usuarios pueden tener una licencia de planificación y un máximo de 15 pueden tener una licencia de trabajo:

   ![](assets/licenses-used-allocated.png)

   Para obtener información sobre cómo un administrador de Workfront define un número máximo de licencias asignadas para un grupo, consulte la sección [Establecer el recuento máximo de licencias para un grupo de inicio](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) en el artículo [Administrar licencias disponibles en el sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Si el grupo que está viendo es un subgrupo, sólo puede ver el número de licencias que se están utilizando, no el número máximo de licencias asignadas para el grupo. Esto se debe a que los administradores de Workfront no definen un recuento máximo de licencias para un subgrupo.
   >
   >![](assets/subgroup-used-licenses-only.png)
   >

1. Para obtener recuentos independientes de cada tipo de licencia que se use actualmente en el grupo (incluidas Revisar y Solicitar), haga clic en el área de texto que se encuentra directamente debajo de **Licencias en uso:**

   ![](assets/click-text-to-see-more.png)

   El cuadro que aparece proporciona la misma información para los cuatro tipos de licencia de Workfront: Planificación, Trabajo, Revisión y Solicitud. En la parte inferior del cuadro, puede ver el número total de licencias que utilizan los miembros de este grupo o uno de sus subgrupos:

   ![](assets/more-license-info.png)

   En el caso de las licencias de revisión y solicitud, la columna Máx. siempre muestra Ilimitado.
