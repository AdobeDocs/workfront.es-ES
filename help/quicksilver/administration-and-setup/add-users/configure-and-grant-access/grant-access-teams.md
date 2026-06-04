---
title: Conceder acceso a los equipos
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los equipos de Workfront
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
TQID: https://experienceleague.adobe.com/Z9KMDwzTwBZLGjLtfxd3H42jd12-7ob3RCn0-IXN-Hc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 677
ht-degree: 79%

---

# Conceder acceso a los equipos

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los equipos de Workfront, como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Configure el acceso de los usuarios a los equipos de edición mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de Equipos y, a continuación, seleccione las capacidades que desea conceder en **Ajuste la configuración**.

   ![equipos de afinación](assets/fine-tune-teams.png)

   * **Ver**: si está configurando cómo los usuarios con cualquier licencia pueden ver los equipos, cambie cualquiera de las siguientes opciones:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Ver equipos asociados con mis grupos</td>
         <td>
          <p><b>Habilitado</b>: cuando los usuarios buscan equipos en un campo de escritura anticipada de equipo, pueden ver los equipos asociados con sus grupos, sean o no integrantes del equipo. </p>
          <p><b>Deshabilitado</b>: cuando los usuarios buscan equipos en un campo de escritura anticipada de equipo, pueden ver los equipos asociados con sus grupos únicamente cuando sean integrantes del equipo.</p><p>Esta opción está habilitada de forma predeterminada.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Ver todos los equipos</td>
         <td><p>Cuando esta opción está habilitada y los usuarios buscan equipos en un campo de escritura anticipada de equipo, los usuarios pueden ver y seleccionar cualquier equipo.</p><p>Esta opción está habilitada de forma predeterminada. </p></td>
        </tr>
       </tbody>
      </table>

   * **Editar**: Si está configurando la forma en que los usuarios con una licencia estándar, de plan o de trabajo pueden administrar equipos, cambie cualquiera de las siguientes opciones:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Crear</td>
         <td><p>Permite a los usuarios con una licencia estándar, de planificación o de trabajo crear equipos.</p><p>Esta opción está habilitada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eliminar</td>
         <td><p> Permite a los usuarios con una licencia estándar o de planificación eliminar los equipos a los que tienen acceso para editar (no disponible para los usuarios con una licencia de trabajo).</p><p>Esta opción está habilitada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar los equipos de los grupos que administro (solo para Administradores de grupos)</td>
         <td><p>Permite a los usuarios con licencia estándar o de planificación designados como administradores de grupos editar los equipos asociados con los grupos que administran.</p><p>Esta opción está habilitada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar los equipos en los que estoy</td>
         <td><p>Permite a los usuarios con una licencia estándar, de planificación o de trabajo editar equipos de los que son miembros.</p><p>Esta opción está desactivada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Ver equipos asociados con mis grupos</td>
         <td>
         <p><b>Habilitado</b>: cuando los usuarios buscan equipos en un campo de escritura anticipada de equipo, pueden ver los equipos asociados con sus grupos, sean o no integrantes del equipo. </p>
         <p><b>Deshabilitado</b>: cuando los usuarios buscan equipos en un campo de escritura anticipada de equipo, pueden ver los equipos asociados con sus grupos únicamente cuando sean integrantes del equipo.</p><p>Esta opción está habilitada de forma predeterminada.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Ver todos los equipos</td>
         <td><p>Cuando esta opción está habilitada y los usuarios buscan equipos en un campo de escritura anticipada de equipo, los usuarios pueden ver y seleccionar cualquier equipo.</p><p>Esta opción está habilitada de forma predeterminada. </p></td>
        </tr>
       </tbody>
      </table>



1. Haga clic en la X para cerrar el cuadro **Ajustar la configuración**.
1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

>[!NOTE]
>
>* Lo siguiente se cumple, independientemente de la configuración del nivel de acceso:
>
>   * Los propietarios de equipos siempre pueden ver y editar sus equipos
>   * Los usuarios siempre tienen acceso para ver los equipos en los que están
>
>* La configuración de cualquier opción disponible tanto para Ver como para Editar (como “Ver equipos asociados con mis grupos”) se conservará si decide seleccionar Ver en lugar de Editar o Editar en lugar de Ver en un nivel de acceso.
>

## Acceso a equipos por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los equipos, vea la sección [Equipos](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#teams) en el artículo [Funcionalidad disponible para cada tipo de objeto](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).
