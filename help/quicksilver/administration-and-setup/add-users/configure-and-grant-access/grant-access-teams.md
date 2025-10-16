---
title: Conceder acceso a los equipos
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los equipos de Workfront
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 99%

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
   <td role="rowheader">paquete de Adobe Workfront</td> 
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

## Configurar el acceso de los usuarios para editar usuarios con un nivel de acceso personalizado

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

   * **Editar**: si está configurando cómo los usuarios con una licencia de planificación y una licencia de trabajo pueden administrar equipos, cambie cualquiera de las siguientes opciones:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Crear</td>
         <td><p>Permite a los usuarios con una licencia de planificación o de trabajo crear equipos.</p><p>Esta opción está habilitada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eliminar</td>
         <td><p> Permite a los usuarios con una licencia de planificación eliminar los equipos a los que tienen acceso de edición (no disponible para los usuarios con una licencia de trabajo).</p><p>Esta opción está habilitada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar los equipos de los grupos que administro (solo para Administradores de grupos)</td>
         <td><p>Permite a los usuarios con una licencia de planificación designados como administradores de grupos editar los equipos asociados con los grupos que administran.</p><p>Esta opción está habilitada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar los equipos en los que estoy</td>
         <td><p>Permite a los usuarios con una licencia de planificación o una licencia de trabajo editar equipos de los que son integrantes.</p><p>Esta opción está desactivada de forma predeterminada.</p></td>
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



1. Haga clic en la X para cerrar el cuadro **Ajuste la configuración**.
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

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los problemas, vea la sección [Equipos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
