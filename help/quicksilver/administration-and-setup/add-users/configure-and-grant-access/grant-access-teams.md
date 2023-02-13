---
title: Concesión de acceso a equipos
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los equipos en Workfront
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 4%

---

# Concesión de acceso a equipos

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los equipos en Workfront, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acceso

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuración del acceso de los usuarios para editar los usuarios mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono del engranaje ![](assets/gear-icon-settings.png) en el **Ver** o **Editar** a la derecha de Equipos y, a continuación, seleccione las capacidades que desea conceder en **Ajustar la configuración**.

   * **Ver**: Si está configurando cómo pueden ver los equipos los usuarios con cualquier licencia, cambie cualquiera de las siguientes opciones:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Ver equipos asociados con mis grupos</td>
         <td>
          <p><b>Habilitado</b>: Cuando los usuarios buscan equipos en un campo de avance de tipo Equipo , los usuarios pueden ver los equipos asociados a sus grupos, sean o no miembros del equipo. </p>
          <p><b>Desactivado</b>: Cuando los usuarios buscan equipos en un campo de avance de tipo Equipo , los usuarios pueden ver los equipos asociados a sus grupos solo donde son miembros del equipo</p><p>Esta opción está activada de forma predeterminada.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Ver todos los equipos</td>
         <td><p>Cuando esta opción está habilitada y los usuarios buscan equipos en un campo de avance de tipo Equipo , los usuarios pueden ver y seleccionar cualquier equipo.</p><p>Esta opción está activada de forma predeterminada. </p></td>
        </tr>
       </tbody>
      </table>

   * **Editar**: Si está configurando cómo los usuarios con una licencia de Plan y una licencia de trabajo pueden administrar equipos, cambie cualquiera de las siguientes opciones:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Crear</td>
         <td><p>Permite a los usuarios con una licencia Plan o una licencia de trabajo crear equipos.</p><p>Esta opción está activada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eliminar</td>
         <td><p> Permite a los usuarios con una licencia de Plan eliminar los equipos a los que tienen acceso para editar (no disponible para los usuarios con una licencia de trabajo).</p><p>Esta opción está activada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar los equipos de los grupos que administro (solo para Administradores de grupos)</td>
         <td><p>Permite a los usuarios de licencias del Plan designados como administradores de grupos editar los equipos asociados con los grupos que administran.</p><p>Esta opción está activada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar equipos en los que estoy</td>
         <td><p>Permite a los usuarios planificar licencias o licencias de trabajo editar equipos de los que sean miembros.</p><p>Esta opción está desactivada de forma predeterminada.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Ver equipos asociados con mis grupos</td>
         <td>
         <p><b>Habilitado</b> Cuando los usuarios buscan equipos en un campo de avance de tipo Equipo , los usuarios pueden ver los equipos asociados a sus grupos, sean o no miembros del equipo. </p>
         <p><b>Desactivado</b>: Cuando los usuarios buscan equipos en un campo de avance de tipo Equipo , los usuarios pueden ver los equipos asociados a sus grupos solo donde son miembros del equipo</p><p>Esta opción está activada de forma predeterminada.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Ver todos los equipos</td>
         <td><p>Cuando esta opción está habilitada y los usuarios buscan equipos en un campo de avance de tipo Equipo , los usuarios pueden ver y seleccionar cualquier equipo.</p><p>Esta opción está activada de forma predeterminada. </p></td>
        </tr>
       </tbody>
      </table>

1. Haga clic en la X para cerrar la **Ajustar la configuración** en la ventana
1. (Opcional) Para configurar las opciones de acceso de otros objetos y áreas del nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando haya terminado, haga clic en **Guardar**.

>[!NOTE]
>
>* Los siguientes son verdaderos, independientemente de la configuración del nivel de acceso:
   >
   >   * Los propietarios de equipos siempre pueden ver y editar sus equipos
   >   * Los usuarios siempre tienen acceso para ver los equipos en los que se encuentran
>
* La configuración de cualquier opción disponible tanto para Vista como para Editar (como &quot;Ver equipos asociados a mis grupos&quot;) se mantiene si decide seleccionar Ver en lugar de Editar o Editar en lugar de Ver en un nivel de acceso.
>


## Acceso a equipos por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con los problemas, consulte la sección [Equipos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
